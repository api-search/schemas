---
description: A data connection defines how Qlik Sense connects to an external data source for loading data into applications. Connections specify the provider type, connection string, authentication credentials, and the architecture of the connector.
layout: schema
name: Qlik Sense Data Connection
properties_list:
- description: Unique identifier (GUID) assigned by the repository
  name: id
  type: string
- description: ISO 8601 timestamp when the data connection was created
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the data connection was last modified
  name: modifiedDate
  type: string
- description: Username of the user who last modified the connection
  name: modifiedByUserName
  type: string
- description: Display name of the data connection
  name: name
  type: string
- description: Connection string containing provider-specific parameters for connecting to the data source
  name: connectionstring
  type: string
- description: Connection provider type identifier (e.g., QvOdbcConnectorPackage.exe, QvOleDbConnectorPackage.exe, folder, web)
  name: type
  type: string
- description: Logon mode for the connection
  name: logOn
  type: integer
- description: Connector architecture
  name: architecture
  type: integer
- description: Engine object identifier associated with the connection
  name: engineObjectId
  type: string
- description: Username for authenticating to the data source
  name: username
  type: string
- description: Password for authenticating to the data source (write-only)
  name: password
  type: string
- description: The user who owns the data connection
  name: owner
  type: object
- description: Tags applied to the data connection
  name: tags
  type: array
- description: Custom property values assigned to the data connection
  name: customProperties
  type: array
- description: List of privileges the current user has on this connection
  name: privileges
  type: array
- description: Schema path identifying the entity type in the QRS
  name: schemaPath
  type: string
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
schema_file: json-schema/qlik-sense-enterprise-data-connection-schema.json
slug: qlik-sense-enterprise-data-connection
source_filename: qlik-sense-enterprise-data-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.dev/qlik-sense-enterprise/data-connection.json\",\n  \"title\": \"Qlik Sense Data Connection\",\n  \"description\": \"A data connection defines how Qlik Sense connects to an external data source for loading data into applications. Connections specify the provider type, connection string, authentication credentials, and the architecture of the connector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier (GUID) assigned by the repository\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the data connection was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the\
  \ data connection was last modified\"\n    },\n    \"modifiedByUserName\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who last modified the connection\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the data connection\",\n      \"minLength\": 1\n    },\n    \"connectionstring\": {\n      \"type\": \"string\",\n      \"description\": \"Connection string containing provider-specific parameters for connecting to the data source\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Connection provider type identifier (e.g., QvOdbcConnectorPackage.exe, QvOleDbConnectorPackage.exe, folder, web)\"\n    },\n    \"logOn\": {\n      \"type\": \"integer\",\n      \"description\": \"Logon mode for the connection\",\n      \"enum\": [0, 1],\n      \"default\": 0\n    },\n    \"architecture\": {\n      \"type\": \"integer\",\n      \"description\": \"Connector architecture\",\n      \"enum\"\
  : [0, 1, 2],\n      \"default\": 0\n    },\n    \"engineObjectId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Engine object identifier associated with the connection\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username for authenticating to the data source\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password for authenticating to the data source (write-only)\",\n      \"writeOnly\": true\n    },\n    \"owner\": {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"The user who owns the data connection\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TagReference\"\n      },\n      \"description\": \"Tags applied to the data connection\"\n    },\n    \"customProperties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomPropertyValue\"\n      },\n      \"\
  description\": \"Custom property values assigned to the data connection\"\n    },\n    \"privileges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of privileges the current user has on this connection\"\n    },\n    \"schemaPath\": {\n      \"type\": \"string\",\n      \"description\": \"Schema path identifying the entity type in the QRS\"\n    }\n  },\n  \"required\": [\"name\", \"connectionstring\", \"type\"],\n  \"$defs\": {\n    \"UserReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"userDirectory\": {\n          \"type\": \"string\"\n        },\n        \"userId\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"TagReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"CustomPropertyValue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"definition\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"value\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/json-schema/qlik-sense-enterprise-data-connection-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
title: Qlik Sense Data Connection
---
