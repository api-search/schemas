---
description: A source identifier and its corresponding version.
layout: schema
name: ProjectSourceVersion
properties_list:
- description: ''
  name: sourceIdentifier
  type: object
- description: ''
  name: sourceVersion
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-source-version-schema.json
slug: amazon-codebuild-project-source-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-source-version-schema.json\",\n  \"title\": \"ProjectSourceVersion\",\n  \"description\": \" A source identifier and its corresponding version. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An identifier for a source in the build project. The identifier can only contain alphanumeric characters and underscores, and must be less than 128 characters in length. \"\n        }\n      ]\n    },\n    \"sourceVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The source version for the corresponding source identifier.\
  \ If specified, must be one of:</p> <ul> <li> <p>For CodeCommit: the commit ID, branch, or Git tag to use.</p> </li> <li> <p>For GitHub: the commit ID, pull request ID, branch name, or tag name that corresponds to the version of the source code you want to build. If a pull request ID is specified, it must use the format <code>pr/pull-request-ID</code> (for example, <code>pr/25</code>). If a branch name is specified, the branch's HEAD commit ID is used. If not specified, the default branch's HEAD commit ID is used.</p> </li> <li> <p>For Bitbucket: the commit ID, branch name, or tag name that corresponds to the version of the source code you want to build. If a branch name is specified, the branch's HEAD commit ID is used. If not specified, the default branch's HEAD commit ID is used.</p> </li> <li> <p>For Amazon S3: the version ID of the object that represents the build input ZIP file to use.</p> </li> </ul> <p> For more information, see <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/sample-source-version.html\\\
  \">Source Version Sample with CodeBuild</a> in the <i>CodeBuild User Guide</i>. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"sourceIdentifier\",\n    \"sourceVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-source-version-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ProjectSourceVersion
---
