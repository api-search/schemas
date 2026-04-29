---
description: List of ActiveMQ queues
layout: schema
name: QueueList
properties_list:
- description: ''
  name: queues
  type: array
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-queue-list-schema.json
slug: apache-servicemix-queue-list
source_filename: apache-servicemix-queue-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-queue-list-schema.json\",\n  \"title\": \"QueueList\",\n  \"description\": \"List of ActiveMQ queues\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queues\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Queue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-queue-list-schema.json
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: QueueList
---
