---
description: ListDiscoveredResourcesRequest schema from Amazon Migration Hub API
layout: schema
name: ListDiscoveredResourcesRequest
properties_list:
- description: ''
  name: ProgressUpdateStream
  type: object
- description: ''
  name: MigrationTaskName
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-list-discovered-resources-request-schema.json
slug: migration-hub-api-list-discovered-resources-request
source_filename: migration-hub-api-list-discovered-resources-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-discovered-resources-request-schema.json\",\n  \"title\": \"ListDiscoveredResourcesRequest\",\n  \"description\": \"ListDiscoveredResourcesRequest schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProgressUpdateStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProgressUpdateStream\"\n        },\n        {\n          \"description\": \"The name of the ProgressUpdateStream.\"\n        }\n      ]\n    },\n    \"MigrationTaskName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MigrationTaskName\"\n        },\n        {\n          \"description\": \"The name of the MigrationTask. <i>Do not store personal data in this field.</i> \"\n        }\n      ]\n    },\n    \"NextToken\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"If a <code>NextToken</code> was returned by a previous call, there are more results available. To retrieve the next page of results, make the call again using the returned token in <code>NextToken</code>.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResultsResources\"\n        },\n        {\n          \"description\": \"The maximum number of results returned per page.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ProgressUpdateStream\",\n    \"MigrationTaskName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-discovered-resources-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ListDiscoveredResourcesRequest
---
