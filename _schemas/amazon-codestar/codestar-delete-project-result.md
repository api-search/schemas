---
description: DeleteProjectResult schema from AWS CodeStar API
layout: schema
name: DeleteProjectResult
properties_list:
- description: ''
  name: stackId
  type: object
- description: ''
  name: projectArn
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-delete-project-result-schema.json
slug: codestar-delete-project-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-delete-project-result-schema.json\",\n  \"title\": \"DeleteProjectResult\",\n  \"description\": \"DeleteProjectResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stackId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StackId\"\n        },\n        {\n          \"description\": \"The ID of the primary stack in AWS CloudFormation that will be deleted as part of deleting the project and its resources.\"\n        }\n      ]\n    },\n    \"projectArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the deleted project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-delete-project-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: DeleteProjectResult
---
