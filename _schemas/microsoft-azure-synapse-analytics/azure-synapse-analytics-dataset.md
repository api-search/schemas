---
description: A dataset resource that represents data structures within linked data stores used in pipelines and data flows.
layout: schema
name: Azure Synapse Analytics Dataset
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: etag
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: microsoft-azure-synapse-analytics
schema_file: json-schema/azure-synapse-analytics-dataset-schema.json
slug: azure-synapse-analytics-dataset
source_filename: azure-synapse-analytics-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-dataset-schema.json\",\n  \"title\": \"Azure Synapse Analytics Dataset\",\n  \"description\": \"A dataset resource that represents data structures within linked data stores used in pipelines and data flows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"required\": [\"type\", \"linkedServiceName\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of dataset.\"\n        },\n        \"description\"\
  : {\n          \"type\": \"string\"\n        },\n        \"linkedServiceName\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"const\": \"LinkedServiceReference\"\n            },\n            \"referenceName\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"object\"\n          }\n        },\n        \"annotations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"folder\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"schema\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"\
  properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"type\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-dataset-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Dataset
---
