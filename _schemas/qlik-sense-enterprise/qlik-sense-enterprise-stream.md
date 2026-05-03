---
description: A Qlik Sense stream is a logical grouping mechanism for organizing and distributing published applications. Streams control access to published apps through security rules, enabling administrators to manage which users can see and interact with specific analytics content.
layout: schema
name: Qlik Sense Stream
properties_list:
- description: Unique identifier (GUID) assigned by the repository
  name: id
  type: string
- description: ISO 8601 timestamp when the stream was created
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the stream was last modified
  name: modifiedDate
  type: string
- description: Username of the user who last modified the stream
  name: modifiedByUserName
  type: string
- description: Display name of the stream
  name: name
  type: string
- description: The user who owns the stream
  name: owner
  type: object
- description: Tags applied to the stream
  name: tags
  type: array
- description: Custom property values assigned to the stream
  name: customProperties
  type: array
- description: List of privileges the current user has on this stream
  name: privileges
  type: array
- description: Schema path identifying the entity type in the QRS
  name: schemaPath
  type: string
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
schema_file: json-schema/qlik-sense-enterprise-stream-schema.json
slug: qlik-sense-enterprise-stream
source_filename: qlik-sense-enterprise-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.dev/qlik-sense-enterprise/stream.json\",\n  \"title\": \"Qlik Sense Stream\",\n  \"description\": \"A Qlik Sense stream is a logical grouping mechanism for organizing and distributing published applications. Streams control access to published apps through security rules, enabling administrators to manage which users can see and interact with specific analytics content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier (GUID) assigned by the repository\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the stream was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp\
  \ when the stream was last modified\"\n    },\n    \"modifiedByUserName\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who last modified the stream\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the stream\",\n      \"minLength\": 1\n    },\n    \"owner\": {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"The user who owns the stream\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TagReference\"\n      },\n      \"description\": \"Tags applied to the stream\"\n    },\n    \"customProperties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomPropertyValue\"\n      },\n      \"description\": \"Custom property values assigned to the stream\"\n    },\n    \"privileges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of\
  \ privileges the current user has on this stream\"\n    },\n    \"schemaPath\": {\n      \"type\": \"string\",\n      \"description\": \"Schema path identifying the entity type in the QRS\"\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"UserReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"userDirectory\": {\n          \"type\": \"string\"\n        },\n        \"userId\": {\n          \"type\": \"string\"\n        },\n        \"privileges\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"TagReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\"\
  : \"string\"\n        },\n        \"privileges\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"CustomPropertyValue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"definition\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"valueType\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"value\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/json-schema/qlik-sense-enterprise-stream-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
title: Qlik Sense Stream
---
