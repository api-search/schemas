---
description: DisableOrganizationAdminAccountRequest schema from Amazon GuardDuty API
layout: schema
name: DisableOrganizationAdminAccountRequest
properties_list:
- description: ''
  name: AdminAccountId
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-disable-organization-admin-account-request-schema.json
slug: guardduty-disable-organization-admin-account-request
source_filename: guardduty-disable-organization-admin-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-disable-organization-admin-account-request-schema.json\",\n  \"title\": \"DisableOrganizationAdminAccountRequest\",\n  \"description\": \"DisableOrganizationAdminAccountRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdminAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adminAccountId\"\n          },\n          \"description\": \"The Amazon Web Services Account ID for the organizations account to be disabled as a GuardDuty delegated administrator.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AdminAccountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-disable-organization-admin-account-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DisableOrganizationAdminAccountRequest
---
