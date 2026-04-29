---
description: ReleaseUpdateDetails schema from Adyen API
layout: schema
name: ReleaseUpdateDetails
properties_list:
- description: 'Type of terminal action: Update Release.'
  name: type
  type: string
- description: Boolean flag that tells if the terminal should update at the first next maintenance call. If false, terminal will update on its configured reboot time.
  name: updateAtFirstMaintenanceCall
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-release-update-details-schema.json
slug: management-release-update-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-release-update-details-schema.json\",\n  \"title\": \"ReleaseUpdateDetails\",\n  \"description\": \"ReleaseUpdateDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"default\": \"ReleaseUpdate\",\n      \"description\": \"Type of terminal action: Update Release.\",\n      \"enum\": [\n        \"ReleaseUpdate\"\n      ],\n      \"type\": \"string\"\n    },\n    \"updateAtFirstMaintenanceCall\": {\n      \"description\": \"Boolean flag that tells if the terminal should update at the first next maintenance call. If false, terminal will update on its configured reboot time.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-release-update-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReleaseUpdateDetails
---
