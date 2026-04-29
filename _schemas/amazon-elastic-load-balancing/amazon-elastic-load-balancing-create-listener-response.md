---
description: Response from the CreateListener action
layout: schema
name: CreateListenerResponse
properties_list:
- description: Information about the listener
  name: listeners
  type: array
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-create-listener-response-schema.json
slug: amazon-elastic-load-balancing-create-listener-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-create-listener-response-schema.json\",\n  \"title\": \"CreateListenerResponse\",\n  \"description\": \"Response from the CreateListener action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"listeners\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the listener\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Listener\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-create-listener-response-schema.json
tags:
- Amazon Web Services
- AWS
- High Availability
- Load Balancing
- Networking
- Scalability
title: CreateListenerResponse
---
