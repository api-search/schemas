---
description: UpdateConfigurationResponse schema from Amazon MSK API
layout: schema
name: UpdateConfigurationResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: LatestRevision
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-configuration-response-schema.json
slug: msk-api-update-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-configuration-response-schema.json\",\n  \"title\": \"UpdateConfigurationResponse\",\n  \"description\": \"UpdateConfigurationResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) of the configuration.</p>\"\n        }\n      ]\n    },\n    \"LatestRevision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationRevision\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"latestRevision\"\n          },\n          \"description\": \"\\n    \
  \        <p>Latest revision of the configuration.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-configuration-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateConfigurationResponse
---
