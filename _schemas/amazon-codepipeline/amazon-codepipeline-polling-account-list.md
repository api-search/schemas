---
description: PollingAccountList schema from Amazon CodePipeline
layout: schema
name: PollingAccountList
properties_list: []
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-polling-account-list-schema.json
slug: amazon-codepipeline-polling-account-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-polling-account-list-schema.json\",\n  \"title\": \"PollingAccountList\",\n  \"description\": \"PollingAccountList schema from Amazon CodePipeline\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/AccountId\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 1000\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-polling-account-list-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PollingAccountList
---
