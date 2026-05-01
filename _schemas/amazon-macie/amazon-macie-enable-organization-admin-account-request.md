---
description: EnableOrganizationAdminAccountRequest schema from Amazon Macie API
layout: schema
name: EnableOrganizationAdminAccountRequest
properties_list:
- description: ''
  name: adminAccountId
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-enable-organization-admin-account-request-schema.json
slug: amazon-macie-enable-organization-admin-account-request
source_filename: amazon-macie-enable-organization-admin-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-enable-organization-admin-account-request-schema.json\",\n  \"title\": \"EnableOrganizationAdminAccountRequest\",\n  \"description\": \"EnableOrganizationAdminAccountRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adminAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account to designate as the delegated Amazon Macie administrator account for the organization.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive token that you provide to ensure\
  \ the idempotency of the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"adminAccountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-enable-organization-admin-account-request-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: EnableOrganizationAdminAccountRequest
---
