---
name: Xamarin.Android - Messenger and Service
description: "Example of IPC communication between an Android service and an activity (using a messenger and a handler)"
page_type: sample
languages:
- csharp
products:
- xamarin
urlFragment: applicationfundamentals-servicesamples-messengerservicedemo
---
# Xamarin.Android Messenger and Service Sample

This solution is an example of IPC communication between an Android service and an Activity (using a Messenger and a Handler). It demonstrates how to perform one-way and two-way IPC calls between an Activity and a Service running in it's own process.

Ensure that the **MessengerService** project is installed on the device _before_ the **MessengerClient** project. If the **MessengerClient** is inadvertently installed first, it will be necessary to uninstall it, install the **MessengerService** app, and then reinstall the **MessengerClient** project.

![Buttons to test messenger services](Screenshots/service-messenger-activity.png)

**Note**: Currently it is not possible to implement an `IsolatedProcess` in Xamarin.Android. Please see [Bugzilla 51940 -  Services with isolated processes and custom Application class fail to resolve overloads properly](https://bugzilla.xamarin.com/show_bug.cgi?id=51940) for more details.