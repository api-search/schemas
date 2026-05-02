---
description: A notebook resource for interactive data exploration supporting Python, Scala, SQL, and .NET languages.
layout: schema
name: Azure Synapse Analytics Notebook
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
schema_file: json-schema/azure-synapse-analytics-notebook-schema.json
slug: azure-synapse-analytics-notebook
source_filename: azure-synapse-analytics-notebook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-notebook-schema.json\",\n  \"title\": \"Azure Synapse Analytics Notebook\",\n  \"description\": \"A notebook resource for interactive data exploration supporting Python, Scala, SQL, and .NET languages.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"nbformat\": {\n          \"type\": \"integer\",\n          \"description\": \"Notebook format major version number.\"\
  \n        },\n        \"nbformat_minor\": {\n          \"type\": \"integer\",\n          \"description\": \"Notebook format minor version number.\"\n        },\n        \"bigDataPool\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"referenceName\": {\n              \"type\": \"string\"\n            },\n            \"type\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"sessionProperties\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"driverMemory\": {\n              \"type\": \"string\"\n            },\n            \"driverCores\": {\n              \"type\": \"integer\"\n            },\n            \"executorMemory\": {\n              \"type\": \"string\"\n            },\n            \"executorCores\": {\n              \"type\": \"integer\"\n            },\n            \"numExecutors\": {\n              \"type\": \"integer\"\n            }\n          }\n        },\n        \"metadata\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"kernelspec\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                },\n                \"display_name\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"language_info\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        },\n        \"cells\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/NotebookCell\"\n          }\n        },\n        \"folder\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\"\
  : {\n    \"NotebookCell\": {\n      \"type\": \"object\",\n      \"description\": \"A notebook cell.\",\n      \"properties\": {\n        \"cell_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of cell (code, markdown).\"\n        },\n        \"source\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Contents of the cell.\"\n        },\n        \"metadata\": {\n          \"type\": \"object\"\n        },\n        \"outputs\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-notebook-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Notebook
---
