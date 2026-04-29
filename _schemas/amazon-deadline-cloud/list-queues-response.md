---
description: Response containing a list of queues.
layout: schema
name: List Queues Response
properties_list:
- description: ''
  name: queues
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/list-queues-response-schema.json
slug: list-queues-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/list-queues-response-schema.json\",\n  \"title\": \"List Queues Response\",\n  \"description\": \"Response containing a list of queues.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queues\": {\n      \"type\": \"array\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/list-queues-response-schema.json
tags:
- AWS
- Compute
- Media
- Rendering
- Visual Effects
title: List Queues Response
---
