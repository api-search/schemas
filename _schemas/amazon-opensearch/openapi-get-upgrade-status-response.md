---
description: Container for response returned by <code> <a>GetUpgradeStatus</a> </code> operation.
layout: schema
name: GetUpgradeStatusResponse
properties_list:
- description: ''
  name: UpgradeStep
  type: object
- description: ''
  name: StepStatus
  type: object
- description: ''
  name: UpgradeName
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-get-upgrade-status-response-schema.json
slug: openapi-get-upgrade-status-response
source_filename: openapi-get-upgrade-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-get-upgrade-status-response-schema.json\",\n  \"title\": \"GetUpgradeStatusResponse\",\n  \"description\": \" Container for response returned by <code> <a>GetUpgradeStatus</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpgradeStep\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpgradeStep\"\n        },\n        {\n          \"description\": \" Represents one of 3 steps that an Upgrade or Upgrade Eligibility Check does through: <ul> <li>PreUpgradeCheck</li> <li>Snapshot</li> <li>Upgrade</li> </ul> \"\n        }\n      ]\n    },\n    \"StepStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpgradeStatus\"\n        },\n        {\n          \"description\": \" One of 4 statuses that a step can go\
  \ through returned as part of the <code> <a>GetUpgradeStatusResponse</a> </code> object. The status can take one of the following values: <ul> <li>In Progress</li> <li>Succeeded</li> <li>Succeeded with Issues</li> <li>Failed</li> </ul> \"\n        }\n      ]\n    },\n    \"UpgradeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpgradeName\"\n        },\n        {\n          \"description\": \"A string that describes the update briefly\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-get-upgrade-status-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: GetUpgradeStatusResponse
---
