---
description: A list of features which will be configured for the organization.
layout: schema
name: OrganizationFeatureConfiguration
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: AutoEnable
  type: object
- description: ''
  name: AdditionalConfiguration
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-organization-feature-configuration-schema.json
slug: guardduty-organization-feature-configuration
source_filename: guardduty-organization-feature-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-feature-configuration-schema.json\",\n  \"title\": \"OrganizationFeatureConfiguration\",\n  \"description\": \"A list of features which will be configured for the organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeature\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the feature that will be configured for the organization.\"\n        }\n      ]\n    },\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrgFeatureStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\"\
  : \"The status of the feature that will be configured for the organization.\"\n        }\n      ]\n    },\n    \"AdditionalConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationAdditionalConfigurations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"additionalConfiguration\"\n          },\n          \"description\": \"The additional information that will be configured for the organization.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-organization-feature-configuration-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: OrganizationFeatureConfiguration
---
