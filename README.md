# Kepi

Dynamically replace strings for Android applications
Built on top of [Philology](https://github.com/JcMinarro/Philology) and [AWS](https://aws.amazon.com), Kepi provides a complete solution to manage Android string resources.

## Overnight update

[WorkManager](https://developer.android.com/topic/libraries/architecture/workmanager) is used to schedule a [PeriodicWorkRequest](https://developer.android.com/reference/androidx/work/PeriodicWorkRequest.html) at a convenient moment : WiFi enabled, battery charging, device idle. For most people, this will be in the evening.

## Realtime update
Websockets are used to push new updates to active users as soon as you upload a new resource file. When the application starts, a check for new resources is made and a persistent connection. Active users will see the update in minutes.