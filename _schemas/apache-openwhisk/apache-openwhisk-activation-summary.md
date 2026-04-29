---
description: ActivationSummary schema from Apache OpenWhisk
layout: schema
name: ActivationSummary
properties_list:
- description: ''
  name: activationId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: start
  type: integer
- description: ''
  name: end
  type: integer
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-activation-summary-schema.json
slug: apache-openwhisk-activation-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-activation-summary-schema.json\",\n  \"title\": \"ActivationSummary\",\n  \"description\": \"ActivationSummary schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activationId\": {\n      \"type\": \"string\",\n      \"example\": \"44794bd6aab74415b4e42a308d880727\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"hello\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"0.0.1\"\n    },\n    \"start\": {\n      \"type\": \"integer\",\n      \"example\": 1718153645993\n    },\n    \"end\": {\n      \"type\": \"integer\",\n      \"example\": 1718153646050\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-activation-summary-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: ActivationSummary
---
