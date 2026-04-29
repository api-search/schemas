---
description: ListDiscoveredResourcesResult schema from Amazon Migration Hub API
layout: schema
name: ListDiscoveredResourcesResult
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: DiscoveredResourceList
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-list-discovered-resources-result-schema.json
slug: migration-hub-api-list-discovered-resources-result
source_filename: migration-hub-api-list-discovered-resources-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-discovered-resources-result-schema.json\",\n  \"title\": \"ListDiscoveredResourcesResult\",\n  \"description\": \"ListDiscoveredResourcesResult schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"If there are more discovered resources than the max result, return the next token to be passed to the next call as a bookmark of where to start from.\"\n        }\n      ]\n    },\n    \"DiscoveredResourceList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiscoveredResourceList\"\n        },\n        {\n          \"description\": \"Returned list of discovered resources\
  \ associated with the given MigrationTask.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-discovered-resources-result-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListDiscoveredResourcesResult
---
