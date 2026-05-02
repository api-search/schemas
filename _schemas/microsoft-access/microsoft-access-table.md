---
description: Schema for a Microsoft Access TableDef object as defined in the DAO (Data Access Objects) reference. A TableDef object represents the stored definition of a base table or a linked table, including its fields, indexes, validation rules, and connection properties.
layout: schema
name: Microsoft Access TableDef
properties_list:
- description: The name of the table in the database.
  name: name
  type: string
- description: 'A value that indicates one or more characteristics of the TableDef object. Combines constants: dbAttachExclusive (65536), dbAttachSavePWD (131072), dbSystemObject (2), dbHiddenObject (1), dbAttachedTa'
  name: attributes
  type:
  - integer
  - 'null'
- description: The date and time the table was created. Read-only.
  name: dateCreated
  type:
  - string
  - 'null'
- description: The date and time of the most recent change made to the table definition or its data. Read-only.
  name: lastUpdated
  type:
  - string
  - 'null'
- description: For linked tables, a value that provides information about the source of the linked table, including the database type and path. Empty string for base tables.
  name: connect
  type:
  - string
  - 'null'
- description: For linked tables, the name of the table in the external data source. Empty for base tables.
  name: sourceTableName
  type:
  - string
  - 'null'
- description: The number of records in the TableDef object. For base tables, this reflects the actual count. For linked tables, this is always -1.
  name: recordCount
  type:
  - integer
  - 'null'
- description: A value that indicates whether the table definition can be changed. True if the table structure can be modified. Read-only.
  name: updatable
  type:
  - boolean
  - 'null'
- description: A value that validates the data in a field as it is changed or added to a table. Uses Access SQL expression syntax. Applied at the table level to validate records.
  name: validationRule
  type:
  - string
  - 'null'
- description: A value that specifies the text of the message that the application displays if the value of a field does not satisfy the validation rule.
  name: validationText
  type:
  - string
  - 'null'
- description: The name of a conflict table containing database records that conflicted during replica synchronization. Read-only. Empty string if no conflicts exist.
  name: conflictTable
  type:
  - string
  - 'null'
- description: A value that indicates which subset of records is replicated to that table from a full replica. Can be a Boolean (True for all records) or a filter expression string.
  name: replicaFilter
  type:
  - string
  - boolean
  - 'null'
- description: A collection of all Field objects in the TableDef. Each Field represents a column of data with a common data type and common set of properties.
  name: fields
  type:
  - array
  - 'null'
- description: A collection of all Index objects defined for the table. Indexes specify the order of records and whether duplicate records are accepted.
  name: indexes
  type:
  - array
  - 'null'
provider_name: Microsoft Access
provider_slug: microsoft-access
schema_file: json-schema/microsoft-access-table-schema.json
slug: microsoft-access-table
source_filename: microsoft-access-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/office/client-developer/access/desktop-database-reference/tabledef-object-dao\",\n  \"title\": \"Microsoft Access TableDef\",\n  \"description\": \"Schema for a Microsoft Access TableDef object as defined in the DAO (Data Access Objects) reference. A TableDef object represents the stored definition of a base table or a linked table, including its fields, indexes, validation rules, and connection properties.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table in the database.\",\n      \"minLength\": 1,\n      \"maxLength\": 64,\n      \"examples\": [\"Customers\", \"Orders\", \"Products\", \"Employees\"]\n    },\n    \"attributes\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"A value that indicates one or more characteristics\
  \ of the TableDef object. Combines constants: dbAttachExclusive (65536), dbAttachSavePWD (131072), dbSystemObject (2), dbHiddenObject (1), dbAttachedTable (1073741824), dbAttachedODBC (536870912).\",\n      \"examples\": [0, 1073741824, 536870912]\n    },\n    \"dateCreated\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the table was created. Read-only.\",\n      \"examples\": [\"2024-01-15T09:00:00Z\"]\n    },\n    \"lastUpdated\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the most recent change made to the table definition or its data. Read-only.\",\n      \"examples\": [\"2024-06-20T14:30:00Z\"]\n    },\n    \"connect\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"For linked tables, a value that provides information about the source of the linked table, including the database type and path. Empty string\
  \ for base tables.\",\n      \"examples\": [\n        \"\",\n        \";DATABASE=C:\\\\Data\\\\External.accdb\",\n        \"ODBC;DSN=MyServer;DATABASE=pubs;\"\n      ]\n    },\n    \"sourceTableName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"For linked tables, the name of the table in the external data source. Empty for base tables.\",\n      \"examples\": [\"\", \"dbo.Customers\"]\n    },\n    \"recordCount\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The number of records in the TableDef object. For base tables, this reflects the actual count. For linked tables, this is always -1.\",\n      \"minimum\": -1,\n      \"examples\": [0, 100, 5000, -1]\n    },\n    \"updatable\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"A value that indicates whether the table definition can be changed. True if the table structure can be modified. Read-only.\"\n    },\n    \"validationRule\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"A value that validates the data in a field as it is changed or added to a table. Uses Access SQL expression syntax. Applied at the table level to validate records.\",\n      \"examples\": [\n        \"[EndDate] >= [StartDate]\",\n        \"[Quantity] > 0\",\n        \"[Price] >= 0 AND [Price] <= 10000\"\n      ]\n    },\n    \"validationText\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A value that specifies the text of the message that the application displays if the value of a field does not satisfy the validation rule.\",\n      \"examples\": [\n        \"End date must be on or after the start date.\",\n        \"Quantity must be greater than zero.\"\n      ]\n    },\n    \"conflictTable\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The name of a conflict table containing database records that conflicted during replica synchronization. Read-only. Empty string if no conflicts exist.\"\n    },\n\
  \    \"replicaFilter\": {\n      \"type\": [\"string\", \"boolean\", \"null\"],\n      \"description\": \"A value that indicates which subset of records is replicated to that table from a full replica. Can be a Boolean (True for all records) or a filter expression string.\"\n    },\n    \"fields\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"A collection of all Field objects in the TableDef. Each Field represents a column of data with a common data type and common set of properties.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Field\"\n      }\n    },\n    \"indexes\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"A collection of all Index objects defined for the table. Indexes specify the order of records and whether duplicate records are accepted.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Index\"\n      }\n    }\n  },\n  \"additionalProperties\": true,\n  \"$defs\": {\n    \"Field\": {\n      \"type\": \"object\",\n     \
  \ \"description\": \"A Field object represents a column of data with a common data type and a common set of properties. Corresponds to the DAO Field object within a TableDef's Fields collection.\",\n      \"required\": [\"name\", \"type\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the field. Must be unique within the Fields collection.\",\n          \"minLength\": 1,\n          \"maxLength\": 64,\n          \"examples\": [\"CustomerID\", \"FirstName\", \"OrderDate\", \"UnitPrice\"]\n        },\n        \"type\": {\n          \"type\": \"integer\",\n          \"description\": \"A value that indicates the data type of the field. DAO type constants: dbBoolean (1), dbByte (2), dbInteger (3), dbLong (4), dbCurrency (5), dbSingle (6), dbDouble (7), dbDate (8), dbBinary (9), dbText (10), dbLongBinary (11 - OLE Object), dbMemo (12), dbGUID (15), dbBigInt (16), dbVarBinary (17), dbChar (18), dbNumeric (19), dbFloat\
  \ (21), dbTime (22), dbTimeStamp (23), dbAttachment (101), dbComplexByte (102), dbComplexInteger (103), dbComplexLong (104), dbComplexSingle (105), dbComplexDouble (106), dbComplexGUID (107), dbComplexDecimal (108), dbComplexText (109).\",\n          \"examples\": [1, 3, 4, 7, 8, 10, 12]\n        },\n        \"size\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"A value that indicates the maximum size, in bytes, of a Field object. For Text fields, this is the maximum number of characters (up to 255). For numeric and fixed-width fields, the size is determined by the type.\",\n          \"minimum\": 0,\n          \"maximum\": 255,\n          \"examples\": [50, 100, 255]\n        },\n        \"attributes\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"A value that indicates characteristics of the field. Combines constants: dbAutoIncrField (16 - AutoNumber), dbDescending (1 - descending sort in index), dbFixedField (1 - fixed\
  \ size), dbHyperlinkField (32768 - hyperlink), dbSystemField (8192 - system field), dbUpdatableField (32 - updatable), dbVariableField (2 - variable size).\",\n          \"examples\": [0, 16, 32768]\n        },\n        \"ordinalPosition\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The relative position of the field within the Fields collection. Determines the default column order.\",\n          \"minimum\": 0,\n          \"examples\": [0, 1, 2, 3]\n        },\n        \"required\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether the field requires a non-Null value. If True, no Null values are allowed.\"\n        },\n        \"allowZeroLength\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether a zero-length string is a valid setting for the Value property of a Text or Memo field.\"\n        },\n        \"defaultValue\": {\n       \
  \   \"type\": [\"string\", \"null\"],\n          \"description\": \"The default value of the field. Automatically assigned to new records if no value is specified.\",\n          \"examples\": [\"0\", \"Date()\", \"\\\"Unknown\\\"\", \"True\"]\n        },\n        \"validationRule\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"An expression that validates the data entered in the field. Uses Access SQL expression syntax.\",\n          \"examples\": [\n            \">0\",\n            \"Like \\\"[A-Z]*\\\"\",\n            \"Between 1 And 100\",\n            \"Is Not Null\"\n          ]\n        },\n        \"validationText\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The text of the error message displayed when the value entered does not satisfy the validation rule.\",\n          \"examples\": [\"Value must be greater than zero.\", \"Please enter a valid entry.\"]\n        },\n        \"validateOnSet\": {\n          \"type\"\
  : [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether the value of the field is immediately validated when set. Primarily used for Memo and Long Binary fields.\"\n        },\n        \"collatingOrder\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"A value that specifies the sequence of the sort order in text for string comparison or sorting.\"\n        },\n        \"foreignName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"A value that specifies the name of the Field object in a foreign table that corresponds to a field in a primary table. Used in Relation objects.\"\n        },\n        \"sourceField\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The name of the field in the original source of data. Read-only.\"\n        },\n        \"sourceTable\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The name of the table that is\
  \ the original source of data. Read-only.\"\n        },\n        \"dataUpdatable\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether the data in the field can be updated. Read-only.\"\n        },\n        \"fieldSize\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The number of bytes used in the database for a Memo or Long Binary (OLE Object) field. Read-only.\",\n          \"minimum\": 0\n        },\n        \"expression\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"For calculated fields (Access 2010+), the expression that defines the calculated value.\",\n          \"examples\": [\"[FirstName] & \\\" \\\" & [LastName]\", \"[Quantity] * [UnitPrice]\"]\n        }\n      }\n    },\n    \"Index\": {\n      \"type\": \"object\",\n      \"description\": \"An Index object specifies the order of records accessed from database tables and whether duplicate records are\
  \ accepted. Corresponds to the DAO Index object within a TableDef's Indexes collection.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the index.\",\n          \"examples\": [\"PrimaryKey\", \"CustomerNameIndex\", \"OrderDateIndex\"]\n        },\n        \"primary\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether the index represents the primary key for the table. Only one index per table can be the primary key.\"\n        },\n        \"unique\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether the index requires unique values. If True, no duplicate values are allowed in the indexed fields.\"\n        },\n        \"required\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether all fields in the index\
  \ require non-Null values.\"\n        },\n        \"ignoreNulls\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether records with Null values in their index fields have index entries. If True, records with Null index values are excluded from the index.\"\n        },\n        \"foreign\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether the index is a foreign key index, automatically created by the database engine when a relationship is established. Read-only.\"\n        },\n        \"clustered\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"A value that indicates whether the index is a clustered index. Not supported by the Microsoft Access database engine; ignored for Access databases.\"\n        },\n        \"distinctCount\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The number of unique values for the\
  \ index that are included in the associated table. Read-only.\",\n          \"minimum\": 0\n        },\n        \"fields\": {\n          \"type\": [\"array\", \"null\"],\n          \"description\": \"A collection of Field objects that make up the index. The order of fields determines the sort hierarchy.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The name of the field included in the index.\"\n              },\n              \"attributes\": {\n                \"type\": [\"integer\", \"null\"],\n                \"description\": \"Attributes of the field within the index. Use dbDescending (1) for descending sort order.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-access/refs/heads/main/json-schema/microsoft-access-table-schema.json
tags:
- Access Database
- Database
- Desktop Database
- Microsoft
- Relational Database
title: Microsoft Access TableDef
---
