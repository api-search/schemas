---
description: <p>Information about the authorization settings for CodeBuild to access the source code to be built.</p> <p>This information is for the CodeBuild console's use only. Your code should not get or set this information directly.</p>
layout: schema
name: SourceAuth
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: resource
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-source-auth-schema.json
slug: amazon-codebuild-source-auth
source_filename: amazon-codebuild-source-auth-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-source-auth-schema.json\",\n  \"title\": \"SourceAuth\",\n  \"description\": \"<p>Information about the authorization settings for CodeBuild to access the source code to be built.</p> <p>This information is for the CodeBuild console's use only. Your code should not get or set this information directly.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceAuthType\"\n        },\n        {\n          \"description\": \"<note> <p> This data type is deprecated and is no longer accurate or used. </p> </note> <p>The authorization type to use. The only valid value is <code>OAUTH</code>, which represents the OAuth authorization type.</p>\"\n        }\n      ]\n    },\n    \"resource\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The resource value that applies to the specified authorization type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-source-auth-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: SourceAuth
---
