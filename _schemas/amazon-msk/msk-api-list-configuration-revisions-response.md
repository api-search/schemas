---
description: ListConfigurationRevisionsResponse schema from Amazon MSK API
layout: schema
name: ListConfigurationRevisionsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Revisions
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-list-configuration-revisions-response-schema.json
slug: msk-api-list-configuration-revisions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-configuration-revisions-response-schema.json\",\n  \"title\": \"ListConfigurationRevisionsResponse\",\n  \"description\": \"ListConfigurationRevisionsResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"\\n            <p>Paginated results marker.</p>\"\n        }\n      ]\n    },\n    \"Revisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfConfigurationRevision\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"revisions\"\n          },\n          \"description\": \"\\\
  n            <p>List of ConfigurationRevision objects.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-configuration-revisions-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListConfigurationRevisionsResponse
---
