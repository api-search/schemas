---
description: ListApplicationStatesResult schema from Amazon Migration Hub API
layout: schema
name: ListApplicationStatesResult
properties_list:
- description: ''
  name: ApplicationStateList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-list-application-states-result-schema.json
slug: migration-hub-api-list-application-states-result
source_filename: migration-hub-api-list-application-states-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-application-states-result-schema.json\",\n  \"title\": \"ListApplicationStatesResult\",\n  \"description\": \"ListApplicationStatesResult schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationStateList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationStateList\"\n        },\n        {\n          \"description\": \"A list of Applications that exist in Application Discovery Service.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"If a <code>NextToken</code> was returned by a previous call, there are more results available. To retrieve the next page\
  \ of results, make the call again using the returned token in <code>NextToken</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-application-states-result-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListApplicationStatesResult
---
