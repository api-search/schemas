---
description: ListConfigurationsResponse schema from Amazon MSK API
layout: schema
name: ListConfigurationsResponse
properties_list:
- description: ''
  name: Configurations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-list-configurations-response-schema.json
slug: msk-api-list-configurations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-configurations-response-schema.json\",\n  \"title\": \"ListConfigurationsResponse\",\n  \"description\": \"ListConfigurationsResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Configurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurations\"\n          },\n          \"description\": \"\\n            <p>An array of MSK configurations.</p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"\\n            <p>The\
  \ paginated results marker. When the result of a ListConfigurations operation is truncated, the call returns NextToken in the response. \\n               To get another batch of configurations, provide this token in your next request.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-configurations-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListConfigurationsResponse
---
