# JW Player Webhook Notification Server

This project is a real-time notification backend built with Express,
Supabase, and Firebase Cloud Messaging (FCM).

## 💡 Why This Project Exists

When new videos are uploaded or live streams start in JW Player, users
should instantly receive a push notification on their devices.

This server makes that happen automatically.

## ⚙️ What It Does

-   Listens to JW Player webhook events
-   Stores notification data in Supabase (PostgreSQL)
-   Sends push notifications using Firebase Cloud Messaging
-   Keeps track of which device received which notification

## 🔄 How It Works

1.  JW Player triggers a webhook event (e.g., new video or live stream).
2.  The server receives the event.
3.  A notification record is saved in the database.
4.  All registered devices are linked to the notification.
5.  Push notifications are sent instantly via Firebase FCM.
6.  Devices can later fetch and display their notification history.

## 🎯 Purpose

This project provides a scalable foundation for:

-   Video platform notifications
-   Live stream alerts
-   Media updates
-   Real-time mobile push systems

------------------------------------------------------------------------

Simple, scalable backend for real-time video notification systems.
