---
description: ImportSourceCredentialsOutput schema from Amazon CodeBuild
layout: schema
name: ImportSourceCredentialsOutput
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-import-source-credentials-output-schema.json
slug: amazon-codebuild-import-source-credentials-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-import-source-credentials-output-schema.json\",\n  \"title\": \"ImportSourceCredentialsOutput\",\n  \"description\": \"ImportSourceCredentialsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the token. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-import-source-credentials-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ImportSourceCredentialsOutput
---
