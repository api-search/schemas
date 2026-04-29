---
description: CreateWebhookInput schema from Amazon CodeBuild
layout: schema
name: CreateWebhookInput
properties_list:
- description: ''
  name: projectName
  type: object
- description: ''
  name: branchFilter
  type: object
- description: ''
  name: filterGroups
  type: object
- description: ''
  name: buildType
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-create-webhook-input-schema.json
slug: amazon-codebuild-create-webhook-input
source_filename: amazon-codebuild-create-webhook-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-webhook-input-schema.json\",\n  \"title\": \"CreateWebhookInput\",\n  \"description\": \"CreateWebhookInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the CodeBuild project.\"\n        }\n      ]\n    },\n    \"branchFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>A regular expression used to determine which repository branches are built when a webhook is triggered. If the name of a branch matches the regular expression, then it is built. If <code>branchFilter</code>\
  \ is empty, then all branches are built.</p> <note> <p>It is recommended that you use <code>filterGroups</code> instead of <code>branchFilter</code>. </p> </note>\"\n        }\n      ]\n    },\n    \"filterGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterGroups\"\n        },\n        {\n          \"description\": \"<p>An array of arrays of <code>WebhookFilter</code> objects used to determine which webhooks are triggered. At least one <code>WebhookFilter</code> in the array must specify <code>EVENT</code> as its <code>type</code>. </p> <p>For a build to be triggered, at least one filter group in the <code>filterGroups</code> array must pass. For a filter group to pass, each of its filters must pass. </p>\"\n        }\n      ]\n    },\n    \"buildType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookBuildType\"\n        },\n        {\n          \"description\": \"Specifies the type of build this webhook will\
  \ trigger.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-create-webhook-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CreateWebhookInput
---
