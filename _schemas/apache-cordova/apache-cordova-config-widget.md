---
description: Root configuration element of the Apache Cordova config.xml file, defining app identity, metadata, and behavior preferences.
layout: schema
name: Widget
properties_list:
- description: Reverse-DNS format unique app identifier (e.g., com.example.myapp).
  name: id
  type: string
- description: Major/minor/patch version number for the application.
  name: version
  type: string
- description: Alternative version for Android; overrides the versionCode auto-generated from version.
  name: android-versionCode
  type: string
- description: Alternative version string for iOS build.
  name: ios-CFBundleVersion
  type: string
- description: Required W3C widgets namespace.
  name: xmlns
  type: string
- description: Formal display name of the application.
  name: name
  type: string
- description: Metadata description used for app-store listings.
  name: description
  type: string
- description: Author contact information.
  name: author
  type: object
- description: Defines the app's starting page.
  name: content
  type: object
- description: Array of preference settings controlling application behavior.
  name: preferences
  type: array
- description: List of plugins to restore.
  name: plugins
  type: array
- description: List of target platforms.
  name: platforms
  type: array
provider_name: Apache Cordova
provider_slug: apache-cordova
schema_file: json-schema/apache-cordova-config-widget-schema.json
slug: apache-cordova-config-widget
tags:
- Apache
- Cross-Platform
- Hybrid Apps
- JavaScript
- Mobile
- Open Source
- Plugins
title: Widget
---
