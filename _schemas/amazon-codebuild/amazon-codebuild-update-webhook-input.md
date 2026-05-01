---
description: UpdateWebhookInput schema from Amazon CodeBuild
layout: schema
name: UpdateWebhookInput
properties_list:
- description: ''
  name: projectName
  type: object
- description: ''
  name: branchFilter
  type: object
- description: ''
  name: rotateSecret
  type: object
- description: ''
  name: filterGroups
  type: object
- description: ''
  name: buildType
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-update-webhook-input-schema.json
slug: amazon-codebuild-update-webhook-input
source_filename: amazon-codebuild-update-webhook-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-webhook-input-schema.json\",\n  \"title\": \"UpdateWebhookInput\",\n  \"description\": \"UpdateWebhookInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the CodeBuild project.\"\n        }\n      ]\n    },\n    \"branchFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>A regular expression used to determine which repository branches are built when a webhook is triggered. If the name of a branch matches the regular expression, then it is built. If <code>branchFilter</code>\
  \ is empty, then all branches are built.</p> <note> <p> It is recommended that you use <code>filterGroups</code> instead of <code>branchFilter</code>. </p> </note>\"\n        }\n      ]\n    },\n    \"rotateSecret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" A boolean value that specifies whether the associated GitHub repository's secret token should be updated. If you use Bitbucket for your repository, <code>rotateSecret</code> is ignored. \"\n        }\n      ]\n    },\n    \"filterGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterGroups\"\n        },\n        {\n          \"description\": \" An array of arrays of <code>WebhookFilter</code> objects used to determine if a webhook event can trigger a build. A filter group must contain at least one <code>EVENT</code> <code>WebhookFilter</code>. \"\n        }\n      ]\n    },\n    \"buildType\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookBuildType\"\n        },\n        {\n          \"description\": \"Specifies the type of build this webhook will trigger.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-update-webhook-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: UpdateWebhookInput
---
