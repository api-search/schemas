---
description: GetAutomatedDiscoveryConfigurationResponse schema from Amazon Macie API
layout: schema
name: GetAutomatedDiscoveryConfigurationResponse
properties_list:
- description: ''
  name: classificationScopeId
  type: object
- description: ''
  name: disabledAt
  type: object
- description: ''
  name: firstEnabledAt
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: sensitivityInspectionTemplateId
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-get-automated-discovery-configuration-response-schema.json
slug: amazon-macie-get-automated-discovery-configuration-response
source_filename: amazon-macie-get-automated-discovery-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-automated-discovery-configuration-response-schema.json\",\n  \"title\": \"GetAutomatedDiscoveryConfigurationResponse\",\n  \"description\": \"GetAutomatedDiscoveryConfigurationResponse schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"classificationScopeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationScopeId\"\n        },\n        {\n          \"description\": \"The unique identifier for the classification scope that's used when performing automated sensitive data discovery for the account. The classification scope specifies S3 buckets to exclude from automated sensitive data discovery.\"\n        }\n      ]\n    },\n    \"disabledAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when automated sensitive data discovery was most recently disabled for the account. This value is null if automated sensitive data discovery wasn't enabled and subsequently disabled for the account.\"\n        }\n      ]\n    },\n    \"firstEnabledAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when automated sensitive data discovery was initially enabled for the account. This value is null if automated sensitive data discovery has never been enabled for the account.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when automated\
  \ sensitive data discovery was most recently enabled or disabled for the account.\"\n        }\n      ]\n    },\n    \"sensitivityInspectionTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityInspectionTemplateId\"\n        },\n        {\n          \"description\": \"The unique identifier for the sensitivity inspection template that's used when performing automated sensitive data discovery for the account. The template specifies which allow lists, custom data identifiers, and managed data identifiers to use when analyzing data.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomatedDiscoveryStatus\"\n        },\n        {\n          \"description\": \"The current status of the automated sensitive data discovery configuration for the account. Possible values are: ENABLED, use the specified settings to perform automated sensitive data discovery activities for the\
  \ account; and, DISABLED, don't perform automated sensitive data discovery activities for the account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-get-automated-discovery-configuration-response-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: GetAutomatedDiscoveryConfigurationResponse
---
