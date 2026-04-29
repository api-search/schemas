---
description: ListOrganizationAdminAccountsResponse schema from Amazon GuardDuty API
layout: schema
name: ListOrganizationAdminAccountsResponse
properties_list:
- description: ''
  name: AdminAccounts
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-list-organization-admin-accounts-response-schema.json
slug: guardduty-list-organization-admin-accounts-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-organization-admin-accounts-response-schema.json\",\n  \"title\": \"ListOrganizationAdminAccountsResponse\",\n  \"description\": \"ListOrganizationAdminAccountsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdminAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdminAccounts\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adminAccounts\"\n          },\n          \"description\": \"A list of accounts configured as GuardDuty delegated administrators.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n\
  \          \"description\": \"The pagination parameter to be used on the next list operation to retrieve more items.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-organization-admin-accounts-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ListOrganizationAdminAccountsResponse
---
