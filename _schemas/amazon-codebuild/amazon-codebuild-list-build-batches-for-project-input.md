---
description: ListBuildBatchesForProjectInput schema from Amazon CodeBuild
layout: schema
name: ListBuildBatchesForProjectInput
properties_list:
- description: ''
  name: projectName
  type: object
- description: ''
  name: filter
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: sortOrder
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-build-batches-for-project-input-schema.json
slug: amazon-codebuild-list-build-batches-for-project-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-build-batches-for-project-input-schema.json\",\n  \"title\": \"ListBuildBatchesForProjectInput\",\n  \"description\": \"ListBuildBatchesForProjectInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the project.\"\n        }\n      ]\n    },\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildBatchFilter\"\n        },\n        {\n          \"description\": \"A <code>BuildBatchFilter</code> object that specifies the filters for the search.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of results to return.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrderType\"\n        },\n        {\n          \"description\": \"<p>Specifies the sort order of the returned items. Valid values include:</p> <ul> <li> <p> <code>ASCENDING</code>: List the batch build identifiers in ascending order by identifier.</p> </li> <li> <p> <code>DESCENDING</code>: List the batch build identifiers in descending order by identifier.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value returned from a previous call to <code>ListBuildBatchesForProject</code>. This specifies the next item to return. To return the\
  \ beginning of the list, exclude this parameter.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-build-batches-for-project-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListBuildBatchesForProjectInput
---
