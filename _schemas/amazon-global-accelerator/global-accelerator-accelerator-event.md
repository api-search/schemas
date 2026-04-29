---
description: A complex type that contains a <code>Timestamp</code> value and <code>Message</code> for changes that you make to an accelerator in Global Accelerator. Messages stored here provide progress or error information when you update an accelerator from IPv4 to dual-stack, or from dual-stack to IPv4. Global Accelerator stores a maximum of ten event messages.
layout: schema
name: AcceleratorEvent
properties_list:
- description: ''
  name: Message
  type: object
- description: ''
  name: Timestamp
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-accelerator-event-schema.json
slug: global-accelerator-accelerator-event
source_filename: global-accelerator-accelerator-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-accelerator-event-schema.json\",\n  \"title\": \"AcceleratorEvent\",\n  \"description\": \"A complex type that contains a <code>Timestamp</code> value and <code>Message</code> for changes that you make to an accelerator in Global Accelerator. Messages stored here provide progress or error information when you update an accelerator from IPv4 to dual-stack, or from dual-stack to IPv4. Global Accelerator stores a maximum of ten event messages. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A string that contains an <code>Event</code> message describing changes or errors when you update an accelerator in Global Accelerator\
  \ from IPv4 to dual-stack, or dual-stack to IPv4.\"\n        }\n      ]\n    },\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp for when you update an accelerator in Global Accelerator from IPv4 to dual-stack, or dual-stack to IPv4.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-accelerator-event-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: AcceleratorEvent
---
