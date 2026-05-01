---
description: Information about a webhook that connects repository events to a build project in CodeBuild.
layout: schema
name: Webhook
properties_list:
- description: ''
  name: url
  type: object
- description: ''
  name: payloadUrl
  type: object
- description: ''
  name: secret
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
- description: ''
  name: lastModifiedSecret
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-webhook-schema.json
slug: amazon-codebuild-webhook
source_filename: amazon-codebuild-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-webhook-schema.json\",\n  \"title\": \"Webhook\",\n  \"description\": \"Information about a webhook that connects repository events to a build project in CodeBuild.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The URL to the webhook.\"\n        }\n      ]\n    },\n    \"payloadUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The CodeBuild endpoint where webhook events are sent.\"\n        }\n      ]\n    },\n    \"secret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n \
  \       },\n        {\n          \"description\": \"<p>The secret token of the associated repository. </p> <note> <p>A Bitbucket webhook does not support <code>secret</code>. </p> </note>\"\n        }\n      ]\n    },\n    \"branchFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>A regular expression used to determine which repository branches are built when a webhook is triggered. If the name of a branch matches the regular expression, then it is built. If <code>branchFilter</code> is empty, then all branches are built.</p> <note> <p>It is recommended that you use <code>filterGroups</code> instead of <code>branchFilter</code>. </p> </note>\"\n        }\n      ]\n    },\n    \"filterGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterGroups\"\n        },\n        {\n          \"description\": \"<p>An array of arrays of <code>WebhookFilter</code>\
  \ objects used to determine which webhooks are triggered. At least one <code>WebhookFilter</code> in the array must specify <code>EVENT</code> as its <code>type</code>. </p> <p>For a build to be triggered, at least one filter group in the <code>filterGroups</code> array must pass. For a filter group to pass, each of its filters must pass. </p>\"\n        }\n      ]\n    },\n    \"buildType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebhookBuildType\"\n        },\n        {\n          \"description\": \"Specifies the type of build this webhook will trigger.\"\n        }\n      ]\n    },\n    \"lastModifiedSecret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A timestamp that indicates the last time a repository's secret token was modified. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-webhook-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: Webhook
---
