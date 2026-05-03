---
description: Represents an Oracle Database table as exposed through the ORDS Data Dictionary API, including table metadata, column definitions, and storage properties.
layout: schema
name: Oracle Database Table
properties_list:
- description: Schema owner of the table
  name: owner
  type: string
- description: Name of the table
  name: table_name
  type: string
- description: Tablespace in which the table is stored
  name: tablespace_name
  type: string
- description: Estimated number of rows based on last statistics gathering
  name: num_rows
  type: integer
- description: Timestamp when statistics were last gathered
  name: last_analyzed
  type: string
- description: Status of the table
  name: status
  type: string
- description: Whether the table is a temporary table
  name: temporary
  type: string
- description: Whether the table is partitioned
  name: partitioned
  type: string
- description: Index-organized table type
  name: iot_type
  type:
  - string
  - 'null'
- description: Table compression status
  name: compression
  type: string
- description: Whether logging is enabled
  name: logging
  type: string
- description: List of columns in the table
  name: columns
  type: array
- description: List of indexes on the table
  name: indexes
  type: array
- description: List of constraints on the table
  name: constraints
  type: array
provider_name: Oracle Database
provider_slug: oracle-database
schema_file: json-schema/oracle-database-table.json
slug: oracle-database-table
source_filename: oracle-database-table.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://oracle.com/schemas/database/table.json\",\n  \"title\": \"Oracle Database Table\",\n  \"description\": \"Represents an Oracle Database table as exposed through the ORDS Data Dictionary API, including table metadata, column definitions, and storage properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Schema owner of the table\"\n    },\n    \"table_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the table\"\n    },\n    \"tablespace_name\": {\n      \"type\": \"string\",\n      \"description\": \"Tablespace in which the table is stored\"\n    },\n    \"num_rows\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Estimated number of rows based on last statistics gathering\"\n    },\n    \"last_analyzed\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date-time\",\n      \"description\": \"Timestamp when statistics were last gathered\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the table\",\n      \"enum\": [\"VALID\", \"INVALID\"]\n    },\n    \"temporary\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the table is a temporary table\",\n      \"enum\": [\"Y\", \"N\"]\n    },\n    \"partitioned\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the table is partitioned\",\n      \"enum\": [\"YES\", \"NO\"]\n    },\n    \"iot_type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Index-organized table type\"\n    },\n    \"compression\": {\n      \"type\": \"string\",\n      \"description\": \"Table compression status\",\n      \"enum\": [\"ENABLED\", \"DISABLED\"]\n    },\n    \"logging\": {\n      \"type\": \"string\",\n      \"description\": \"Whether logging is enabled\",\n      \"enum\": [\"YES\", \"NO\"]\n   \
  \ },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"List of columns in the table\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Column\"\n      }\n    },\n    \"indexes\": {\n      \"type\": \"array\",\n      \"description\": \"List of indexes on the table\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Index\"\n      }\n    },\n    \"constraints\": {\n      \"type\": \"array\",\n      \"description\": \"List of constraints on the table\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Constraint\"\n      }\n    }\n  },\n  \"required\": [\"owner\", \"table_name\"],\n  \"$defs\": {\n    \"Column\": {\n      \"type\": \"object\",\n      \"description\": \"A column in an Oracle Database table\",\n      \"properties\": {\n        \"column_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the column\"\n        },\n        \"data_type\": {\n          \"type\": \"string\",\n          \"description\": \"Oracle data type of the\
  \ column\",\n          \"examples\": [\"VARCHAR2\", \"NUMBER\", \"DATE\", \"TIMESTAMP\", \"CLOB\", \"BLOB\", \"JSON\", \"RAW\"]\n        },\n        \"data_length\": {\n          \"type\": \"integer\",\n          \"description\": \"Length of the column in bytes\"\n        },\n        \"data_precision\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Numeric precision for NUMBER columns\"\n        },\n        \"data_scale\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Numeric scale for NUMBER columns\"\n        },\n        \"nullable\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the column allows NULL values\",\n          \"enum\": [\"Y\", \"N\"]\n        },\n        \"column_id\": {\n          \"type\": \"integer\",\n          \"description\": \"Position of the column in the table definition\"\n        },\n        \"default_value\": {\n          \"type\": [\"string\", \"null\"],\n          \"\
  description\": \"Default value expression for the column\"\n        },\n        \"identity_column\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this is an identity column\",\n          \"enum\": [\"YES\", \"NO\"]\n        },\n        \"virtual_column\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this is a virtual (computed) column\",\n          \"enum\": [\"YES\", \"NO\"]\n        }\n      },\n      \"required\": [\"column_name\", \"data_type\"]\n    },\n    \"Index\": {\n      \"type\": \"object\",\n      \"description\": \"An index on an Oracle Database table\",\n      \"properties\": {\n        \"index_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the index\"\n        },\n        \"index_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the index\",\n          \"enum\": [\"NORMAL\", \"BITMAP\", \"FUNCTION-BASED NORMAL\", \"FUNCTION-BASED BITMAP\", \"DOMAIN\"\
  ]\n        },\n        \"uniqueness\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the index enforces uniqueness\",\n          \"enum\": [\"UNIQUE\", \"NONUNIQUE\"]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Status of the index\",\n          \"enum\": [\"VALID\", \"INVALID\", \"UNUSABLE\"]\n        },\n        \"columns\": {\n          \"type\": \"array\",\n          \"description\": \"Columns included in the index\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\"index_name\"]\n    },\n    \"Constraint\": {\n      \"type\": \"object\",\n      \"description\": \"A constraint on an Oracle Database table\",\n      \"properties\": {\n        \"constraint_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the constraint\"\n        },\n        \"constraint_type\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Type of constraint\",\n          \"enum\": [\"P\", \"U\", \"R\", \"C\", \"V\", \"O\"],\n          \"x-enum-descriptions\": {\n            \"P\": \"Primary key\",\n            \"U\": \"Unique key\",\n            \"R\": \"Referential integrity (foreign key)\",\n            \"C\": \"Check constraint\",\n            \"V\": \"With check option on a view\",\n            \"O\": \"With read only on a view\"\n          }\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Enforcement status\",\n          \"enum\": [\"ENABLED\", \"DISABLED\"]\n        },\n        \"r_constraint_name\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Referenced constraint name for foreign keys\"\n        },\n        \"r_owner\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Owner of the referenced constraint\"\n        }\n      },\n      \"required\": [\"constraint_name\", \"constraint_type\"\
  ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/json-schema/oracle-database-table.json
tags:
- Cloud
- Database
- Enterprise
- Oracle
- REST API
- SQL
title: Oracle Database Table
---
