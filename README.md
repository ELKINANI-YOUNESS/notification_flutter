This code snippet is for initializing and showing notifications using the flutter_local_notifications package in Flutter.

The _initializeNotifications function is responsible for initializing the plugin with the specified settings. It sets the default Android icon for the notifications using AndroidInitializationSettings.

The _showNotification function is used to show a notification with the given title and body. It first formats the elapsed time using the TimerUtil.formatTime method and appends it to the body.

It then creates an AndroidNotificationDetails object with the specified settings for the notification. The actions parameter allows you to add custom actions to the notification, in this case, a "Star" action and a "Stop Time" action. Each action is defined using AndroidNotificationAction, specifying the action's ID, label, and icon.

Finally, it creates a NotificationDetails object with the Android specific settings and shows the notification using flutterLocalNotificationsPlugin.show. The notification ID is set to 0, and the title, body, and platformChannelSpecifics are provided.
