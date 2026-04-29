---
description: UpdateAutomatedDiscoveryConfigurationRequest schema from Amazon Macie API
layout: schema
name: UpdateAutomatedDiscoveryConfigurationRequest
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-update-automated-discovery-configuration-request-schema.json
slug: amazon-macie-update-automated-discovery-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-automated-discovery-configuration-request-schema.json\",\n  \"title\": \"UpdateAutomatedDiscoveryConfigurationRequest\",\n  \"description\": \"UpdateAutomatedDiscoveryConfigurationRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomatedDiscoveryStatus\"\n        },\n        {\n          \"description\": \"<p>The new status of automated sensitive data discovery for the account. Valid values are: ENABLED, start or resume automated sensitive data discovery activities for the account; and, DISABLED, stop performing automated sensitive data discovery activities for the account.</p> <p>When you enable automated sensitive data discovery for the first time, Amazon\
  \ Macie uses default configuration settings to determine which data sources to analyze and which managed data identifiers to use. To change these settings, use the UpdateClassificationScope and UpdateSensitivityInspectionTemplate operations, respectively. If you change the settings and subsequently disable the configuration, Amazon Macie retains your changes.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-update-automated-discovery-configuration-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UpdateAutomatedDiscoveryConfigurationRequest
---
