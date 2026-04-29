---
description: ListServiceVersionsRequest schema from Amazon Snow Family API
layout: schema
name: ListServiceVersionsRequest
properties_list:
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: DependentServices
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-service-versions-request-schema.json
slug: amazon-snow-family-list-service-versions-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-service-versions-request-schema.json\",\n  \"title\": \"ListServiceVersionsRequest\",\n  \"description\": \"ListServiceVersionsRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceName\"\n        },\n        {\n          \"description\": \"The name of the service for which you're requesting supported versions.\"\n        }\n      ]\n    },\n    \"DependentServices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DependentServiceList\"\n        },\n        {\n          \"description\": \"A list of names and versions of dependant services of the requested service.\"\n        }\n      ]\n    },\n    \"MaxResults\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListLimit\"\n        },\n        {\n          \"description\": \"The maximum number of <code>ListServiceVersions</code> objects to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Because HTTP requests are stateless, this is the starting point for the next list of returned <code>ListServiceVersionsRequest</code> versions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ServiceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-service-versions-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListServiceVersionsRequest
---
