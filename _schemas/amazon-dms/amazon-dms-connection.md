---
description: Status of the connection between an endpoint and a replication instance, including Amazon Resource Names (ARNs) and the last error message issued.
layout: schema
name: Connection
properties_list:
- description: ''
  name: ReplicationInstanceArn
  type: object
- description: ''
  name: EndpointArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: LastFailureMessage
  type: object
- description: ''
  name: EndpointIdentifier
  type: object
- description: ''
  name: ReplicationInstanceIdentifier
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-connection-schema.json
slug: amazon-dms-connection
source_filename: amazon-dms-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"Status of the connection between an endpoint and a replication instance, including Amazon Resource Names (ARNs) and the last error message issued.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReplicationInstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of the replication instance.\"\n        }\n      ]\n    },\n    \"EndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN string that uniquely identifies the endpoint.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The connection status. This parameter can return one of the following values:</p> <ul> <li> <p> <code>\\\"successful\\\"</code> </p> </li> <li> <p> <code>\\\"testing\\\"</code> </p> </li> <li> <p> <code>\\\"failed\\\"</code> </p> </li> <li> <p> <code>\\\"deleting\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"LastFailureMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error message when the connection last failed.\"\n        }\n      ]\n    },\n    \"EndpointIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier of the endpoint. Identifiers must begin with a letter and must contain only ASCII letters, digits, and hyphens. They can't end with a hyphen\
  \ or contain two consecutive hyphens.\"\n        }\n      ]\n    },\n    \"ReplicationInstanceIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The replication instance identifier. This parameter is stored as a lowercase string.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-connection-schema.json
tags:
- Data Replication
- Database
- Database Migration
- Migration
title: Connection
---
