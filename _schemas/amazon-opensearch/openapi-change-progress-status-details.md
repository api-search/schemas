---
description: The progress details of a specific domain configuration change.
layout: schema
name: ChangeProgressStatusDetails
properties_list:
- description: ''
  name: ChangeId
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: PendingProperties
  type: object
- description: ''
  name: CompletedProperties
  type: object
- description: ''
  name: TotalNumberOfStages
  type: object
- description: ''
  name: ChangeProgressStages
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-change-progress-status-details-schema.json
slug: openapi-change-progress-status-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-change-progress-status-details-schema.json\",\n  \"title\": \"ChangeProgressStatusDetails\",\n  \"description\": \"The progress details of a specific domain configuration change.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GUID\"\n        },\n        {\n          \"description\": \"The unique change identifier associated with a specific domain configuration change.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateTimestamp\"\n        },\n        {\n          \"description\": \"The time at which the configuration change is made on the domain.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/OverallChangeStatus\"\n        },\n        {\n          \"description\": \"The overall status of the domain configuration change. This field can take the following values: <code>PENDING</code>, <code>PROCESSING</code>, <code>COMPLETED</code> and <code>FAILED</code>\"\n        }\n      ]\n    },\n    \"PendingProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The list of properties involved in the domain configuration change that are still in pending.\"\n        }\n      ]\n    },\n    \"CompletedProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\n        },\n        {\n          \"description\": \"The list of properties involved in the domain configuration change that are completed.\"\n        }\n      ]\n    },\n    \"TotalNumberOfStages\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/TotalNumberOfStages\"\n        },\n        {\n          \"description\": \"The total number of stages required for the configuration change.\"\n        }\n      ]\n    },\n    \"ChangeProgressStages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeProgressStageList\"\n        },\n        {\n          \"description\": \"The specific stages that the domain is going through to perform the configuration change.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-change-progress-status-details-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ChangeProgressStatusDetails
---
