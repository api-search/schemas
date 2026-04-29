---
description: Uniquely identifies an evaluation result.
layout: schema
name: EvaluationResultIdentifier
properties_list:
- description: ''
  name: EvaluationResultQualifier
  type: object
- description: ''
  name: OrderingTimestamp
  type: object
- description: ''
  name: ResourceEvaluationId
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-evaluation-result-identifier-schema.json
slug: config-evaluation-result-identifier
source_filename: config-evaluation-result-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-result-identifier-schema.json\",\n  \"title\": \"EvaluationResultIdentifier\",\n  \"description\": \"Uniquely identifies an evaluation result.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EvaluationResultQualifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationResultQualifier\"\n        },\n        {\n          \"description\": \"Identifies an Config rule used to evaluate an Amazon Web Services resource, and provides the type and ID of the evaluated resource.\"\n        }\n      ]\n    },\n    \"OrderingTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time of the event that triggered the evaluation of your Amazon Web Services resources.\
  \ The time can indicate when Config delivered a configuration item change notification, or it can indicate when Config delivered the configuration snapshot, depending on which event triggered the evaluation.\"\n        }\n      ]\n    },\n    \"ResourceEvaluationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluationId\"\n        },\n        {\n          \"description\": \"A Unique ID for an evaluation result.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-result-identifier-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: EvaluationResultIdentifier
---
