---
description: Schema for a Microsoft Access Database object as defined in the DAO (Data Access Objects) reference. A Database object represents an open Access database (.accdb or .mdb) and provides methods and properties to manipulate its structure and data, including tables, queries, relations, and containers.
layout: schema
name: Microsoft Access Database
properties_list:
- description: The name and path of the database file. For a Microsoft Access database, this is the full file path to the .accdb or .mdb file.
  name: name
  type: string
- description: The version of the Microsoft Access database engine that created the database. Returns a four-character string representing the engine version number.
  name: version
  type:
  - string
  - 'null'
- description: A value that specifies the sequence of the sort order in text for string comparison or sorting. Corresponds to locale-specific collation constants such as dbLangGeneral.
  name: collatingOrder
  type:
  - integer
  - 'null'
- description: A value that provides information about the source of an open database, a database used in a pass-through query, or a linked table. Contains the connection string for ODBC or external data sources.
  name: connect
  type:
  - string
  - 'null'
- description: A value that specifies the number of seconds to wait before a timeout error occurs when a query is executed on an ODBC data source.
  name: queryTimeout
  type:
  - integer
  - 'null'
- description: The number of records affected by the most recently invoked Execute method. Read-only.
  name: recordsAffected
  type:
  - integer
  - 'null'
- description: A value that indicates whether changes can be made to the database. True if the database can be modified; False if it is read-only. Read-only.
  name: updatable
  type:
  - boolean
  - 'null'
- description: A value that indicates whether the database supports transactions (BeginTrans, CommitTrans, and Rollback). Read-only.
  name: transactions
  type:
  - boolean
  - 'null'
- description: A 16-byte value that uniquely identifies the Design Master in a replica set. Used in database replication scenarios.
  name: designMasterID
  type:
  - string
  - 'null'
- description: A 16-byte value that uniquely identifies a database replica. Read-only.
  name: replicaID
  type:
  - string
  - 'null'
- description: A collection of all stored TableDef objects in the database. Each TableDef represents the definition of a base table or linked table.
  name: tableDefs
  type:
  - array
  - 'null'
- description: A collection of all stored QueryDef objects in the database. Each QueryDef represents the definition of a saved query.
  name: queryDefs
  type:
  - array
  - 'null'
- description: A collection of all stored Relation objects in the database. Each Relation defines a relationship between fields in tables.
  name: relations
  type:
  - array
  - 'null'
- description: A collection of all Container objects in the database. Containers store information about database objects such as forms, reports, tables, and modules for security purposes.
  name: containers
  type:
  - array
  - 'null'
provider_name: Microsoft Access
provider_slug: microsoft-access
schema_file: json-schema/microsoft-access-database-schema.json
slug: microsoft-access-database
source_filename: microsoft-access-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/office/client-developer/access/desktop-database-reference/database-object-dao\",\n  \"title\": \"Microsoft Access Database\",\n  \"description\": \"Schema for a Microsoft Access Database object as defined in the DAO (Data Access Objects) reference. A Database object represents an open Access database (.accdb or .mdb) and provides methods and properties to manipulate its structure and data, including tables, queries, relations, and containers.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name and path of the database file. For a Microsoft Access database, this is the full file path to the .accdb or .mdb file.\",\n      \"examples\": [\"C:\\\\Databases\\\\Northwind.accdb\", \"Northwind.mdb\"]\n    },\n    \"version\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"description\": \"The version of the Microsoft Access database engine that created the database. Returns a four-character string representing the engine version number.\",\n      \"examples\": [\"4.0\", \"3.0\"]\n    },\n    \"collatingOrder\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"A value that specifies the sequence of the sort order in text for string comparison or sorting. Corresponds to locale-specific collation constants such as dbLangGeneral.\",\n      \"examples\": [1024]\n    },\n    \"connect\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A value that provides information about the source of an open database, a database used in a pass-through query, or a linked table. Contains the connection string for ODBC or external data sources.\",\n      \"examples\": [\"ODBC;DSN=MyServer;DATABASE=pubs;\", \"\"]\n    },\n    \"queryTimeout\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"A value that\
  \ specifies the number of seconds to wait before a timeout error occurs when a query is executed on an ODBC data source.\",\n      \"minimum\": 0,\n      \"default\": 60,\n      \"examples\": [60, 120]\n    },\n    \"recordsAffected\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The number of records affected by the most recently invoked Execute method. Read-only.\",\n      \"minimum\": 0\n    },\n    \"updatable\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"A value that indicates whether changes can be made to the database. True if the database can be modified; False if it is read-only. Read-only.\"\n    },\n    \"transactions\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"A value that indicates whether the database supports transactions (BeginTrans, CommitTrans, and Rollback). Read-only.\"\n    },\n    \"designMasterID\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A 16-byte value\
  \ that uniquely identifies the Design Master in a replica set. Used in database replication scenarios.\",\n      \"examples\": [\"{2E5FE6A0-E199-11CD-BC4C-00AA003C157A}\"]\n    },\n    \"replicaID\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A 16-byte value that uniquely identifies a database replica. Read-only.\",\n      \"examples\": [\"{8A0C7F3B-4E12-4B8D-9D3A-1C2E5F6A7B8C}\"]\n    },\n    \"tableDefs\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"A collection of all stored TableDef objects in the database. Each TableDef represents the definition of a base table or linked table.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TableDefSummary\"\n      }\n    },\n    \"queryDefs\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"A collection of all stored QueryDef objects in the database. Each QueryDef represents the definition of a saved query.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/QueryDef\"\n \
  \     }\n    },\n    \"relations\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"A collection of all stored Relation objects in the database. Each Relation defines a relationship between fields in tables.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Relation\"\n      }\n    },\n    \"containers\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"A collection of all Container objects in the database. Containers store information about database objects such as forms, reports, tables, and modules for security purposes.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Container\"\n      }\n    }\n  },\n  \"additionalProperties\": true,\n  \"$defs\": {\n    \"TableDefSummary\": {\n      \"type\": \"object\",\n      \"description\": \"A summary representation of a TableDef object within the Database's TableDefs collection.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n  \
  \        \"description\": \"The name of the table.\",\n          \"examples\": [\"Customers\", \"Orders\", \"Products\"]\n        },\n        \"attributes\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"A value that indicates one or more characteristics of the TableDef object. Combines constants such as dbAttachExclusive, dbAttachSavePWD, dbSystemObject, dbHiddenObject, and dbAttachedTable.\",\n          \"examples\": [0, 1073741824]\n        },\n        \"dateCreated\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the table was created. Read-only.\",\n          \"examples\": [\"2024-01-15T09:00:00Z\"]\n        },\n        \"lastUpdated\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The date and time of the most recent change made to the table. Read-only.\",\n          \"examples\": [\"2024-06-20T14:30:00Z\"\
  ]\n        },\n        \"recordCount\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The number of records in the table. For linked tables, this value is always -1.\",\n          \"minimum\": -1\n        },\n        \"sourceTableName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"For linked tables, the name of the source table in the external data source. Empty for base tables.\"\n        },\n        \"connect\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"For linked tables, the connection string to the external data source. Empty for base tables.\"\n        }\n      }\n    },\n    \"QueryDef\": {\n      \"type\": \"object\",\n      \"description\": \"A QueryDef object represents a saved query definition in the database. Contains the SQL statement and metadata for the query.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"The name of the query.\",\n          \"examples\": [\"qryCustomerOrders\", \"qryProductSales\"]\n        },\n        \"type\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"A value that indicates the type of query, such as select (0), crosstab (16), delete (32), update (48), append (64), make-table (80), DDL (96), SQL pass-through (112), union (128), or bulk (144).\",\n          \"enum\": [0, 16, 32, 48, 64, 80, 96, 112, 128, 144, null]\n        },\n        \"sql\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The SQL statement that defines the query.\",\n          \"examples\": [\"SELECT * FROM Customers WHERE Country = 'USA'\"]\n        },\n        \"dateCreated\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the query was created. Read-only.\"\n        },\n        \"lastUpdated\": {\n          \"type\":\
  \ [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The date and time of the most recent change to the query. Read-only.\"\n        },\n        \"updatable\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"Whether the query definition can be changed.\"\n        },\n        \"connect\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The connection string for a pass-through query.\"\n        },\n        \"returnsRecords\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"For SQL pass-through queries, whether the query returns records.\"\n        }\n      }\n    },\n    \"Relation\": {\n      \"type\": \"object\",\n      \"description\": \"A Relation object represents a relationship between fields in tables or queries. Used to enforce referential integrity between a primary table and a foreign table.\",\n      \"required\": [\"name\", \"table\", \"foreignTable\"\
  ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the relationship.\",\n          \"examples\": [\"CategoriesProducts\", \"CustomersOrders\"]\n        },\n        \"table\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the primary (referenced) table in the relationship.\",\n          \"examples\": [\"Categories\", \"Customers\"]\n        },\n        \"foreignTable\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the foreign (referencing) table in the relationship.\",\n          \"examples\": [\"Products\", \"Orders\"]\n        },\n        \"attributes\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"A value that indicates the relationship type and enforcement rules. Combines constants: dbRelationUnique (1), dbRelationDontEnforce (2), dbRelationInherited (4), dbRelationUpdateCascade (256), dbRelationDeleteCascade (4096),\
  \ dbRelationLeft (16777216), dbRelationRight (33554432).\",\n          \"examples\": [0, 256, 4096, 4352]\n        },\n        \"fields\": {\n          \"type\": [\"array\", \"null\"],\n          \"description\": \"The fields involved in the relationship, mapping primary key fields to foreign key fields.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The name of the field in the primary table.\"\n              },\n              \"foreignName\": {\n                \"type\": \"string\",\n                \"description\": \"The name of the corresponding field in the foreign table.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"Container\": {\n      \"type\": \"object\",\n      \"description\": \"A Container object groups similar types of Document objects for security and access control. Built-in containers include\
  \ Databases, Tables, and Relations.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the container.\",\n          \"examples\": [\"Databases\", \"Tables\", \"Relations\", \"Forms\", \"Reports\", \"Scripts\", \"Modules\"]\n        },\n        \"owner\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The owner of the container.\"\n        },\n        \"permissions\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The permissions for the container.\"\n        },\n        \"documents\": {\n          \"type\": [\"array\", \"null\"],\n          \"description\": \"The documents within this container.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The name of the document.\"\n              },\n              \"owner\"\
  : {\n                \"type\": [\"string\", \"null\"],\n                \"description\": \"The owner of the document.\"\n              },\n              \"dateCreated\": {\n                \"type\": [\"string\", \"null\"],\n                \"format\": \"date-time\",\n                \"description\": \"When the document was created.\"\n              },\n              \"lastUpdated\": {\n                \"type\": [\"string\", \"null\"],\n                \"format\": \"date-time\",\n                \"description\": \"When the document was last modified.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-access/refs/heads/main/json-schema/microsoft-access-database-schema.json
tags:
- Access Database
- Database
- Desktop Database
- Microsoft
- Relational Database
title: Microsoft Access Database
---
