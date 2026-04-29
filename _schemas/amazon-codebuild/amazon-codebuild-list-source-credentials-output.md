---
description: ListSourceCredentialsOutput schema from Amazon CodeBuild
layout: schema
name: ListSourceCredentialsOutput
properties_list:
- description: ''
  name: sourceCredentialsInfos
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-source-credentials-output-schema.json
slug: amazon-codebuild-list-source-credentials-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-source-credentials-output-schema.json\",\n  \"title\": \"ListSourceCredentialsOutput\",\n  \"description\": \"ListSourceCredentialsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceCredentialsInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceCredentialsInfos\"\n        },\n        {\n          \"description\": \" A list of <code>SourceCredentialsInfo</code> objects. Each <code>SourceCredentialsInfo</code> object includes the authentication type, token ARN, and type of source provider for one set of credentials. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-source-credentials-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListSourceCredentialsOutput
---
