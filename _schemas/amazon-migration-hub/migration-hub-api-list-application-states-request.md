---
description: ListApplicationStatesRequest schema from Amazon Migration Hub API
layout: schema
name: ListApplicationStatesRequest
properties_list:
- description: ''
  name: ApplicationIds
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-list-application-states-request-schema.json
slug: migration-hub-api-list-application-states-request
source_filename: migration-hub-api-list-application-states-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-application-states-request-schema.json\",\n  \"title\": \"ListApplicationStatesRequest\",\n  \"description\": \"ListApplicationStatesRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationIds\"\n        },\n        {\n          \"description\": \"The configurationIds from the Application Discovery Service that uniquely identifies your applications.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"If a <code>NextToken</code> was returned by a previous call, there are more results available.\
  \ To retrieve the next page of results, make the call again using the returned token in <code>NextToken</code>.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"Maximum number of results to be returned per page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-application-states-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListApplicationStatesRequest
---
