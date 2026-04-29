---
description: <p/>
layout: schema
name: ListDiscoveredResourcesRequest
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resourceIds
  type: object
- description: ''
  name: resourceName
  type: object
- description: ''
  name: limit
  type: object
- description: ''
  name: includeDeletedResources
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-list-discovered-resources-request-schema.json
slug: config-list-discovered-resources-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-discovered-resources-request-schema.json\",\n  \"title\": \"ListDiscoveredResourcesRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The type of resources that you want Config to list in the response.\"\n        }\n      ]\n    },\n    \"resourceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceIdList\"\n        },\n        {\n          \"description\": \"The IDs of only those resources that you want Config to list in the response. If you do not specify this parameter, Config lists all resources of the specified type that it has discovered. You can list\
  \ a minimum of 1 resourceID and a maximum of 20 resourceIds.\"\n        }\n      ]\n    },\n    \"resourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The custom name of only those resources that you want Config to list in the response. If you do not specify this parameter, Config lists all resources of the specified type that it has discovered.\"\n        }\n      ]\n    },\n    \"limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of resource identifiers returned on each page. The default is 100. You cannot specify a number greater than 100. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"includeDeletedResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n         \
  \ \"description\": \"Specifies whether Config includes deleted resources in the results. By default, deleted resources are not included.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-list-discovered-resources-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ListDiscoveredResourcesRequest
---
