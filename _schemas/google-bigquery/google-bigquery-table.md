---
description: Schema representing a BigQuery table resource, including its structure, metadata, and configuration.
layout: schema
name: Google BigQuery Table
properties_list:
- description: The resource type, always bigquery#table
  name: kind
  type: string
- description: The fully-qualified unique name of the table in the format projectId:datasetId.tableId
  name: id
  type: string
- description: Reference describing the ID of this table
  name: tableReference
  type: object
- description: A descriptive name for this table
  name: friendlyName
  type: string
- description: A user-friendly description of this table
  name: description
  type: string
- description: Describes the schema of this table
  name: schema
  type: object
- description: The number of rows of data in this table
  name: numRows
  type: string
- description: The size of this table in bytes, excluding any data in the streaming buffer
  name: numBytes
  type: string
- description: Describes the table type
  name: type
  type: string
- description: The geographic location where the table resides
  name: location
  type: string
- description: The labels associated with this table
  name: labels
  type: object
- description: The time when this table was created, in milliseconds since the epoch
  name: creationTime
  type: string
- description: The time when this table expires, in milliseconds since the epoch
  name: expirationTime
  type: string
- description: The time when this table was last modified, in milliseconds since the epoch
  name: lastModifiedTime
  type: string
provider_name: Google BigQuery
provider_slug: google-bigquery
schema_file: json-schema/google-bigquery-table-schema.json
slug: google-bigquery-table
source_filename: google-bigquery-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/bigquery/table.json\",\n  \"title\": \"Google BigQuery Table\",\n  \"description\": \"Schema representing a BigQuery table resource, including its structure, metadata, and configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type, always bigquery#table\",\n      \"const\": \"bigquery#table\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The fully-qualified unique name of the table in the format projectId:datasetId.tableId\"\n    },\n    \"tableReference\": {\n      \"$ref\": \"#/$defs/TableReference\",\n      \"description\": \"Reference describing the ID of this table\"\n    },\n    \"friendlyName\": {\n      \"type\": \"string\",\n      \"description\": \"A descriptive name for this table\",\n      \"maxLength\": 1024\n    },\n    \"\
  description\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly description of this table\"\n    },\n    \"schema\": {\n      \"$ref\": \"#/$defs/TableSchema\",\n      \"description\": \"Describes the schema of this table\"\n    },\n    \"numRows\": {\n      \"type\": \"string\",\n      \"description\": \"The number of rows of data in this table\"\n    },\n    \"numBytes\": {\n      \"type\": \"string\",\n      \"description\": \"The size of this table in bytes, excluding any data in the streaming buffer\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Describes the table type\",\n      \"enum\": [\"TABLE\", \"VIEW\", \"MATERIALIZED_VIEW\", \"EXTERNAL\", \"SNAPSHOT\"]\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geographic location where the table resides\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"The labels associated with this table\",\n      \"\
  additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time when this table was created, in milliseconds since the epoch\"\n    },\n    \"expirationTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time when this table expires, in milliseconds since the epoch\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time when this table was last modified, in milliseconds since the epoch\"\n    }\n  },\n  \"$defs\": {\n    \"TableReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference uniquely identifying a BigQuery table\",\n      \"required\": [\"projectId\", \"datasetId\", \"tableId\"],\n      \"properties\": {\n        \"projectId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the project containing this table\"\n        },\n        \"datasetId\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The ID of the dataset containing this table\"\n        },\n        \"tableId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the table\"\n        }\n      }\n    },\n    \"TableSchema\": {\n      \"type\": \"object\",\n      \"description\": \"Schema of a BigQuery table\",\n      \"properties\": {\n        \"fields\": {\n          \"type\": \"array\",\n          \"description\": \"Describes the fields in a table\",\n          \"items\": {\n            \"$ref\": \"#/$defs/TableFieldSchema\"\n          }\n        }\n      }\n    },\n    \"TableFieldSchema\": {\n      \"type\": \"object\",\n      \"description\": \"A field in a BigQuery table schema\",\n      \"required\": [\"name\", \"type\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The field name, must be unique within the table schema\"\n        },\n        \"type\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The field data type\",\n          \"enum\": [\"STRING\", \"BYTES\", \"INTEGER\", \"INT64\", \"FLOAT\", \"FLOAT64\", \"NUMERIC\", \"BIGNUMERIC\", \"BOOLEAN\", \"BOOL\", \"TIMESTAMP\", \"DATE\", \"TIME\", \"DATETIME\", \"GEOGRAPHY\", \"RECORD\", \"STRUCT\", \"JSON\", \"RANGE\"]\n        },\n        \"mode\": {\n          \"type\": \"string\",\n          \"description\": \"The field mode\",\n          \"enum\": [\"NULLABLE\", \"REQUIRED\", \"REPEATED\"],\n          \"default\": \"NULLABLE\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The field description\"\n        },\n        \"fields\": {\n          \"type\": \"array\",\n          \"description\": \"Describes the nested schema fields if the type is RECORD\",\n          \"items\": {\n            \"$ref\": \"#/$defs/TableFieldSchema\"\n          }\n        },\n        \"policyTags\": {\n          \"type\": \"object\",\n          \"description\": \"\
  Policy tags attached to this field for column-level security\",\n          \"properties\": {\n            \"names\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"A list of policy tag resource names\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-bigquery/refs/heads/main/json-schema/google-bigquery-table-schema.json
tags:
- Analytics
- Big Data
- Cloud
- Data Warehouse
- Serverless
- SQL
title: Google BigQuery Table
---
