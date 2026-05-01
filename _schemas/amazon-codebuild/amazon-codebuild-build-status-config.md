---
description: Contains information that defines how the CodeBuild build project reports the build status to the source provider.
layout: schema
name: BuildStatusConfig
properties_list:
- description: ''
  name: context
  type: object
- description: ''
  name: targetUrl
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-status-config-schema.json
slug: amazon-codebuild-build-status-config
source_filename: amazon-codebuild-build-status-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-status-config-schema.json\",\n  \"title\": \"BuildStatusConfig\",\n  \"description\": \"Contains information that defines how the CodeBuild build project reports the build status to the source provider. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"context\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Specifies the context of the build status CodeBuild sends to the source provider. The usage of this parameter depends on the source provider.</p> <dl> <dt>Bitbucket</dt> <dd> <p>This parameter is used for the <code>name</code> parameter in the Bitbucket commit status. For more information, see <a href=\\\"https://developer.atlassian.com/bitbucket/api/2/reference/resource/repositories/%7Bworkspace%7D/%7Brepo_slug%7D/commit/%7Bnode%7D/statuses/build\\\
  \">build</a> in the Bitbucket API documentation.</p> </dd> <dt>GitHub/GitHub Enterprise Server</dt> <dd> <p>This parameter is used for the <code>context</code> parameter in the GitHub commit status. For more information, see <a href=\\\"https://developer.github.com/v3/repos/statuses/#create-a-commit-status\\\">Create a commit status</a> in the GitHub developer guide.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"targetUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Specifies the target url of the build status CodeBuild sends to the source provider. The usage of this parameter depends on the source provider.</p> <dl> <dt>Bitbucket</dt> <dd> <p>This parameter is used for the <code>url</code> parameter in the Bitbucket commit status. For more information, see <a href=\\\"https://developer.atlassian.com/bitbucket/api/2/reference/resource/repositories/%7Bworkspace%7D/%7Brepo_slug%7D/commit/%7Bnode%7D/statuses/build\\\
  \">build</a> in the Bitbucket API documentation.</p> </dd> <dt>GitHub/GitHub Enterprise Server</dt> <dd> <p>This parameter is used for the <code>target_url</code> parameter in the GitHub commit status. For more information, see <a href=\\\"https://developer.github.com/v3/repos/statuses/#create-a-commit-status\\\">Create a commit status</a> in the GitHub developer guide.</p> </dd> </dl>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-status-config-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildStatusConfig
---
