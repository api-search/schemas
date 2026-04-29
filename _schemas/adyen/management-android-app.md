---
description: AndroidApp schema from Adyen API
layout: schema
name: AndroidApp
properties_list:
- description: The description that was provided when uploading the app. The description is not shown on the terminal.
  name: description
  type: string
- description: The error code of the app. It exists if the status is error or invalid.
  name: errorCode
  type: string
- description: The unique identifier of the app.
  name: id
  type: string
- description: The app name that is shown on the terminal.
  name: label
  type: string
- description: The package name that uniquely identifies the Android app.
  name: packageName
  type: string
- description: 'The status of the app. Possible values: * `processing`: the app is being signed and converted to a format that the terminal can handle. * `error`: something went wrong. Check that the app matches the '
  name: status
  type: string
- description: The version number of the app.
  name: versionCode
  type: integer
- description: The app version number that is shown on the terminal.
  name: versionName
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-android-app-schema.json
slug: management-android-app
source_filename: management-android-app-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-android-app-schema.json\",\n  \"title\": \"AndroidApp\",\n  \"description\": \"AndroidApp schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description that was provided when uploading the app. The description is not shown on the terminal.\",\n      \"type\": \"string\"\n    },\n    \"errorCode\": {\n      \"description\": \"The error code of the app. It exists if the status is error or invalid.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the app.\",\n      \"type\": \"string\"\n    },\n    \"label\": {\n      \"description\": \"The app name that is shown on the terminal.\",\n      \"type\": \"string\"\n    },\n    \"packageName\": {\n      \"description\": \"The package\
  \ name that uniquely identifies the Android app.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the app. Possible values: \\n* `processing`: the app is being signed and converted to a format that the terminal can handle.\\n* `error`: something went wrong. Check that the app matches the [requirements](https://docs.adyen.com/point-of-sale/android-terminals/app-requirements).\\n* `invalid`: there is something wrong with the APK file of the app.\\n* `ready`: the app has been signed and converted.\\n* `archived`: the app is no longer available.\",\n      \"type\": \"string\"\n    },\n    \"versionCode\": {\n      \"description\": \"The version number of the app.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"versionName\": {\n      \"description\": \"The app version number that is shown on the terminal.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-android-app-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AndroidApp
---
