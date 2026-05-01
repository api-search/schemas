---
description: CreateDetectorRequest schema from Amazon GuardDuty API
layout: schema
name: CreateDetectorRequest
properties_list:
- description: ''
  name: Enable
  type: object
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: FindingPublishingFrequency
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
schema_file: json-schema/guardduty-create-detector-request-schema.json
slug: guardduty-create-detector-request
source_filename: guardduty-create-detector-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-detector-request-schema.json\",\n  \"title\": \"CreateDetectorRequest\",\n  \"description\": \"CreateDetectorRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enable\"\n          },\n          \"description\": \"A Boolean value that specifies whether the detector is to be enabled.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientToken\"\n          },\n          \"description\": \"The idempotency token for the\
  \ create request.\"\n        }\n      ]\n    },\n    \"FindingPublishingFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingPublishingFrequency\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingPublishingFrequency\"\n          },\n          \"description\": \"A value that specifies how frequently updated findings are exported.\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceConfigurations\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n          },\n          \"description\": \"<p>Describes which data sources will be enabled for the detector.</p> <p>There might be regional differences because some data sources might not be available in all the Amazon Web Services Regions where GuardDuty is presently supported. For more information, see <a href=\\\"https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_regions.html\\\
  \">Regions and endpoints</a>.</p>This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"The tags to be added to a new detector resource.\"\n        }\n      ]\n    },\n    \"Features\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorFeatureConfigurations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"A list of features that will be configured for the detector.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Enable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-detector-request-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CreateDetectorRequest
---
