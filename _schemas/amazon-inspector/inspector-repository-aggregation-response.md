---
description: A response that contains details on the results of a finding aggregation by repository.
layout: schema
name: RepositoryAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: affectedImages
  type: object
- description: ''
  name: repository
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-repository-aggregation-response-schema.json
slug: inspector-repository-aggregation-response
source_filename: inspector-repository-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-repository-aggregation-response-schema.json\",\n  \"title\": \"RepositoryAggregationResponse\",\n  \"description\": \"A response that contains details on the results of a finding aggregation by repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account associated with the findings.\"\n        }\n      ]\n    },\n    \"affectedImages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of container images impacted by the findings.\"\n        }\n      ]\n    },\n    \"repository\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the repository associated with the findings.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"An object that represent the count of matched findings per severity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"repository\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-repository-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: RepositoryAggregationResponse
---
