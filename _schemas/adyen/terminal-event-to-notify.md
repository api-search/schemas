---
description: Event the POI notifies to the Sale System.
layout: schema
name: EventToNotify
properties_list: []
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-event-to-notify-schema.json
slug: terminal-event-to-notify
source_filename: terminal-event-to-notify-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-event-to-notify-schema.json\",\n  \"title\": \"EventToNotify\",\n  \"description\": \"Event the POI notifies to the Sale System.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"Abort\",\n    \"BeginMaintenance\",\n    \"CardInserted\",\n    \"CardRemoved\",\n    \"Completed\",\n    \"CustomerLanguage\",\n    \"EndMaintenance\",\n    \"Initialised\",\n    \"KeyPressed\",\n    \"OutOfOrder\",\n    \"Reject\",\n    \"SaleAdmin\",\n    \"SaleWakeUp\",\n    \"SecurityAlarm\",\n    \"Shutdown\",\n    \"StopAssistance\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-event-to-notify-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EventToNotify
---
