---
description: ''
layout: schema
name: CollectRequest
properties_list:
- description: An array of events to send to the Edge Network.
  name: events
  type: array
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/data-collection-collect-request-schema.json
slug: data-collection-collect-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"An array of events to send to the Edge Network.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/data-collection-collect-request-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: CollectRequest
---
