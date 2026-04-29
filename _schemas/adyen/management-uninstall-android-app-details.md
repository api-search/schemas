---
description: UninstallAndroidAppDetails schema from Adyen API
layout: schema
name: UninstallAndroidAppDetails
properties_list:
- description: The unique identifier of the app to be uninstalled.
  name: appId
  type: string
- description: 'Type of terminal action: Uninstall an Android app.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-uninstall-android-app-details-schema.json
slug: management-uninstall-android-app-details
source_filename: management-uninstall-android-app-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-uninstall-android-app-details-schema.json\",\n  \"title\": \"UninstallAndroidAppDetails\",\n  \"description\": \"UninstallAndroidAppDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"description\": \"The unique identifier of the app to be uninstalled.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"UninstallAndroidApp\",\n      \"description\": \"Type of terminal action: Uninstall an Android app.\",\n      \"enum\": [\n        \"UninstallAndroidApp\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-uninstall-android-app-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UninstallAndroidAppDetails
---
