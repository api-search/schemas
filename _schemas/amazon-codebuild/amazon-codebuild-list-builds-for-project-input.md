---
description: ListBuildsForProjectInput schema from Amazon CodeBuild
layout: schema
name: ListBuildsForProjectInput
properties_list:
- description: ''
  name: projectName
  type: object
- description: ''
  name: sortOrder
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-builds-for-project-input-schema.json
slug: amazon-codebuild-list-builds-for-project-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-builds-for-project-input-schema.json\",\n  \"title\": \"ListBuildsForProjectInput\",\n  \"description\": \"ListBuildsForProjectInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the CodeBuild project.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrderType\"\n        },\n        {\n          \"description\": \"<p>The order to sort the results in. The results are sorted by build number, not the build identifier. If this is not specified, the results are sorted in descending order.</p> <p>Valid\
  \ values include:</p> <ul> <li> <p> <code>ASCENDING</code>: List the build identifiers in ascending order, by build number.</p> </li> <li> <p> <code>DESCENDING</code>: List the build identifiers in descending order, by build number.</p> </li> </ul> <p>If the project has more than 100 builds, setting the sort order will result in an error. </p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"During a previous call, if there are more than 100 items in the list, only the first 100 items are returned, along with a unique string called a <i>nextToken</i>. To get the next batch of items in the list, call this operation again, adding the next token to the call. To get all of the items in the list, keep calling this operation with each subsequent next token that is returned, until no more next tokens are returned.\"\n        }\n      ]\n    }\n  },\n  \"\
  required\": [\n    \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-builds-for-project-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListBuildsForProjectInput
---
