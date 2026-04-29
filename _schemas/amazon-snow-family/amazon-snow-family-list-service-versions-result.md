---
description: ListServiceVersionsResult schema from Amazon Snow Family API
layout: schema
name: ListServiceVersionsResult
properties_list:
- description: ''
  name: ServiceVersions
  type: object
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: DependentServices
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-service-versions-result-schema.json
slug: amazon-snow-family-list-service-versions-result
source_filename: amazon-snow-family-list-service-versions-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-service-versions-result-schema.json\",\n  \"title\": \"ListServiceVersionsResult\",\n  \"description\": \"ListServiceVersionsResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceVersionList\"\n        },\n        {\n          \"description\": \"A list of supported versions.\"\n        }\n      ]\n    },\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceName\"\n        },\n        {\n          \"description\": \"The name of the service for which the system provided supported versions.\"\n        }\n      ]\n    },\n    \"DependentServices\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/DependentServiceList\"\n        },\n        {\n          \"description\": \"A list of names and versions of dependant services of the service for which the system provided supported versions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Because HTTP requests are stateless, this is the starting point of the next list of returned <code>ListServiceVersionsResult</code> results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ServiceVersions\",\n    \"ServiceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-service-versions-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListServiceVersionsResult
---
