---
description: An object that contains information on which data sources will be configured to be automatically enabled for new members within the organization.
layout: schema
name: OrganizationDataSourceConfigurations
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
schema_file: json-schema/guardduty-organization-data-source-configurations-schema.json
slug: guardduty-organization-data-source-configurations
source_filename: guardduty-organization-data-source-configurations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-data-source-configurations-schema.json\",\n  \"title\": \"OrganizationDataSourceConfigurations\",\n  \"description\": \"An object that contains information on which data sources will be configured to be automatically enabled for new members within the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Logs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationS3LogsConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Logs\"\n          },\n          \"description\": \"Describes whether S3 data event logs are enabled for new members of the organization.\"\n        }\n      ]\n    },\n    \"Kubernetes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationKubernetesConfiguration\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"kubernetes\"\n          },\n          \"description\": \"Describes the configuration of Kubernetes data sources for new members of the organization.\"\n        }\n      ]\n    },\n    \"MalwareProtection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationMalwareProtectionConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"malwareProtection\"\n          },\n          \"description\": \"Describes the configuration of Malware Protection for new members of the organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-data-source-configurations-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationDataSourceConfigurations
---
