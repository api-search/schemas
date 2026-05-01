---
description: UpdateOrganizationConfigurationRequest schema from Amazon GuardDuty API
layout: schema
name: UpdateOrganizationConfigurationRequest
properties_list:
- description: ''
  name: AutoEnable
  type: object
- description: ''
  name: DataSources
  type: object
- description: ''
  name: Features
  type: object
- description: ''
  name: AutoEnableOrganizationMembers
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-update-organization-configuration-request-schema.json
slug: guardduty-update-organization-configuration-request
source_filename: guardduty-update-organization-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-organization-configuration-request-schema.json\",\n  \"title\": \"UpdateOrganizationConfigurationRequest\",\n  \"description\": \"UpdateOrganizationConfigurationRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\": \"<p>Indicates whether to automatically enable member accounts in the organization.</p> <p>Even though this is still supported, we recommend using <code>AutoEnableOrganizationMembers</code> to achieve the similar results.</p>This field is deprecated, use AutoEnableOrganizationMembers\
  \ instead\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationDataSourceConfigurations\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n          },\n          \"description\": \"Describes which data sources will be updated.This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Features\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationFeaturesConfigurations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"A list of features that will be configured for the organization.\"\n        }\n      ]\n    },\n    \"AutoEnableOrganizationMembers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoEnableMembers\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"autoEnableOrganizationMembers\"\n          },\n          \"description\": \"<p>Indicates the auto-enablement configuration of GuardDuty for the member accounts in the organization. </p> <ul> <li> <p> <code>NEW</code>: Indicates that when a new account joins the organization, they will have GuardDuty enabled automatically. </p> </li> <li> <p> <code>ALL</code>: Indicates that all accounts in the Amazon Web Services Organization have GuardDuty enabled automatically. This includes <code>NEW</code> accounts that join the organization and accounts that may have been suspended or removed from the organization in GuardDuty.</p> </li> <li> <p> <code>NONE</code>: Indicates that GuardDuty will not be automatically enabled for any accounts in the organization. GuardDuty must be managed for each account individually by the administrator.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-update-organization-configuration-request-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: UpdateOrganizationConfigurationRequest
---
