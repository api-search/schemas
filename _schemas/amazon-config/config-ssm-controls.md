---
description: Amazon Web Services Systems Manager (SSM) specific remediation controls.
layout: schema
name: SsmControls
properties_list:
- description: ''
  name: ConcurrentExecutionRatePercentage
  type: object
- description: ''
  name: ErrorPercentage
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-ssm-controls-schema.json
slug: config-ssm-controls
source_filename: config-ssm-controls-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-ssm-controls-schema.json\",\n  \"title\": \"SsmControls\",\n  \"description\": \"Amazon Web Services Systems Manager (SSM) specific remediation controls.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConcurrentExecutionRatePercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The maximum percentage of remediation actions allowed to run in parallel on the non-compliant resources for that specific rule. You can specify a percentage, such as 10%. The default value is 10. \"\n        }\n      ]\n    },\n    \"ErrorPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of errors\
  \ that are allowed before SSM stops running automations on non-compliant resources for that specific rule. You can specify a percentage of errors, for example 10%. If you do not specifiy a percentage, the default is 50%. For example, if you set the ErrorPercentage to 40% for 10 non-compliant resources, then SSM stops running the automations when the fifth error is received. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-ssm-controls-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: SsmControls
---
