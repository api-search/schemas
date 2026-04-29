---
description: A list of additional configurations which will be configured for the organization.
layout: schema
name: OrganizationAdditionalConfiguration
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: AutoEnable
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-additional-configuration-schema.json
slug: guardduty-organization-additional-configuration
source_filename: guardduty-organization-additional-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-additional-configuration-schema.json\",\n  \"title\": \"OrganizationAdditionalConfiguration\",\n  \"description\": \"A list of additional configurations which will be configured for the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeatureAdditionalConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the additional configuration that will be configured for the organization.\"\n        }\n      ]\n    },\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeatureStatus\"\n        },\n        {\n          \"xml\": {\n          \
  \  \"name\": \"autoEnable\"\n          },\n          \"description\": \"The status of the additional configuration that will be configured for the organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-additional-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationAdditionalConfiguration
---
