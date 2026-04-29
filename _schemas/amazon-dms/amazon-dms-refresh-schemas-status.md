---
description: Provides information that describes status of a schema at an endpoint specified by the <code>DescribeRefreshSchemaStatus</code> operation.
layout: schema
name: RefreshSchemasStatus
properties_list:
- description: ''
  name: EndpointArn
  type: object
- description: ''
  name: ReplicationInstanceArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: LastRefreshDate
  type: object
- description: ''
  name: LastFailureMessage
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-refresh-schemas-status-schema.json
slug: amazon-dms-refresh-schemas-status
source_filename: amazon-dms-refresh-schemas-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-refresh-schemas-status-schema.json\",\n  \"title\": \"RefreshSchemasStatus\",\n  \"description\": \"Provides information that describes status of a schema at an endpoint specified by the <code>DescribeRefreshSchemaStatus</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) string that uniquely identifies the endpoint.\"\n        }\n      ]\n    },\n    \"ReplicationInstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication instance.\"\n        }\n    \
  \  ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RefreshSchemasStatusTypeValue\"\n        },\n        {\n          \"description\": \"The status of the schema.\"\n        }\n      ]\n    },\n    \"LastRefreshDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date the schema was last refreshed.\"\n        }\n      ]\n    },\n    \"LastFailureMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The last failure message for the schema.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-refresh-schemas-status-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: RefreshSchemasStatus
---
