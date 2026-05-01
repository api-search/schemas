---
description: <p>Contains information about an exported environment variable. </p> <p>Exported environment variables are used in conjunction with CodePipeline to export environment variables from the current build stage to subsequent stages in the pipeline. For more information, see <a href="https://docs.aws.amazon.com/codepipeline/latest/userguide/actions-variables.html">Working with variables</a> in the <i>CodePipeline User Guide</i>.</p> <note> <p> During a build, the value of a variable is available starting with the <code>install</code> phase. It can be updated between the start of the <code>install</code> phase and the end of the <code>post_build</code> phase. After the <code>post_build</code> phase ends, the value of exported variables cannot change.</p> </note>
layout: schema
name: ExportedEnvironmentVariable
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-exported-environment-variable-schema.json
slug: amazon-codebuild-exported-environment-variable
source_filename: amazon-codebuild-exported-environment-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-exported-environment-variable-schema.json\",\n  \"title\": \"ExportedEnvironmentVariable\",\n  \"description\": \"<p>Contains information about an exported environment variable. </p> <p>Exported environment variables are used in conjunction with CodePipeline to export environment variables from the current build stage to subsequent stages in the pipeline. For more information, see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/actions-variables.html\\\">Working with variables</a> in the <i>CodePipeline User Guide</i>.</p> <note> <p> During a build, the value of a variable is available starting with the <code>install</code> phase. It can be updated between the start of the <code>install</code> phase and the end of the <code>post_build</code> phase. After the <code>post_build</code>\
  \ phase ends, the value of exported variables cannot change.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the exported environment variable.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The value assigned to the exported environment variable.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-exported-environment-variable-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ExportedEnvironmentVariable
---
