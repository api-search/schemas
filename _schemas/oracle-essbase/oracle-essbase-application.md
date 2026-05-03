---
description: An Oracle Essbase application containing one or more databases (cubes) for multi-dimensional analysis. Applications serve as the top-level container for databases, scripts, connections, and security configuration.
layout: schema
name: Oracle Essbase Application
properties_list:
- description: Application name. Limited to 30 characters, must not contain spaces, and is case-insensitive.
  name: name
  type: string
- description: User ID of the application owner who created the application.
  name: owner
  type: string
- description: Application creation timestamp in milliseconds since Unix epoch.
  name: creationTime
  type: integer
- description: User ID of the person who last modified the application.
  name: modifiedBy
  type: string
- description: Last modification timestamp in milliseconds since Unix epoch.
  name: modifiedTime
  type: integer
- description: Current runtime status of the application.
  name: status
  type: string
- description: Human-readable description of the application purpose.
  name: description
  type: string
- description: Storage type of the application. ASO is aggregate storage optimized for read-heavy workloads. BSO is block storage optimized for write-heavy workloads. CURRENCY is for currency conversion applications
  name: type
  type: string
- description: Timestamp when the application was last started, in milliseconds since Unix epoch.
  name: startTime
  type: integer
- description: Number of users currently connected to the application.
  name: connectedUsersCount
  type: integer
- description: The authenticated user's role for this application (e.g., app_manager).
  name: role
  type: string
- description: If true, the application is managed in EAS Lite instead of the Essbase web interface.
  name: easManagedApp
  type: boolean
- description: Whether users with read permission can start the application.
  name: startStopAppAllowed
  type: boolean
- description: Whether application inspection is allowed.
  name: inspectAppAllowed
  type: boolean
- description: Whether the application data is encrypted at rest.
  name: encrypted
  type: boolean
- description: Name of the AI connection configuration associated with this application.
  name: aiConnection
  type: string
- description: ''
  name: appVariablesSetting
  type: object
- description: HATEOAS navigation links for related resources.
  name: links
  type: array
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-application-schema.json
slug: oracle-essbase-application
source_filename: oracle-essbase-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-application-schema.json\",\n  \"title\": \"Oracle Essbase Application\",\n  \"description\": \"An Oracle Essbase application containing one or more databases (cubes) for multi-dimensional analysis. Applications serve as the top-level container for databases, scripts, connections, and security configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name. Limited to 30 characters, must not contain spaces, and is case-insensitive.\",\n      \"maxLength\": 30\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the application owner who created the application.\"\n    },\n    \"creationTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Application creation timestamp in milliseconds since Unix epoch.\"\n    },\n    \"modifiedBy\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"User ID of the person who last modified the application.\"\n    },\n    \"modifiedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last modification timestamp in milliseconds since Unix epoch.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current runtime status of the application.\",\n      \"enum\": [\"started\", \"stopped\"]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the application purpose.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Storage type of the application. ASO is aggregate storage optimized for read-heavy workloads. BSO is block storage optimized for write-heavy workloads. CURRENCY is for currency conversion applications.\",\n      \"enum\": [\"ASO\", \"BSO\", \"CURRENCY\"]\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"\
  Timestamp when the application was last started, in milliseconds since Unix epoch.\"\n    },\n    \"connectedUsersCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of users currently connected to the application.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The authenticated user's role for this application (e.g., app_manager).\"\n    },\n    \"easManagedApp\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the application is managed in EAS Lite instead of the Essbase web interface.\"\n    },\n    \"startStopAppAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether users with read permission can start the application.\"\n    },\n    \"inspectAppAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether application inspection is allowed.\"\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application data is encrypted at\
  \ rest.\"\n    },\n    \"aiConnection\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the AI connection configuration associated with this application.\"\n    },\n    \"appVariablesSetting\": {\n      \"$ref\": \"#/$defs/VariablesSetting\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"HATEOAS navigation links for related resources.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"VariablesSetting\": {\n      \"type\": \"object\",\n      \"description\": \"Settings controlling substitution variable visibility and update permissions.\",\n      \"properties\": {\n        \"showVariables\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether substitution variables are visible to users.\"\n        },\n        \"updateVariables\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether substitution variables can be updated\
  \ by users.\"\n        }\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation link.\",\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Link relation type.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Link URL.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for this link.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Media type of the linked resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-application-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase Application
---
