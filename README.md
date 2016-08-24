NotificationListenerService
===================================

##Introduction
NotificationListenerService is introduced in Android 4.3 (API 18). It allows an application to receive information about notifications as it creates or removes. NotificationListenerService class is derived from the Service class. It has two abstract methods namely 1. onNotificationPosted 2. onNotificationRemoved.  
To use NotificationListenerService, we need to create a java file which extends NotificationListenerService and implement two callback methods. Both methods have a parameter named "sbn", which is an object of StatusBarNotification class. StatusBarNotification provides necessary information about Notifications.
NotificationListenerService provides facility to fetch active notifications using getActiveNotifications and also provides a feature to remove notifications using cancelAllNotifications.

##Useful Methods
1. NotificationListenerService
	* onNotificationPosted
	* onNotificationRemoved
2. StatusBarNotification
	* getId
	* getNotification
	* getPackageName
	* getPostTime
	* isClearable
	* isOngoing

##Note
User require to enable notification permission from "Settings > Security > Notification access".
And Also user can take permission by using PERMISSION ON/OFF Button

![Mou icon](https://photos.google.com/share/AF1QipM7I7T6o2A7ljhMMsSRcX8vPvEFcK7yNjif9PH8JygS7uBfGEice4JKuk7CfnqtfA/photo/AF1QipMSAsQyEhK5YLEHSlJFccWonnirRDBmu-S9J2lo?key=OC02Zl9wVEFwVnEweTVNNWZ4Sk9nYnNqVXNvZk13)
![Mou icon](https://photos.google.com/share/AF1QipOwjD6366yi2iOHrYbLJv8t1r9eIRvsbLGOpvqoNkubdJ1KH2AFzy9OB8jEody9WA/photo/AF1QipMvJGy6My__B5UXtj1obawOyB1Tfc8ofj453rAa?key=LVY4Z3BUZHZWSElnV1JhSWxNQnNVM1MwdHBGbFNn)
