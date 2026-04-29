---
description: Describes whether S3 data event logs will be automatically enabled for new members of the organization.
layout: schema
name: OrganizationS3LogsConfiguration
properties_list:
- description: ''
  name: AutoEnable
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-s3-logs-configuration-schema.json
slug: guardduty-organization-s3-logs-configuration
source_filename: guardduty-organization-s3-logs-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-s3-logs-configuration-schema.json\",\n  \"title\": \"OrganizationS3LogsConfiguration\",\n  \"description\": \"Describes whether S3 data event logs will be automatically enabled for new members of the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\": \"A value that contains information on whether S3 data event logs will be enabled automatically as a data source for the organization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoEnable\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-s3-logs-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationS3LogsConfiguration
---
