---
description: Response from listing organization admin accounts
layout: schema
name: ListOrganizationAdminAccountsResponse
properties_list:
- description: The list of delegated administrator accounts.
  name: Administrators
  type: array
- description: If there are more accounts remaining in the results, then this is the pagination token.
  name: NextToken
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-organization-admin-accounts-response-schema.json
slug: amazon-detective-list-organization-admin-accounts-response
source_filename: amazon-detective-list-organization-admin-accounts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-organization-admin-accounts-response-schema.json\",\n  \"title\": \"ListOrganizationAdminAccountsResponse\",\n  \"description\": \"Response from listing organization admin accounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Administrators\": {\n      \"type\": \"array\",\n      \"description\": \"The list of delegated administrator accounts.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Administrator\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"If there are more accounts remaining in the results, then this is the pagination token.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-organization-admin-accounts-response-schema.json
tags:
- Forensics
- Investigation
- Security
title: ListOrganizationAdminAccountsResponse
---
