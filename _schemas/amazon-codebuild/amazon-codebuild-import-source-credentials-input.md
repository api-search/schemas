---
description: ImportSourceCredentialsInput schema from Amazon CodeBuild
layout: schema
name: ImportSourceCredentialsInput
properties_list:
- description: ''
  name: username
  type: object
- description: ''
  name: token
  type: object
- description: ''
  name: serverType
  type: object
- description: ''
  name: authType
  type: object
- description: ''
  name: shouldOverwrite
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-import-source-credentials-input-schema.json
slug: amazon-codebuild-import-source-credentials-input
source_filename: amazon-codebuild-import-source-credentials-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-import-source-credentials-input-schema.json\",\n  \"title\": \"ImportSourceCredentialsInput\",\n  \"description\": \"ImportSourceCredentialsInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The Bitbucket username when the <code>authType</code> is BASIC_AUTH. This parameter is not valid for other types of source providers or connections. \"\n        }\n      ]\n    },\n    \"token\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveNonEmptyString\"\n        },\n        {\n          \"description\": \" For GitHub or GitHub Enterprise, this is the personal\
  \ access token. For Bitbucket, this is the app password. \"\n        }\n      ]\n    },\n    \"serverType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerType\"\n        },\n        {\n          \"description\": \" The source provider used for this project. \"\n        }\n      ]\n    },\n    \"authType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthType\"\n        },\n        {\n          \"description\": \" The type of authentication used to connect to a GitHub, GitHub Enterprise, or Bitbucket repository. An OAUTH connection is not supported by the API and must be created using the CodeBuild console. \"\n        }\n      ]\n    },\n    \"shouldOverwrite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" Set to <code>false</code> to prevent overwriting the repository source credentials. Set to <code>true</code> to\
  \ overwrite the repository source credentials. The default value is <code>true</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"token\",\n    \"serverType\",\n    \"authType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-import-source-credentials-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ImportSourceCredentialsInput
---
