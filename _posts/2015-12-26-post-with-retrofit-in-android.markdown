---
layout: post
title:  "Send HTTP Post using Retrofit, in Android"
date:   2014-12-26
author: Macha Da Costa
category: android
image: droid_request.png
excerpt: This post is about using retorfit in an android project.
---

This tutorial explain how to make a HTTP POST request wwith the library Retrofit in an Android project. JSON format with Retrofit version 2.0 is used.

# Configure project to use Retrofit
First of all, we have to import the last version of Retrofit library in our Android Studio project.

1. Create a new Android project or Open an existing one.
2. In the gradle file of the project, the one attached to app/ module (not the one attached to the whole project!), include the library:

	```java
	 dependencies {
		compile 'com.squareup.retrofit:retrofit:2.0.0-beta2'
	 } 
	```
3. In the same gradle file, import a JSON converter:

	```java
	dependencies {
		compile 'com.squareup.retrofit:converter-gson:2.0.0-beta2'
	}
	```
4. Add permission to authorize application to connect to the internet in the Manifest file of the project, AndroidManifest.xml (beetween manifest and application tag):

	```xml
	<uses-permission android:name="android.permission.INTERNET" />
	```
