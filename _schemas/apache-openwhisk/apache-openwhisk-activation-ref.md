---
description: ActivationRef schema from Apache OpenWhisk
layout: schema
name: ActivationRef
properties_list:
- description: Activation identifier for async invocations
  name: activationId
  type: string
provider_name: Apache OpenWhisk
provider_slug: apache-openwhisk
schema_file: json-schema/apache-openwhisk-activation-ref-schema.json
slug: apache-openwhisk-activation-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-activation-ref-schema.json\",\n  \"title\": \"ActivationRef\",\n  \"description\": \"ActivationRef schema from Apache OpenWhisk\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activationId\": {\n      \"type\": \"string\",\n      \"description\": \"Activation identifier for async invocations\",\n      \"example\": \"44794bd6aab74415b4e42a308d880727\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openwhisk/refs/heads/main/json-schema/apache-openwhisk-activation-ref-schema.json
tags:
- Cloud Native
- Event-Driven
- FaaS
- Serverless
- Apache
- Open Source
- Functions
title: ActivationRef
---
