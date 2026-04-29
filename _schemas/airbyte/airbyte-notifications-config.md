---
description: Configures workspace notifications.
layout: schema
name: NotificationsConfig
properties_list:
- description: ''
  name: failure
  type: object
- description: ''
  name: success
  type: object
- description: ''
  name: connectionUpdate
  type: object
- description: ''
  name: connectionUpdateActionRequired
  type: object
- description: ''
  name: syncDisabled
  type: object
- description: ''
  name: syncDisabledWarning
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-notifications-config-schema.json
slug: airbyte-notifications-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-notifications-config-schema.json\",\n  \"title\": \"NotificationsConfig\",\n  \"description\": \"Configures workspace notifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"failure\": {\n      \"$ref\": \"#/components/schemas/NotificationConfig\"\n    },\n    \"success\": {\n      \"$ref\": \"#/components/schemas/NotificationConfig\"\n    },\n    \"connectionUpdate\": {\n      \"$ref\": \"#/components/schemas/NotificationConfig\"\n    },\n    \"connectionUpdateActionRequired\": {\n      \"$ref\": \"#/components/schemas/NotificationConfig\"\n    },\n    \"syncDisabled\": {\n      \"$ref\": \"#/components/schemas/NotificationConfig\"\n    },\n    \"syncDisabledWarning\": {\n      \"$ref\": \"#/components/schemas/NotificationConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-notifications-config-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: NotificationsConfig
---
