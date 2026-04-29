---
description: <p>State information about the operation step.</p>
layout: schema
name: ClusterOperationStepInfo
properties_list:
- description: ''
  name: StepStatus
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-cluster-operation-step-info-schema.json
slug: msk-api-cluster-operation-step-info
source_filename: msk-api-cluster-operation-step-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-operation-step-info-schema.json\",\n  \"title\": \"ClusterOperationStepInfo\",\n  \"description\": \"\\n            <p>State information about the operation step.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StepStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stepStatus\"\n          },\n          \"description\": \"\\n            <p>The steps current status.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-operation-step-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ClusterOperationStepInfo
---
