---
description: String dictionary resource.
layout: schema
name: ConnectionStringDictionary
properties_list:
- description: Connection strings.
  name: properties
  type: object
provider_name: Azure Function Apps
provider_slug: azure-function-apps
schema_file: json-schema/azure-function-apps-connection-string-dictionary-schema.json
slug: azure-function-apps-connection-string-dictionary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-connection-string-dictionary-schema.json\",\n  \"title\": \"ConnectionStringDictionary\",\n  \"description\": \"String dictionary resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"properties\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/ConnStringValueTypePair\"\n      },\n      \"description\": \"Connection strings.\",\n      \"type\": \"object\",\n      \"x-ms-client-flatten\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-function-apps/refs/heads/main/json-schema/azure-function-apps-connection-string-dictionary-schema.json
tags:
- Azure
- Compute
- FaaS
- Functions
- Serverless
title: ConnectionStringDictionary
---
