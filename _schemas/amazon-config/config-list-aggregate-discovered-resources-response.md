---
description: ListAggregateDiscoveredResourcesResponse schema
layout: schema
name: ListAggregateDiscoveredResourcesResponse
properties_list:
- description: ''
  name: ResourceIdentifiers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-list-aggregate-discovered-resources-response-schema.json
slug: config-list-aggregate-discovered-resources-response
source_filename: config-list-aggregate-discovered-resources-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-aggregate-discovered-resources-response-schema.json\",\n  \"title\": \"ListAggregateDiscoveredResourcesResponse\",\n  \"description\": \"ListAggregateDiscoveredResourcesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceIdentifiers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiscoveredResourceIdentifierList\"\n        },\n        {\n          \"description\": \"Returns a list of <code>ResourceIdentifiers</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated\
  \ response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-aggregate-discovered-resources-response-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ListAggregateDiscoveredResourcesResponse
---
