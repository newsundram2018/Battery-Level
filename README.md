Flutter uses a flexible system that allows you to call platform-specific APIs whether available in Kotlin or Java code on Android, or in Swift or Objective-C code on iOS.
Flutter’s builtin platform-specific API support does not rely on code generation, but rather on a flexible message passing style. Alternatively, the package Pigeon can be used for sending structured typesafe messages via code generation:

The Flutter portion of the app sends messages to its host, the iOS or Android portion of the app, over a platform channel.

The host listens on the platform channel, and receives the message. It then calls into any number of platform-specific APIs—using the native programming language—and sends a response back to the client, the Flutter portion of the app.


In this repo I had immplemented battery status checker functionality using native android code in kotlin.
