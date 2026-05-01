---
description: History of the last 10 Upgrades and Upgrade Eligibility Checks.
layout: schema
name: UpgradeHistory
properties_list:
- description: ''
  name: UpgradeName
  type: object
- description: ''
  name: StartTimestamp
  type: object
- description: ''
  name: UpgradeStatus
  type: object
- description: ''
  name: StepsList
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-upgrade-history-schema.json
slug: openapi-upgrade-history
source_filename: openapi-upgrade-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-upgrade-history-schema.json\",\n  \"title\": \"UpgradeHistory\",\n  \"description\": \"History of the last 10 Upgrades and Upgrade Eligibility Checks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpgradeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpgradeName\"\n        },\n        {\n          \"description\": \"A string that describes the update briefly\"\n        }\n      ]\n    },\n    \"StartTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartTimestamp\"\n        },\n        {\n          \"description\": \"UTC Timestamp at which the Upgrade API call was made in \\\"yyyy-MM-ddTHH:mm:ssZ\\\" format.\"\n        }\n      ]\n    },\n    \"UpgradeStatus\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/UpgradeStatus\"\n        },\n        {\n          \"description\": \" The overall status of the update. The status can take one of the following values: <ul> <li>In Progress</li> <li>Succeeded</li> <li>Succeeded with Issues</li> <li>Failed</li> </ul> \"\n        }\n      ]\n    },\n    \"StepsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpgradeStepsList\"\n        },\n        {\n          \"description\": \" A list of <code> <a>UpgradeStepItem</a> </code> s representing information about each step performed as pard of a specific Upgrade or Upgrade Eligibility Check. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-upgrade-history-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: UpgradeHistory
---
