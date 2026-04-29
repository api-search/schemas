---
description: CreateWorldExportJobRequest schema from openapi
layout: schema
name: CreateWorldExportJobRequest
properties_list:
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: worlds
  type: object
- description: ''
  name: outputLocation
  type: object
- description: ''
  name: iamRole
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-create-world-export-job-request-schema.json
slug: amazon-robomaker-openapi-create-world-export-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-world-export-job-request-schema.json\",\n  \"title\": \"CreateWorldExportJobRequest\",\n  \"description\": \"CreateWorldExportJobRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"worlds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arns\"\n        },\n        {\n          \"description\": \"A list of Amazon Resource Names (arns) that correspond to worlds to export.\"\n        }\n      ]\n    },\n    \"outputLocation\"\
  : {\n      \"$ref\": \"#/components/schemas/OutputLocation\"\n    },\n    \"iamRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRole\"\n        },\n        {\n          \"description\": \"The IAM role that the world export process uses to access the Amazon S3 bucket and put the export.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the world export job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"worlds\",\n    \"outputLocation\",\n    \"iamRole\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-world-export-job-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: CreateWorldExportJobRequest
---
