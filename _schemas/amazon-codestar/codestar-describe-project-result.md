---
description: DescribeProjectResult schema from AWS CodeStar API
layout: schema
name: DescribeProjectResult
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: createdTimeStamp
  type: object
- description: ''
  name: stackId
  type: object
- description: ''
  name: projectTemplateId
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-describe-project-result-schema.json
slug: codestar-describe-project-result
source_filename: codestar-describe-project-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-describe-project-result-schema.json\",\n  \"title\": \"DescribeProjectResult\",\n  \"description\": \"DescribeProjectResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The display name for the project.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource\
  \ Name (ARN) for the project.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectDescription\"\n        },\n        {\n          \"description\": \"The description of the project, if any.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"A user- or system-generated token that identifies the entity that requested project creation. \"\n        }\n      ]\n    },\n    \"createdTimeStamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedTimestamp\"\n        },\n        {\n          \"description\": \"The date and time the project was created, in timestamp format.\"\n        }\n      ]\n    },\n    \"stackId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StackId\"\n        },\n   \
  \     {\n          \"description\": \"The ID of the primary stack in AWS CloudFormation used to generate resources for the project.\"\n        }\n      ]\n    },\n    \"projectTemplateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectTemplateId\"\n        },\n        {\n          \"description\": \"The ID for the AWS CodeStar project template used to create the project.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectStatus\"\n        },\n        {\n          \"description\": \"The project creation or deletion status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-describe-project-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: DescribeProjectResult
---
