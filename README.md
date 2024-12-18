# Лабораторная работа №6. Уведомления.

**Выполнила**: Рябых

**Язык программирования**: Java

## Что делает приложение?
Приложение позволяет пользователю создавать, просматривать, и удалять напоминания с заданными датой и временем. 

### Основной функционал:
1. **Создание напоминаний**:
   - Заголовок, текст, дата и время напоминания задаются пользователем.
   - Используются `TimePickerDialog` и `DatePickerDialog` для выбора даты и времени.
   - Напоминания сохраняются в базу данных (SQLite).

2. **Просмотр напоминаний**:
   - Список всех установленных напоминаний с указанием даты и времени.

3. **Удаление напоминаний**:
   - Возможность удаления напоминания из базы данных и отмены запланированного уведомления.

4. **Отображение уведомлений**:
   - Напоминания стилизуются в `Notification Center` и `Status Bar` (собственный логотип).
   - При нажатии на уведомление происходит переход в активность приложения, где отображается полный текст напоминания.

## Техническая реализация:
- Уведомления реализуются с помощью классов `Notification`, `NotificationManager`, `PendingIntent`, `BroadcastReceiver`, и `AlarmManager`.
- Хранение данных осуществляется в базе данных SQLite.
- Установка даты и времени — через `TimePickerDialog` и `DatePickerDialog`.
