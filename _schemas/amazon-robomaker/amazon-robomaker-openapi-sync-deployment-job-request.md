---
description: Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: SyncDeploymentJobRequest
properties_list:
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: fleet
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-sync-deployment-job-request-schema.json
slug: amazon-robomaker-openapi-sync-deployment-job-request
source_filename: amazon-robomaker-openapi-sync-deployment-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-sync-deployment-job-request-schema.json\",\n  \"title\": \"SyncDeploymentJobRequest\",\n  \"description\": \"Support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"fleet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The target\
  \ fleet for the synchronization.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"clientRequestToken\",\n    \"fleet\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-sync-deployment-job-request-schema.json
tags:
- Robotics
- Simulation
title: SyncDeploymentJobRequest
---
