---
description: Snowflake account object.
layout: schema
name: ManagedAccount
properties_list:
- description: Cloud in which the managed account is located. For reader accounts, this is always the same as the cloud for the provider account.
  name: cloud
  type: string
- description: Region in which the managed account is located. For reader accounts, this is always the same as the region for the provider account.
  name: region
  type: string
- description: Legacy identifier for the account.
  name: locator
  type: string
- description: Date and time the account was created.
  name: created_on
  type: string
- description: Account URL that is used to connect to the account, in the account name format. The account identifier in this format follows the pattern <orgname>-<account_name>.
  name: url
  type: string
- description: Account URL that is used to connect to the account, in the legacy account locator format.
  name: account_locator_url
  type: string
- description: Optional comment in which to store information related to the account.
  name: comment
  type: string
- description: Name of the account administrator.
  name: admin_name
  type: string
- description: Password for the account administrator.
  name: admin_password
  type: string
- description: Type of the account.
  name: account_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/managed-account-managed-account-schema.json
slug: managed-account-managed-account
source_filename: managed-account-managed-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManagedAccount\",\n  \"type\": \"object\",\n  \"description\": \"Snowflake account object.\",\n  \"properties\": {\n    \"cloud\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud in which the managed account is located. For reader accounts, this is always the same as the cloud for the provider account.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Region in which the managed account is located. For reader accounts, this is always the same as the region for the provider account.\"\n    },\n    \"locator\": {\n      \"type\": \"string\",\n      \"description\": \"Legacy identifier for the account.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the account was created.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Account URL that is used to connect to the\
  \ account, in the account name format. The account identifier in this format follows the pattern <orgname>-<account_name>.\"\n    },\n    \"account_locator_url\": {\n      \"type\": \"string\",\n      \"description\": \"Account URL that is used to connect to the account, in the legacy account locator format.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment in which to store information related to the account.\"\n    },\n    \"admin_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the account administrator.\"\n    },\n    \"admin_password\": {\n      \"type\": \"string\",\n      \"description\": \"Password for the account administrator.\"\n    },\n    \"account_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the account.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/managed-account-managed-account-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ManagedAccount
---
