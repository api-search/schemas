---
description: UpdateDetectorRequest schema from Amazon GuardDuty API
layout: schema
name: UpdateDetectorRequest
properties_list:
- description: ''
  name: Enable
  type: object
- description: ''
  name: FindingPublishingFrequency
  type: object
- description: ''
  name: DataSources
  type: object
- description: ''
  name: Features
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-update-detector-request-schema.json
slug: guardduty-update-detector-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-detector-request-schema.json\",\n  \"title\": \"UpdateDetectorRequest\",\n  \"description\": \"UpdateDetectorRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enable\"\n          },\n          \"description\": \"Specifies whether the detector is enabled or not enabled.\"\n        }\n      ]\n    },\n    \"FindingPublishingFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingPublishingFrequency\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"findingPublishingFrequency\"\n          },\n          \"description\"\
  : \"An enum value that specifies how frequently findings are exported, such as to CloudWatch Events.\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceConfigurations\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n          },\n          \"description\": \"<p>Describes which data sources will be updated.</p> <p>There might be regional differences because some data sources might not be available in all the Amazon Web Services Regions where GuardDuty is presently supported. For more information, see <a href=\\\"https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_regions.html\\\">Regions and endpoints</a>.</p>This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Features\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectorFeatureConfigurations\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"Provides the features that will be updated for the detector.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-detector-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UpdateDetectorRequest
---
