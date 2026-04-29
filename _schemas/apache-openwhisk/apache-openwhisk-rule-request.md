---
description: RuleRequest schema from Apache OpenWhisk
layout: schema
name: RuleRequest
properties_list:
- description: Trigger name to associate
  name: trigger
  type: string
- description: Action name to invoke
  name: action
  type: string
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-rule-request-schema.json
slug: apache-openwhisk-rule-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-rule-request-schema.json\",\n  \"title\": \"RuleRequest\",\n  \"description\": \"RuleRequest schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"trigger\": {\n      \"type\": \"string\",\n      \"description\": \"Trigger name to associate\",\n      \"example\": \"/guest/myTrigger\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Action name to invoke\",\n      \"example\": \"/guest/hello\"\n    }\n  },\n  \"required\": [\n    \"trigger\",\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-rule-request-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: RuleRequest
---
