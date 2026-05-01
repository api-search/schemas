---
description: Information about the resource of the GuardDuty account.
layout: schema
name: CoverageResource
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: DetectorId
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: ResourceDetails
  type: object
- description: ''
  name: CoverageStatus
  type: object
- description: ''
  name: Issue
  type: object
- description: ''
  name: UpdatedAt
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-coverage-resource-schema.json
slug: guardduty-coverage-resource
source_filename: guardduty-coverage-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-resource-schema.json\",\n  \"title\": \"CoverageResource\",\n  \"description\": \"Information about the resource of the GuardDuty account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceId\"\n          },\n          \"description\": \"The unique ID of the resource.\"\n        }\n      ]\n    },\n    \"DetectorId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"detectorId\"\n          },\n          \"description\": \"The unique ID of the GuardDuty detector associated with the resource.\"\n\
  \        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The unique ID of the Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"ResourceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageResourceDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceDetails\"\n          },\n          \"description\": \"Information about the resource for which the coverage statistics are retrieved.\"\n        }\n      ]\n    },\n    \"CoverageStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"coverageStatus\"\n          },\n          \"description\": \"Represents the status of the EKS cluster\
  \ coverage.\"\n        }\n      ]\n    },\n    \"Issue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"issue\"\n          },\n          \"description\": \"Represents the reason why a coverage status was <code>UNHEALTHY</code> for the EKS cluster.\"\n        }\n      ]\n    },\n    \"UpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"updatedAt\"\n          },\n          \"description\": \"The timestamp at which the coverage details for the resource were last updated. This is in UTC format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-coverage-resource-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CoverageResource
---
