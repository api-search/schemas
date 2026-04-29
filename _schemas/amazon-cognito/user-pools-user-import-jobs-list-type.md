---
description: UserImportJobsListType schema from Amazon Cognito API
layout: schema
name: UserImportJobsListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-user-import-jobs-list-type-schema.json
slug: user-pools-user-import-jobs-list-type
source_filename: user-pools-user-import-jobs-list-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-import-jobs-list-type-schema.json\",\n  \"title\": \"UserImportJobsListType\",\n  \"description\": \"UserImportJobsListType schema from Amazon Cognito API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/UserImportJobType\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 50\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-import-jobs-list-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UserImportJobsListType
---
