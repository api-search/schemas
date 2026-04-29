---
description: DeleteConfigurationResponse schema from Amazon MSK API
layout: schema
name: DeleteConfigurationResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-delete-configuration-response-schema.json
slug: msk-api-delete-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-delete-configuration-response-schema.json\",\n  \"title\": \"DeleteConfigurationResponse\",\n  \"description\": \"DeleteConfigurationResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) that uniquely identifies an MSK configuration.</p>\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"\\n\
  \            <p>The state of the configuration. The possible states are ACTIVE, DELETING, and DELETE_FAILED. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-delete-configuration-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DeleteConfigurationResponse
---
