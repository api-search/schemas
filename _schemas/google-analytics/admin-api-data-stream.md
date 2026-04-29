---
description: A resource message representing a data stream.
layout: schema
name: DataStream
properties_list:
- description: Data specific to Android app streams.
  name: androidAppStreamData
  type: object
- description: Output only. Time when this stream was originally created.
  name: createTime
  type: string
- description: Human-readable display name for the Data Stream. Required for web data streams. The max allowed display name length is 255 UTF-16 code units.
  name: displayName
  type: string
- description: Data specific to iOS app streams.
  name: iosAppStreamData
  type: object
- description: 'Output only. Resource name of this Data Stream. Format: properties/{property_id}/dataStreams/{stream_id} Example: "properties/1000/dataStreams/2000"'
  name: name
  type: string
- description: Required. Immutable. The type of this DataStream resource.
  name: type
  type: string
- description: Output only. Time when stream payload fields were last updated.
  name: updateTime
  type: string
- description: Data specific to web streams.
  name: webStreamData
  type: object
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-data-stream-schema.json
slug: admin-api-data-stream
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-data-stream-schema.json\",\n  \"title\": \"DataStream\",\n  \"description\": \"A resource message representing a data stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"androidAppStreamData\": {\n      \"description\": \"Data specific to Android app streams.\",\n      \"properties\": {\n        \"firebaseAppId\": {\n          \"description\": \"Output only. ID of the corresponding Android app in Firebase, if any. This ID can change if the Android app is deleted and recreated.\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"packageName\": {\n          \"description\": \"Immutable. The package name for the app being measured. Example: \\\"com.example.myandroidapp\\\"\",\n          \"type\": \"string\"\n        }\n      },\n      \"type\": \"\
  object\"\n    },\n    \"createTime\": {\n      \"description\": \"Output only. Time when this stream was originally created.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"Human-readable display name for the Data Stream. Required for web data streams. The max allowed display name length is 255 UTF-16 code units.\",\n      \"type\": \"string\"\n    },\n    \"iosAppStreamData\": {\n      \"description\": \"Data specific to iOS app streams.\",\n      \"properties\": {\n        \"bundleId\": {\n          \"description\": \"Required. Immutable. The Apple App Store Bundle ID for the app Example: \\\"com.example.myiosapp\\\"\",\n          \"type\": \"string\"\n        },\n        \"firebaseAppId\": {\n          \"description\": \"Output only. ID of the corresponding iOS app in Firebase, if any. This ID can change if the iOS app is deleted and recreated.\",\n          \"readOnly\": true,\n\
  \          \"type\": \"string\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"name\": {\n      \"description\": \"Output only. Resource name of this Data Stream. Format: properties/{property_id}/dataStreams/{stream_id} Example: \\\"properties/1000/dataStreams/2000\\\"\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Required. Immutable. The type of this DataStream resource.\",\n      \"enum\": [\n        \"DATA_STREAM_TYPE_UNSPECIFIED\",\n        \"WEB_DATA_STREAM\",\n        \"ANDROID_APP_DATA_STREAM\",\n        \"IOS_APP_DATA_STREAM\"\n      ],\n      \"type\": \"string\"\n    },\n    \"updateTime\": {\n      \"description\": \"Output only. Time when stream payload fields were last updated.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"webStreamData\": {\n      \"description\": \"Data specific to web streams.\",\n      \"properties\": {\n  \
  \      \"defaultUri\": {\n          \"description\": \"Domain name of the web app being measured, or empty. Example: \\\"http://www.google.com\\\", \\\"https://www.google.com\\\"\",\n          \"type\": \"string\"\n        },\n        \"firebaseAppId\": {\n          \"description\": \"Output only. ID of the corresponding web app in Firebase, if any. This ID can change if the web app is deleted and recreated.\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        },\n        \"measurementId\": {\n          \"description\": \"Output only. Analytics Measurement ID. Example: \\\"G-1A2BCD345E\\\"\",\n          \"readOnly\": true,\n          \"type\": \"string\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-data-stream-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: DataStream
---
