---
description: DeleteProjectRequest schema from AWS CodeStar API
layout: schema
name: DeleteProjectRequest
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: deleteStack
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-delete-project-request-schema.json
slug: codestar-delete-project-request
source_filename: codestar-delete-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-delete-project-request-schema.json\",\n  \"title\": \"DeleteProjectRequest\",\n  \"description\": \"DeleteProjectRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project to be deleted in AWS CodeStar.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"A user- or system-generated token that identifies the entity that requested project deletion. This token can be used to repeat the request. \"\n        }\n      ]\n    },\n    \"deleteStack\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeleteStack\"\n        },\n        {\n          \"description\": \"Whether to send a delete request for the primary stack in AWS CloudFormation originally used to generate the project and its resources. This option will delete all AWS resources for the project (except for any buckets in Amazon S3) as well as deleting the project itself. Recommended for most use cases.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-delete-project-request-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: DeleteProjectRequest
---
