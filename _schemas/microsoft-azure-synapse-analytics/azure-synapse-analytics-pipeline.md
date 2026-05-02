---
description: A data integration pipeline resource that orchestrates data movement and transformation activities.
layout: schema
name: Azure Synapse Analytics Pipeline
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
schema_file: json-schema/azure-synapse-analytics-pipeline-schema.json
slug: azure-synapse-analytics-pipeline
source_filename: azure-synapse-analytics-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-pipeline-schema.json\",\n  \"title\": \"Azure Synapse Analytics Pipeline\",\n  \"description\": \"A data integration pipeline resource that orchestrates data movement and transformation activities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the pipeline.\"\n        },\n        \"activities\": {\n          \"type\": \"array\",\n  \
  \        \"items\": {\n            \"$ref\": \"#/$defs/Activity\"\n          },\n          \"description\": \"List of activities in the pipeline.\"\n        },\n        \"parameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/ParameterSpecification\"\n          },\n          \"description\": \"List of parameters for pipeline.\"\n        },\n        \"variables\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/VariableSpecification\"\n          },\n          \"description\": \"List of variables for pipeline.\"\n        },\n        \"concurrency\": {\n          \"type\": \"integer\",\n          \"description\": \"The max number of concurrent runs for the pipeline.\"\n        },\n        \"annotations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"folder\": {\n          \"type\": \"\
  object\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The name of the folder that this Pipeline is in.\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"Activity\": {\n      \"type\": \"object\",\n      \"description\": \"A pipeline activity.\",\n      \"required\": [\"name\", \"type\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Activity name.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of activity.\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"dependsOn\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"activity\": {\n                \"type\": \"string\"\n              },\n              \"dependencyConditions\"\
  : {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\",\n                  \"enum\": [\"Succeeded\", \"Failed\", \"Skipped\", \"Completed\"]\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"ParameterSpecification\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"Object\", \"String\", \"Int\", \"Float\", \"Bool\", \"Array\", \"SecureString\"]\n        },\n        \"defaultValue\": {\n          \"description\": \"Default value of the parameter.\"\n        }\n      }\n    },\n    \"VariableSpecification\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"String\", \"Bool\", \"Array\"]\n        },\n        \"defaultValue\": {\n          \"description\": \"Default value of the variable.\"\n        }\n      }\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-pipeline-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Pipeline
---
