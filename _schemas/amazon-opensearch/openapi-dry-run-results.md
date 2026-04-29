---
description: DryRunResults schema from Amazon OpenSearch Service API
layout: schema
name: DryRunResults
properties_list:
- description: ''
  name: DeploymentType
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-dry-run-results-schema.json
slug: openapi-dry-run-results
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-dry-run-results-schema.json\",\n  \"title\": \"DryRunResults\",\n  \"description\": \"DryRunResults schema from Amazon OpenSearch Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeploymentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentType\"\n        },\n        {\n          \"description\": \" Specifies the deployment mechanism through which the update shall be applied on the domain. Possible responses are <code>Blue/Green</code> (The update will require a blue/green deployment.) <code>DynamicUpdate</code> (The update can be applied in-place without a Blue/Green deployment required.) <code>Undetermined</code> (The domain is undergoing an update which needs to complete before the deployment type can be predicted.) <code>None</code>\
  \ (The configuration change matches the current configuration and will not result in any update.) \"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"Contains an optional message associated with the DryRunResults.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-dry-run-results-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DryRunResults
---
