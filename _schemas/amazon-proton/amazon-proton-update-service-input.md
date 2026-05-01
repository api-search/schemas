---
description: UpdateServiceInput schema from Amazon Proton API
layout: schema
name: UpdateServiceInput
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: spec
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-update-service-input-schema.json
slug: amazon-proton-update-service-input
source_filename: amazon-proton-update-service-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-input-schema.json\",\n  \"title\": \"UpdateServiceInput\",\n  \"description\": \"UpdateServiceInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The edited service description.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the service to edit.\"\n        }\n      ]\n    },\n    \"spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpecContents\"\n        },\n        {\n          \"description\"\
  : \"Lists the service instances to add and the existing service instances to remain. Omit the existing service instances to delete from the list. <i>Don't</i> include edits to the existing service instances or pipeline. For more information, see <a href=\\\"https://docs.aws.amazon.com/proton/latest/userguide/ag-svc-update.html\\\">Edit a service</a> in the <i>Proton User Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-update-service-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: UpdateServiceInput
---
