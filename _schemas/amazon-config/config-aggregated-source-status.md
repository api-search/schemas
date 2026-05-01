---
description: The current sync status between the source and the aggregator account.
layout: schema
name: AggregatedSourceStatus
properties_list:
- description: ''
  name: SourceId
  type: object
- description: ''
  name: SourceType
  type: object
- description: ''
  name: AwsRegion
  type: object
- description: ''
  name: LastUpdateStatus
  type: object
- description: ''
  name: LastUpdateTime
  type: object
- description: ''
  name: LastErrorCode
  type: object
- description: ''
  name: LastErrorMessage
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-aggregated-source-status-schema.json
slug: config-aggregated-source-status
source_filename: config-aggregated-source-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregated-source-status-schema.json\",\n  \"title\": \"AggregatedSourceStatus\",\n  \"description\": \"The current sync status between the source and the aggregator account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The source account ID or an organization.\"\n        }\n      ]\n    },\n    \"SourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedSourceType\"\n        },\n        {\n          \"description\": \"The source account or an organization.\"\n        }\n      ]\n    },\n    \"AwsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n\
  \        },\n        {\n          \"description\": \"The region authorized to collect aggregated data.\"\n        }\n      ]\n    },\n    \"LastUpdateStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AggregatedSourceStatusType\"\n        },\n        {\n          \"description\": \"<p>Filters the last updated status type.</p> <ul> <li> <p>Valid value FAILED indicates errors while moving data.</p> </li> <li> <p>Valid value SUCCEEDED indicates the data was successfully moved.</p> </li> <li> <p>Valid value OUTDATED indicates the data is not the most recent.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"LastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time of the last update.\"\n        }\n      ]\n    },\n    \"LastErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n \
  \         \"description\": \"The error code that Config returned when the source account aggregation last failed.\"\n        }\n      ]\n    },\n    \"LastErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The message indicating that the source account aggregation failed due to an error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-aggregated-source-status-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: AggregatedSourceStatus
---
