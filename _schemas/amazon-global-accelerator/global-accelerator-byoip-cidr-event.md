---
description: A complex type that contains a <code>Message</code> and a <code>Timestamp</code> value for changes that you make in the status of an IP address range that you bring to Global Accelerator through bring your own IP address (BYOIP).
layout: schema
name: ByoipCidrEvent
properties_list:
- description: ''
  name: Message
  type: object
- description: ''
  name: Timestamp
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-byoip-cidr-event-schema.json
slug: global-accelerator-byoip-cidr-event
source_filename: global-accelerator-byoip-cidr-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-byoip-cidr-event-schema.json\",\n  \"title\": \"ByoipCidrEvent\",\n  \"description\": \"A complex type that contains a <code>Message</code> and a <code>Timestamp</code> value for changes that you make in the status of an IP address range that you bring to Global Accelerator through bring your own IP address (BYOIP).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A string that contains an <code>Event</code> message describing changes that you make in the status of an IP address range that you bring to Global Accelerator through bring your own IP address (BYOIP).\"\n        }\n      ]\n    },\n    \"Timestamp\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp for when you make a status change for an IP address range that you bring to Global Accelerator through bring your own IP address (BYOIP).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-byoip-cidr-event-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: ByoipCidrEvent
---
