---
description: A Qlik Sense application (app) containing data models, visualizations, sheets, stories, and bookmarks. Apps are the primary container for analytics content in Qlik Sense Enterprise.
layout: schema
name: Qlik Sense Application
properties_list:
- description: Unique identifier (GUID) assigned by the repository
  name: id
  type: string
- description: ISO 8601 timestamp when the app was created
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the app was last modified. Used for optimistic concurrency control.
  name: modifiedDate
  type: string
- description: Username of the user who last modified the app
  name: modifiedByUserName
  type: string
- description: Display name of the application
  name: name
  type: string
- description: Internal application identifier used by the engine
  name: appId
  type: string
- description: Description of the application's purpose and content
  name: description
  type: string
- description: ISO 8601 timestamp when the app was published to a stream
  name: publishTime
  type: string
- description: Whether the app is currently published to a stream
  name: published
  type: boolean
- description: The stream the app is published to, if any
  name: stream
  type: object
- description: Size of the application QVF file in bytes
  name: fileSize
  type: integer
- description: ISO 8601 timestamp of the last successful data reload
  name: lastReloadTime
  type: string
- description: Relative path to the application thumbnail image
  name: thumbnail
  type: string
- description: Qlik Sense product version the app was last saved in
  name: savedInProductVersion
  type: string
- description: Hash indicating the migration state of the app
  name: migrationHash
  type: string
- description: Availability status of the app
  name: availabilityStatus
  type: integer
- description: The user who owns the application
  name: owner
  type: object
- description: Tags applied to the application for categorization
  name: tags
  type: array
- description: Custom property values assigned to the application
  name: customProperties
  type: array
- description: List of privileges the current user has on this app
  name: privileges
  type: array
- description: Schema path identifying the entity type in the QRS
  name: schemaPath
  type: string
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
schema_file: json-schema/qlik-sense-enterprise-app-schema.json
slug: qlik-sense-enterprise-app
source_filename: qlik-sense-enterprise-app-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.dev/qlik-sense-enterprise/app.json\",\n  \"title\": \"Qlik Sense Application\",\n  \"description\": \"A Qlik Sense application (app) containing data models, visualizations, sheets, stories, and bookmarks. Apps are the primary container for analytics content in Qlik Sense Enterprise.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier (GUID) assigned by the repository\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the app was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the app was last modified. Used for optimistic concurrency control.\"\n    },\n    \"modifiedByUserName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who last modified the app\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the application\",\n      \"minLength\": 1\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"Internal application identifier used by the engine\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the application's purpose and content\"\n    },\n    \"publishTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the app was published to a stream\"\n    },\n    \"published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the app is currently published to a stream\",\n      \"default\": false\n    },\n    \"stream\": {\n      \"$ref\": \"#/$defs/StreamReference\",\n      \"description\": \"The stream the app is published\
  \ to, if any\"\n    },\n    \"fileSize\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Size of the application QVF file in bytes\",\n      \"minimum\": 0\n    },\n    \"lastReloadTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last successful data reload\"\n    },\n    \"thumbnail\": {\n      \"type\": \"string\",\n      \"description\": \"Relative path to the application thumbnail image\"\n    },\n    \"savedInProductVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Qlik Sense product version the app was last saved in\"\n    },\n    \"migrationHash\": {\n      \"type\": \"string\",\n      \"description\": \"Hash indicating the migration state of the app\"\n    },\n    \"availabilityStatus\": {\n      \"type\": \"integer\",\n      \"description\": \"Availability status of the app\",\n      \"enum\": [0, 1],\n      \"default\": 0\n    },\n    \"owner\"\
  : {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"The user who owns the application\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TagReference\"\n      },\n      \"description\": \"Tags applied to the application for categorization\"\n    },\n    \"customProperties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomPropertyValue\"\n      },\n      \"description\": \"Custom property values assigned to the application\"\n    },\n    \"privileges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of privileges the current user has on this app\"\n    },\n    \"schemaPath\": {\n      \"type\": \"string\",\n      \"description\": \"Schema path identifying the entity type in the QRS\"\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"StreamReference\": {\n      \"type\": \"object\",\n    \
  \  \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"privileges\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"UserReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"userDirectory\": {\n          \"type\": \"string\"\n        },\n        \"userId\": {\n          \"type\": \"string\"\n        },\n        \"privileges\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"TagReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"\
  string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"privileges\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"CustomPropertyValue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"createdDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"modifiedDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"modifiedByUserName\": {\n          \"type\": \"string\"\n        },\n        \"definition\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\"\n            },\n            \"name\": {\n             \
  \ \"type\": \"string\"\n            },\n            \"valueType\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"value\": {\n          \"type\": \"string\"\n        },\n        \"schemaPath\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/json-schema/qlik-sense-enterprise-app-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
title: Qlik Sense Application
---
