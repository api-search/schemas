---
description: AllowedAccounts schema from Amazon CodePipeline
layout: schema
name: AllowedAccounts
properties_list: []
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-allowed-accounts-schema.json
slug: amazon-codepipeline-allowed-accounts
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-allowed-accounts-schema.json\",\n  \"title\": \"AllowedAccounts\",\n  \"description\": \"AllowedAccounts schema from Amazon CodePipeline\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/AllowedAccount\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 1000\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-allowed-accounts-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: AllowedAccounts
---
