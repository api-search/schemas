---
description: CancelServiceInstanceDeploymentInput schema from Amazon Proton API
layout: schema
name: CancelServiceInstanceDeploymentInput
properties_list:
- description: ''
  name: serviceInstanceName
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-cancel-service-instance-deployment-input-schema.json
slug: amazon-proton-cancel-service-instance-deployment-input
source_filename: amazon-proton-cancel-service-instance-deployment-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-cancel-service-instance-deployment-input-schema.json\",\n  \"title\": \"CancelServiceInstanceDeploymentInput\",\n  \"description\": \"CancelServiceInstanceDeploymentInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceInstanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service instance with the deployment to cancel.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service with the service instance deployment to cancel.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"serviceInstanceName\",\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-cancel-service-instance-deployment-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CancelServiceInstanceDeploymentInput
---
