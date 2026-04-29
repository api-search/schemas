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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cordova/refs/heads/main/json-schema/apache-cordova-config-widget-schema.json\",\n  \"title\": \"Widget\",\n  \"description\": \"Root configuration element of the Apache Cordova config.xml file, defining app identity, metadata, and behavior preferences.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Reverse-DNS format unique app identifier (e.g., com.example.myapp).\",\n      \"example\": \"com.example.myapp\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Major/minor/patch version number for the application.\",\n      \"example\": \"1.0.0\"\n    },\n    \"android-versionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Alternative version for Android; overrides the versionCode auto-generated from version.\",\n      \"\
  example\": \"10\"\n    },\n    \"ios-CFBundleVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Alternative version string for iOS build.\",\n      \"example\": \"1.0.0\"\n    },\n    \"xmlns\": {\n      \"type\": \"string\",\n      \"description\": \"Required W3C widgets namespace.\",\n      \"example\": \"http://www.w3.org/ns/widgets\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Formal display name of the application.\",\n      \"example\": \"My Cordova App\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Metadata description used for app-store listings.\",\n      \"example\": \"A hybrid mobile application built with Apache Cordova.\"\n    },\n    \"author\": {\n      \"type\": \"object\",\n      \"description\": \"Author contact information.\",\n      \"properties\": {\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Author\
  \ email address.\",\n          \"example\": \"developer@example.com\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Author website URL.\",\n          \"example\": \"https://example.com\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"Author name.\",\n          \"example\": \"Jane Smith\"\n        }\n      }\n    },\n    \"content\": {\n      \"type\": \"object\",\n      \"description\": \"Defines the app's starting page.\",\n      \"properties\": {\n        \"src\": {\n          \"type\": \"string\",\n          \"description\": \"Starting page relative path.\",\n          \"default\": \"index.html\",\n          \"example\": \"index.html\"\n        }\n      }\n    },\n    \"preferences\": {\n      \"type\": \"array\",\n      \"description\": \"Array of preference settings controlling application behavior.\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Preference name.\",\n            \"example\": \"Fullscreen\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Preference value.\",\n            \"example\": \"true\"\n          }\n        },\n        \"required\": [\"name\", \"value\"]\n      }\n    },\n    \"plugins\": {\n      \"type\": \"array\",\n      \"description\": \"List of plugins to restore.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Plugin name.\",\n            \"example\": \"cordova-plugin-camera\"\n          },\n          \"spec\": {\n            \"type\": \"string\",\n            \"description\": \"Plugin version or repository reference.\",\n            \"example\": \"^7.0.0\"\n          }\n        },\n        \"required\"\
  : [\"name\", \"spec\"]\n      }\n    },\n    \"platforms\": {\n      \"type\": \"array\",\n      \"description\": \"List of target platforms.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Platform identifier.\",\n            \"enum\": [\"android\", \"ios\", \"electron\", \"browser\"],\n            \"example\": \"android\"\n          },\n          \"spec\": {\n            \"type\": \"string\",\n            \"description\": \"Platform version.\",\n            \"example\": \"^15.0.0\"\n          }\n        },\n        \"required\": [\"name\"]\n      }\n    }\n  },\n  \"required\": [\"id\", \"version\", \"xmlns\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cordova/refs/heads/main/json-schema/apache-cordova-config-widget-schema.json
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
