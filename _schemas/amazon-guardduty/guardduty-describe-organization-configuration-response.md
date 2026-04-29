---
description: DescribeOrganizationConfigurationResponse schema from Amazon GuardDuty API
layout: schema
name: DescribeOrganizationConfigurationResponse
properties_list:
- description: ''
  name: AutoEnable
  type: object
- description: ''
  name: MemberAccountLimitReached
  type: object
- description: ''
  name: DataSources
  type: object
- description: ''
  name: Features
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: AutoEnableOrganizationMembers
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-describe-organization-configuration-response-schema.json
slug: guardduty-describe-organization-configuration-response
source_filename: guardduty-describe-organization-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-describe-organization-configuration-response-schema.json\",\n  \"title\": \"DescribeOrganizationConfigurationResponse\",\n  \"description\": \"DescribeOrganizationConfigurationResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoEnable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"autoEnable\"\n          },\n          \"description\": \"<p>Indicates whether GuardDuty is automatically enabled for accounts added to the organization.</p> <p>Even though this is still supported, we recommend using <code>AutoEnableOrganizationMembers</code> to achieve the similar results.</p>This field is deprecated, use\
  \ AutoEnableOrganizationMembers instead\"\n        }\n      ]\n    },\n    \"MemberAccountLimitReached\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"memberAccountLimitReached\"\n          },\n          \"description\": \"Indicates whether the maximum number of allowed member accounts are already associated with the delegated administrator account for your organization.\"\n        }\n      ]\n    },\n    \"DataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationDataSourceConfigurationsResult\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"dataSources\"\n          },\n          \"description\": \"Describes which data sources are enabled automatically for member accounts.This parameter is deprecated, use Features instead\"\n        }\n      ]\n    },\n    \"Features\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationFeaturesConfigurationsResults\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"features\"\n          },\n          \"description\": \"A list of features that are configured for this organization.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The pagination parameter to be used on the next list operation to retrieve more items.\"\n        }\n      ]\n    },\n    \"AutoEnableOrganizationMembers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoEnableMembers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"autoEnableOrganizationMembers\"\n          },\n          \"description\": \"<p>Indicates the auto-enablement\
  \ configuration of GuardDuty for the member accounts in the organization.</p> <ul> <li> <p> <code>NEW</code>: Indicates that when a new account joins the organization, they will have GuardDuty enabled automatically. </p> </li> <li> <p> <code>ALL</code>: Indicates that all accounts in the Amazon Web Services Organization have GuardDuty enabled automatically. This includes <code>NEW</code> accounts that join the organization and accounts that may have been suspended or removed from the organization in GuardDuty.</p> </li> <li> <p> <code>NONE</code>: Indicates that GuardDuty will not be automatically enabled for any accounts in the organization. GuardDuty must be managed for each account individually by the administrator.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MemberAccountLimitReached\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-describe-organization-configuration-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DescribeOrganizationConfigurationResponse
---
