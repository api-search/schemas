---
description: <p>Step taken during a cluster operation.</p>
layout: schema
name: ClusterOperationStep
properties_list:
- description: ''
  name: StepInfo
  type: object
- description: ''
  name: StepName
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-cluster-operation-step-schema.json
slug: msk-api-cluster-operation-step
source_filename: msk-api-cluster-operation-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-operation-step-schema.json\",\n  \"title\": \"ClusterOperationStep\",\n  \"description\": \"\\n            <p>Step taken during a cluster operation.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StepInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterOperationStepInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stepInfo\"\n          },\n          \"description\": \"\\n            <p>Information about the step and its status.</p>\"\n        }\n      ]\n    },\n    \"StepName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stepName\"\n          },\n          \"description\": \"\\n            <p>The name\
  \ of the step.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-operation-step-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ClusterOperationStep
---
