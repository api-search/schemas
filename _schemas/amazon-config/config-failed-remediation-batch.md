---
description: List of each of the failed remediations with specific reasons.
layout: schema
name: FailedRemediationBatch
properties_list:
- description: ''
  name: FailureMessage
  type: object
- description: ''
  name: FailedItems
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-failed-remediation-batch-schema.json
slug: config-failed-remediation-batch
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-failed-remediation-batch-schema.json\",\n  \"title\": \"FailedRemediationBatch\",\n  \"description\": \"List of each of the failed remediations with specific reasons.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailureMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Returns a failure message. For example, the resource is already compliant.\"\n        }\n      ]\n    },\n    \"FailedItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemediationConfigurations\"\n        },\n        {\n          \"description\": \"Returns remediation configurations of the failed items.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-failed-remediation-batch-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: FailedRemediationBatch
---
