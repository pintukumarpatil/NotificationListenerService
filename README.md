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

![Mou icon](https://github.com/pintukumarpatil/NotificationListenerService/blob/master/NotificationListener/screen/device-2016-08-31-170319.png)
