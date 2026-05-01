---
description: ListCoverageRequest schema from Amazon GuardDuty API
layout: schema
name: ListCoverageRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: FilterCriteria
  type: object
- description: ''
  name: SortCriteria
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-list-coverage-request-schema.json
slug: guardduty-list-coverage-request
source_filename: guardduty-list-coverage-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-coverage-request-schema.json\",\n  \"title\": \"ListCoverageRequest\",\n  \"description\": \"ListCoverageRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"A token to use for paginating results that are returned in the response. Set the value of this parameter to null for the first request to a list action. For subsequent calls, use the NextToken value returned from the previous request to continue listing results after the first page.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxResults\"\n          },\n          \"description\": \"The maximum number of results to return in the response.\"\n        }\n      ]\n    },\n    \"FilterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageFilterCriteria\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"filterCriteria\"\n          },\n          \"description\": \"Represents the criteria used to filter the coverage details.\"\n        }\n      ]\n    },\n    \"SortCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageSortCriteria\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sortCriteria\"\n          },\n          \"description\": \"Represents the criteria used to sort the coverage details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-coverage-request-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ListCoverageRequest
---
