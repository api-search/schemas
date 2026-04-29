---
description: CreateSimulationApplicationVersionRequest schema from openapi
layout: schema
name: CreateSimulationApplicationVersionRequest
properties_list:
- description: ''
  name: application
  type: object
- description: ''
  name: currentRevisionId
  type: object
- description: ''
  name: s3Etags
  type: object
- description: ''
  name: imageDigest
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-create-simulation-application-version-request-schema.json
slug: amazon-robomaker-openapi-create-simulation-application-version-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-simulation-application-version-request-schema.json\",\n  \"title\": \"CreateSimulationApplicationVersionRequest\",\n  \"description\": \"CreateSimulationApplicationVersionRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The application information for the simulation application.\"\n        }\n      ]\n    },\n    \"currentRevisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \"The current revision id for the simulation application. If you provide a value and it matches the latest revision\
  \ ID, a new version will be created.\"\n        }\n      ]\n    },\n    \"s3Etags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Etags\"\n        },\n        {\n          \"description\": \"The Amazon S3 eTag identifier for the zip file bundle that you use to create the simulation application.\"\n        }\n      ]\n    },\n    \"imageDigest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageDigest\"\n        },\n        {\n          \"description\": \"The SHA256 digest used to identify the Docker image URI used to created the simulation application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"application\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-simulation-application-version-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: CreateSimulationApplicationVersionRequest
---
