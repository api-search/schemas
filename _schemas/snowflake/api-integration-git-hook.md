---
description: ''
layout: schema
name: GitHook
properties_list:
- description: Whether to allow any Snowflake secret when accessing the Git repository. This setting is ignored if allowed_authentication_secrets is present.
  name: allow_any_secret
  type: boolean
- description: A comma-separated list of fully-qualified Snowflake secret names that UDF or procedure handler code can use when accessing the Git repository.
  name: allowed_authentication_secrets
  type: array
- description: A comma-separated list of Snowflake security integration names that UDF or procedure handler code can use when accessing the Git repository. If empty, allow no integrations.
  name: allowed_api_authentication_integrations
  type: array
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/api-integration-git-hook-schema.json
slug: api-integration-git-hook
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GitHook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allow_any_secret\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to allow any Snowflake secret when accessing the Git repository. This setting is ignored if allowed_authentication_secrets is present.\"\n    },\n    \"allowed_authentication_secrets\": {\n      \"type\": \"array\",\n      \"description\": \"A comma-separated list of fully-qualified Snowflake secret names that UDF or procedure handler code can use when accessing the Git repository.\"\n    },\n    \"allowed_api_authentication_integrations\": {\n      \"type\": \"array\",\n      \"description\": \"A comma-separated list of Snowflake security integration names that UDF or procedure handler code can use when accessing the Git repository. If empty, allow no integrations.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/api-integration-git-hook-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: GitHook
---
