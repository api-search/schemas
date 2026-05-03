---
description: An Oracle Essbase database (cube) within an application. Databases contain the multi-dimensional data model with dimensions, members, and data values. Each database has its own outline, scripts, filters, and security configuration.
layout: schema
name: Oracle Essbase Database
properties_list:
- description: Database name. Must not contain spaces.
  name: name
  type: string
- description: Name of the parent application that contains this database.
  name: application
  type: string
- description: User ID of the database owner.
  name: owner
  type: string
- description: Database creation timestamp in milliseconds since Unix epoch.
  name: creationTime
  type: integer
- description: User ID of the person who last modified the database.
  name: modifiedBy
  type: string
- description: Last modification timestamp in milliseconds since Unix epoch.
  name: modifiedTime
  type: integer
- description: Current runtime status of the database.
  name: status
  type: string
- description: Timestamp when the database was last started, in milliseconds since Unix epoch.
  name: startTime
  type: integer
- description: Human-readable description of the database purpose.
  name: description
  type: string
- description: 'Storage type of the database. ASO (Aggregate Storage Option) is optimized for read-heavy analytical queries. BSO (Block Storage Option) is optimized for write-heavy planning and forecasting. CURRENCY '
  name: type
  type: string
- description: The authenticated user's application role for this database.
  name: applicationRole
  type: string
- description: Whether the parent application is managed in EAS Lite (Essbase 21c independent deployment only).
  name: easManagedApp
  type: boolean
- description: Whether the user has permission to start or stop this database.
  name: startStopDBAllowed
  type: boolean
- description: Whether the user has permission to inspect this database.
  name: inspectDBAllowed
  type: boolean
- description: ''
  name: dbVariablesSetting
  type: object
- description: HATEOAS navigation links for related resources.
  name: links
  type: array
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-database-schema.json
slug: oracle-essbase-database
source_filename: oracle-essbase-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-database-schema.json\",\n  \"title\": \"Oracle Essbase Database\",\n  \"description\": \"An Oracle Essbase database (cube) within an application. Databases contain the multi-dimensional data model with dimensions, members, and data values. Each database has its own outline, scripts, filters, and security configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Database name. Must not contain spaces.\"\n    },\n    \"application\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the parent application that contains this database.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the database owner.\"\n    },\n    \"creationTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Database creation timestamp in milliseconds since Unix\
  \ epoch.\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the person who last modified the database.\"\n    },\n    \"modifiedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last modification timestamp in milliseconds since Unix epoch.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current runtime status of the database.\",\n      \"enum\": [\"started\", \"stopped\"]\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp when the database was last started, in milliseconds since Unix epoch.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the database purpose.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Storage type of the database. ASO (Aggregate Storage Option) is optimized for read-heavy analytical queries. BSO (Block Storage Option)\
  \ is optimized for write-heavy planning and forecasting. CURRENCY is for currency conversion databases.\",\n      \"enum\": [\"ASO\", \"BSO\", \"CURRENCY\"]\n    },\n    \"applicationRole\": {\n      \"type\": \"string\",\n      \"description\": \"The authenticated user's application role for this database.\"\n    },\n    \"easManagedApp\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the parent application is managed in EAS Lite (Essbase 21c independent deployment only).\"\n    },\n    \"startStopDBAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has permission to start or stop this database.\"\n    },\n    \"inspectDBAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has permission to inspect this database.\"\n    },\n    \"dbVariablesSetting\": {\n      \"$ref\": \"#/$defs/VariablesSetting\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"HATEOAS navigation links\
  \ for related resources.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"VariablesSetting\": {\n      \"type\": \"object\",\n      \"description\": \"Settings controlling substitution variable visibility and update permissions.\",\n      \"properties\": {\n        \"showVariables\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether substitution variables are visible to users.\"\n        },\n        \"updateVariables\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether substitution variables can be updated by users.\"\n        }\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation link.\",\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Link relation type.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"uri\",\n          \"description\": \"Link URL.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for this link.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Media type of the linked resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-database-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase Database
---
