---
description: Request to enable an organization admin account for Detective
layout: schema
name: EnableOrganizationAdminAccountRequest
properties_list:
- description: The AWS account identifier of the account to designate as the Detective administrator account for the organization.
  name: AccountId
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-enable-organization-admin-account-request-schema.json
slug: amazon-detective-enable-organization-admin-account-request
source_filename: amazon-detective-enable-organization-admin-account-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-enable-organization-admin-account-request-schema.json\",\n  \"title\": \"EnableOrganizationAdminAccountRequest\",\n  \"description\": \"Request to enable an organization admin account for Detective\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account identifier of the account to designate as the Detective administrator account for the organization.\",\n      \"example\": \"123456789012\"\n    }\n  },\n  \"required\": [\n    \"AccountId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-enable-organization-admin-account-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: EnableOrganizationAdminAccountRequest
---
