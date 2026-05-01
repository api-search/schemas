---
description: A list of additional configuration which will be configured for the organization.
layout: schema
name: OrganizationAdditionalConfigurationResult
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: AutoEnable
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-additional-configuration-result-schema.json
slug: guardduty-organization-additional-configuration-result
source_filename: guardduty-organization-additional-configuration-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-additional-configuration-result-schema.json\",\n  \"title\": \"OrganizationAdditionalConfigurationResult\",\n  \"description\": \"A list of additional configuration which will be configured for the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeatureAdditionalConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the additional configuration that is configured for the member accounts within the organization.\"\n        }\n      ]\n    },\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeatureStatus\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\": \"<p>Describes how The status of the additional configuration that are configured for the member accounts within the organization.</p> <p>If you set <code>AutoEnable</code> to <code>NEW</code>, a feature will be configured for only the new accounts when they join the organization.</p> <p>If you set <code>AutoEnable</code> to <code>NONE</code>, no feature will be configured for the accounts when they join the organization.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-additional-configuration-result-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationAdditionalConfigurationResult
---
