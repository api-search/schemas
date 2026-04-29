---
description: ListServiceInstancesInput schema from Amazon Proton API
layout: schema
name: ListServiceInstancesInput
properties_list:
- description: ''
  name: filters
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: serviceName
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-service-instances-input-schema.json
slug: amazon-proton-list-service-instances-input
source_filename: amazon-proton-list-service-instances-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-instances-input-schema.json\",\n  \"title\": \"ListServiceInstancesInput\",\n  \"description\": \"ListServiceInstancesInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListServiceInstancesFilterList\"\n        },\n        {\n          \"description\": \"An array of filtering criteria that scope down the result list. By default, all service instances in the Amazon Web Services account are returned.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxPageResults\"\n        },\n        {\n          \"description\": \"The maximum number of service instances to list.\"\n      \
  \  }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next service in the array of service instances, after the list of service instances that was previously requested.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service that the service instance belongs to.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListServiceInstancesSortBy\"\n        },\n        {\n          \"description\": \"<p>The field that the result list is sorted by.</p> <p>When you choose to sort by <code>serviceName</code>, service instances within each service are sorted by service instance name.</p> <p>Default:\
  \ <code>serviceName</code> </p>\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"<p>Result list sort order.</p> <p>Default: <code>ASCENDING</code> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-instances-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListServiceInstancesInput
---
