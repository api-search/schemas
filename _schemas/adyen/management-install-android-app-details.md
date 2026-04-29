---
description: InstallAndroidAppDetails schema from Adyen API
layout: schema
name: InstallAndroidAppDetails
properties_list:
- description: The unique identifier of the app to be installed.
  name: appId
  type: string
- description: 'Type of terminal action: Install an Android app.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-install-android-app-details-schema.json
slug: management-install-android-app-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-install-android-app-details-schema.json\",\n  \"title\": \"InstallAndroidAppDetails\",\n  \"description\": \"InstallAndroidAppDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appId\": {\n      \"description\": \"The unique identifier of the app to be installed.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"InstallAndroidApp\",\n      \"description\": \"Type of terminal action: Install an Android app.\",\n      \"enum\": [\n        \"InstallAndroidApp\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-install-android-app-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InstallAndroidAppDetails
---
