---
description: An object that contains information on which data sources are automatically enabled for new members within the organization.
layout: schema
name: OrganizationDataSourceConfigurationsResult
properties_list:
- description: ''
  name: S3Logs
  type: object
- description: ''
  name: Kubernetes
  type: object
- description: ''
  name: MalwareProtection
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-data-source-configurations-result-schema.json
slug: guardduty-organization-data-source-configurations-result
source_filename: guardduty-organization-data-source-configurations-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-data-source-configurations-result-schema.json\",\n  \"title\": \"OrganizationDataSourceConfigurationsResult\",\n  \"description\": \"An object that contains information on which data sources are automatically enabled for new members within the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationS3LogsConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Logs\"\n          },\n          \"description\": \"Describes whether S3 data event logs are enabled as a data source.\"\n        }\n      ]\n    },\n    \"Kubernetes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationKubernetesConfigurationResult\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"kubernetes\"\n          },\n          \"description\": \"Describes the configuration of Kubernetes data sources.\"\n        }\n      ]\n    },\n    \"MalwareProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationMalwareProtectionConfigurationResult\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"malwareProtection\"\n          },\n          \"description\": \"Describes the configuration of Malware Protection data source for an organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Logs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-data-source-configurations-result-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationDataSourceConfigurationsResult
---
