---
description: Provides information about types of supported endpoints in response to a request by the <code>DescribeEndpointTypes</code> operation. This information includes the type of endpoint, the database engine name, and whether change data capture (CDC) is supported.
layout: schema
name: SupportedEndpointType
properties_list:
- description: ''
  name: EngineName
  type: object
- description: ''
  name: SupportsCDC
  type: object
- description: ''
  name: EndpointType
  type: object
- description: ''
  name: ReplicationInstanceEngineMinimumVersion
  type: object
- description: ''
  name: EngineDisplayName
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-supported-endpoint-type-schema.json
slug: amazon-dms-supported-endpoint-type
source_filename: amazon-dms-supported-endpoint-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-supported-endpoint-type-schema.json\",\n  \"title\": \"SupportedEndpointType\",\n  \"description\": \"Provides information about types of supported endpoints in response to a request by the <code>DescribeEndpointTypes</code> operation. This information includes the type of endpoint, the database engine name, and whether change data capture (CDC) is supported.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EngineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The database engine name. Valid values, depending on the EndpointType, include <code>\\\"mysql\\\"</code>, <code>\\\"oracle\\\"</code>, <code>\\\"postgres\\\"</code>, <code>\\\"mariadb\\\"</code>, <code>\\\"aurora\\\"</code>, <code>\\\"\
  aurora-postgresql\\\"</code>, <code>\\\"redshift\\\"</code>, <code>\\\"s3\\\"</code>, <code>\\\"db2\\\"</code>, <code>\\\"db2-zos\\\"</code>, <code>\\\"azuredb\\\"</code>, <code>\\\"sybase\\\"</code>, <code>\\\"dynamodb\\\"</code>, <code>\\\"mongodb\\\"</code>, <code>\\\"kinesis\\\"</code>, <code>\\\"kafka\\\"</code>, <code>\\\"elasticsearch\\\"</code>, <code>\\\"documentdb\\\"</code>, <code>\\\"sqlserver\\\"</code>, <code>\\\"neptune\\\"</code>, and <code>\\\"babelfish\\\"</code>.\"\n        }\n      ]\n    },\n    \"SupportsCDC\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates if change data capture (CDC) is supported.\"\n        }\n      ]\n    },\n    \"EndpointType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationEndpointTypeValue\"\n        },\n        {\n          \"description\": \"The type of endpoint. Valid values are <code>source</code>\
  \ and <code>target</code>.\"\n        }\n      ]\n    },\n    \"ReplicationInstanceEngineMinimumVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The earliest DMS engine version that supports this endpoint engine. Note that endpoint engines released with DMS versions earlier than 3.1.1 do not return a value for this parameter.\"\n        }\n      ]\n    },\n    \"EngineDisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The expanded name for the engine name. For example, if the <code>EngineName</code> parameter is \\\"aurora\\\", this value would be \\\"Amazon Aurora MySQL\\\".\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-supported-endpoint-type-schema.json
tags:
- Data Replication
- Database
- Database Migration
- Migration
title: SupportedEndpointType
---
