---
description: NamespaceLimits schema from Apache OpenWhisk
layout: schema
name: NamespaceLimits
properties_list:
- description: Maximum concurrent activations
  name: concurrency
  type: integer
- description: Actions per minute limit
  name: minuteRate
  type: integer
- description: Actions per hour limit
  name: hourRate
  type: integer
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-namespace-limits-schema.json
slug: apache-openwhisk-namespace-limits
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-namespace-limits-schema.json\",\n  \"title\": \"NamespaceLimits\",\n  \"description\": \"NamespaceLimits schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"concurrency\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum concurrent activations\",\n      \"example\": 1000\n    },\n    \"minuteRate\": {\n      \"type\": \"integer\",\n      \"description\": \"Actions per minute limit\",\n      \"example\": 600\n    },\n    \"hourRate\": {\n      \"type\": \"integer\",\n      \"description\": \"Actions per hour limit\",\n      \"example\": 36000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-namespace-limits-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: NamespaceLimits
---
