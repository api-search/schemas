---
description: Contains information about the debug session for a build. For more information, see <a href="https://docs.aws.amazon.com/codebuild/latest/userguide/session-manager.html">Viewing a running build in Session Manager</a>.
layout: schema
name: DebugSession
properties_list:
- description: ''
  name: sessionEnabled
  type: object
- description: ''
  name: sessionTarget
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-debug-session-schema.json
slug: amazon-codebuild-debug-session
source_filename: amazon-codebuild-debug-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-debug-session-schema.json\",\n  \"title\": \"DebugSession\",\n  \"description\": \"Contains information about the debug session for a build. For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/session-manager.html\\\">Viewing a running build in Session Manager</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \"Specifies if session debugging is enabled for this build.\"\n        }\n      ]\n    },\n    \"sessionTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Contains\
  \ the identifier of the Session Manager session used for the build. To work with the paused build, you open this session to examine, control, and resume the build.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-debug-session-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: DebugSession
---
