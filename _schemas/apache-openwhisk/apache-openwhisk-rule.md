---
description: Rule schema from Apache OpenWhisk
layout: schema
name: Rule
properties_list:
- description: ''
  name: namespace
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: status
  type: string
- description: Fully qualified trigger name
  name: trigger
  type: string
- description: Fully qualified action name
  name: action
  type: string
- description: ''
  name: updated
  type: integer
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-rule-schema.json
slug: apache-openwhisk-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-rule-schema.json\",\n  \"title\": \"Rule\",\n  \"description\": \"Rule schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"example\": \"guest\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"myRule\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"0.0.1\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"example\": \"active\"\n    },\n    \"trigger\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified trigger name\",\n      \"example\": \"/guest/myTrigger\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Fully qualified action name\",\n      \"example\": \"/guest/hello\"\n    },\n    \"updated\": {\n      \"type\": \"integer\",\n      \"example\": 1718153645993\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-rule-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: Rule
---
