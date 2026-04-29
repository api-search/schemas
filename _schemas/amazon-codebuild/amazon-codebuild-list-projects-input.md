---
description: ListProjectsInput schema from Amazon CodeBuild
layout: schema
name: ListProjectsInput
properties_list:
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-projects-input-schema.json
slug: amazon-codebuild-list-projects-input
source_filename: amazon-codebuild-list-projects-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-projects-input-schema.json\",\n  \"title\": \"ListProjectsInput\",\n  \"description\": \"ListProjectsInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectSortByType\"\n        },\n        {\n          \"description\": \"<p>The criterion to be used to list build project names. Valid values include:</p> <ul> <li> <p> <code>CREATED_TIME</code>: List based on when each build project was created.</p> </li> <li> <p> <code>LAST_MODIFIED_TIME</code>: List based on when information about each build project was last changed.</p> </li> <li> <p> <code>NAME</code>: List based on each build project's name.</p> </li> </ul> <p>Use <code>sortOrder</code> to specify in\
  \ what order to list the build project names based on the preceding criteria.</p>\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrderType\"\n        },\n        {\n          \"description\": \"<p>The order in which to list build projects. Valid values include:</p> <ul> <li> <p> <code>ASCENDING</code>: List in ascending order.</p> </li> <li> <p> <code>DESCENDING</code>: List in descending order.</p> </li> </ul> <p>Use <code>sortBy</code> to specify the criterion to be used to list build project names.</p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"During a previous call, if there are more than 100 items in the list, only the first 100 items are returned, along with a unique string called a <i>nextToken</i>. To get the next batch of items in the list, call\
  \ this operation again, adding the next token to the call. To get all of the items in the list, keep calling this operation with each subsequent next token that is returned, until no more next tokens are returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-projects-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListProjectsInput
---
