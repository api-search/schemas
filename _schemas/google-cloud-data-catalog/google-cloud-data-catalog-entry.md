---
description: Represents a data catalog entry, which is a metadata record for a data resource such as a BigQuery table, Pub/Sub topic, or Cloud Storage fileset.
layout: schema
name: Google Cloud Data Catalog Entry
properties_list:
- description: Output only. The resource name of the entry.
  name: name
  type: string
- description: The resource this metadata entry refers to.
  name: linkedResource
  type: string
- description: Fully qualified name of the resource.
  name: fullyQualifiedName
  type: string
- description: The type of the entry.
  name: type
  type: string
- description: Display name of the entry.
  name: displayName
  type: string
- description: Entry description that can include rich text.
  name: description
  type: string
- description: Schema of the entry, such as columns in a table.
  name: schema
  type: object
- description: Timestamps from the underlying source system.
  name: sourceSystemTimestamps
  type: object
- description: Output only. The source system of the entry.
  name: integratedSystem
  type: string
- description: Custom source system that user specified.
  name: userSpecifiedSystem
  type: string
provider_name: Google Cloud Data Catalog
provider_slug: google-cloud-data-catalog
schema_file: json-schema/google-cloud-data-catalog-entry-schema.json
slug: google-cloud-data-catalog-entry
source_filename: google-cloud-data-catalog-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-data-catalog/refs/heads/main/json-schema/google-cloud-data-catalog-entry-schema.json\",\n  \"title\": \"Google Cloud Data Catalog Entry\",\n  \"description\": \"Represents a data catalog entry, which is a metadata record for a data resource such as a BigQuery table, Pub/Sub topic, or Cloud Storage fileset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The resource name of the entry.\"\n    },\n    \"linkedResource\": {\n      \"type\": \"string\",\n      \"description\": \"The resource this metadata entry refers to.\"\n    },\n    \"fullyQualifiedName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified name of the resource.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENTRY_TYPE_UNSPECIFIED\"\
  ,\n        \"TABLE\",\n        \"MODEL\",\n        \"DATA_STREAM\",\n        \"FILESET\",\n        \"CLUSTER\",\n        \"DATABASE\",\n        \"DATA_SOURCE_CONNECTION\",\n        \"ROUTINE\",\n        \"LAKE\",\n        \"ZONE\",\n        \"SERVICE\"\n      ],\n      \"description\": \"The type of the entry.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the entry.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Entry description that can include rich text.\"\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"Schema of the entry, such as columns in a table.\",\n      \"properties\": {\n        \"columns\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"column\": {\n                \"type\": \"string\",\n                \"description\": \"Column name.\"\n         \
  \     },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Type of the column.\"\n              },\n              \"description\": {\n                \"type\": \"string\",\n                \"description\": \"Description of the column.\"\n              },\n              \"mode\": {\n                \"type\": \"string\",\n                \"enum\": [\"MODE_UNSPECIFIED\", \"NULLABLE\", \"REQUIRED\", \"REPEATED\"],\n                \"description\": \"A column mode indicates whether values are required, nullable, or repeated.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"sourceSystemTimestamps\": {\n      \"type\": \"object\",\n      \"description\": \"Timestamps from the underlying source system.\",\n      \"properties\": {\n        \"createTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"updateTime\": {\n          \"type\": \"string\",\n          \"\
  format\": \"date-time\"\n        },\n        \"expireTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"integratedSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The source system of the entry.\"\n    },\n    \"userSpecifiedSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Custom source system that user specified.\"\n    }\n  },\n  \"required\": [\"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-data-catalog/refs/heads/main/json-schema/google-cloud-data-catalog-entry-schema.json
tags:
- Data Catalog
- Data Governance
- Google Cloud
- Metadata
title: Google Cloud Data Catalog Entry
---
