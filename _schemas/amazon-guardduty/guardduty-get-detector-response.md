---
description: GetDetectorResponse schema from Amazon GuardDuty API
layout: schema
name: GetDetectorResponse
properties_list:
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: FindingPublishingFrequency
  type: object
- description: ''
  name: ServiceRole
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: UpdatedAt
  type: object
- description: ''
  name: DataSources
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Features
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-get-detector-response-schema.json
slug: guardduty-get-detector-response
source_filename: guardduty-get-detector-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-detector-response-schema.json\",\n  \"title\": \"GetDetectorResponse\",\n  \"description\": \"GetDetectorResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The timestamp of when the detector was created.\"\n        }\n      ]\n    },\n    \"FindingPublishingFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingPublishingFrequency\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingPublishingFrequency\"\n          },\n          \"description\": \"The publishing\
  \ frequency of the finding.\"\n        }\n      ]\n    },\n    \"ServiceRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceRole\"\n          },\n          \"description\": \"The GuardDuty service role.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The detector status.\"\n        }\n      ]\n    },\n    \"UpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"updatedAt\"\n          },\n          \"description\": \"The last-updated timestamp for the detector.\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/DataSourceConfigurationsResult\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n          },\n          \"description\": \"Describes which data sources are enabled for the detector.This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags of the detector resource.\"\n        }\n      ]\n    },\n    \"Features\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorFeatureConfigurationsResults\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"Describes the features that have been enabled for the detector.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"ServiceRole\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-get-detector-response-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: GetDetectorResponse
---
