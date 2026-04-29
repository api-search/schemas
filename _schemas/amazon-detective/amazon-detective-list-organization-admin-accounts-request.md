---
description: Request to list organization admin accounts
layout: schema
name: ListOrganizationAdminAccountsRequest
properties_list:
- description: The pagination token for the next page of results.
  name: NextToken
  type: string
- description: The maximum number of results to return.
  name: MaxResults
  type: integer
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-list-organization-admin-accounts-request-schema.json
slug: amazon-detective-list-organization-admin-accounts-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-organization-admin-accounts-request-schema.json\",\n  \"title\": \"ListOrganizationAdminAccountsRequest\",\n  \"description\": \"Request to list organization admin accounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The pagination token for the next page of results.\",\n      \"example\": \"abc123token\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results to return.\",\n      \"example\": 100\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-list-organization-admin-accounts-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: ListOrganizationAdminAccountsRequest
---
