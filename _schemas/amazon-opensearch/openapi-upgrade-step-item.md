---
description: Represents a single step of the Upgrade or Upgrade Eligibility Check workflow.
layout: schema
name: UpgradeStepItem
properties_list:
- description: ''
  name: UpgradeStep
  type: object
- description: ''
  name: UpgradeStepStatus
  type: object
- description: ''
  name: Issues
  type: object
- description: ''
  name: ProgressPercent
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-upgrade-step-item-schema.json
slug: openapi-upgrade-step-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-upgrade-step-item-schema.json\",\n  \"title\": \"UpgradeStepItem\",\n  \"description\": \"Represents a single step of the Upgrade or Upgrade Eligibility Check workflow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpgradeStep\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpgradeStep\"\n        },\n        {\n          \"description\": \" Represents one of 3 steps that an Upgrade or Upgrade Eligibility Check does through: <ul> <li>PreUpgradeCheck</li> <li>Snapshot</li> <li>Upgrade</li> </ul> \"\n        }\n      ]\n    },\n    \"UpgradeStepStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpgradeStatus\"\n        },\n        {\n          \"description\": \" The status of a particular step during an upgrade. The status\
  \ can take one of the following values: <ul> <li>In Progress</li> <li>Succeeded</li> <li>Succeeded with Issues</li> <li>Failed</li> </ul> \"\n        }\n      ]\n    },\n    \"Issues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Issues\"\n        },\n        {\n          \"description\": \"A list of strings containing detailed information about the errors encountered in a particular step.\"\n        }\n      ]\n    },\n    \"ProgressPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The Floating point value representing progress percentage of a particular step.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-upgrade-step-item-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: UpgradeStepItem
---
