---
description: Represents an Amazon Glue ETL job with its associated configuration, state, and metadata.
layout: schema
name: Amazon Glue Job
properties_list:
- description: The name of the job
  name: name
  type: string
- description: The IAM role associated with the job
  name: role
  type: string
- description: The job command configuration
  name: command
  type: object
- description: The Glue version to use for the job
  name: glueVersion
  type: string
- description: The type of predefined worker
  name: workerType
  type: string
- description: The number of workers allocated
  name: numberOfWorkers
  type: integer
- description: The maximum number of times to retry a failed job
  name: maxRetries
  type: integer
- description: The job timeout in minutes
  name: timeout
  type: integer
- description: The connections used by the job
  name: connections
  type: object
- description: Default arguments for the job
  name: defaultArguments
  type: object
- description: The time the job was created
  name: createdOn
  type: string
- description: The time the job was last modified
  name: lastModifiedOn
  type: string
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/amazon-glue-schema.json
slug: amazon-glue
source_filename: amazon-glue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/glue/job.json\",\n  \"title\": \"Amazon Glue Job\",\n  \"description\": \"Represents an Amazon Glue ETL job with its associated configuration, state, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"role\", \"command\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The IAM role associated with the job\"\n    },\n    \"command\": {\n      \"type\": \"object\",\n      \"description\": \"The job command configuration\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the job command\"\n        },\n        \"scriptLocation\": {\n          \"type\": \"string\",\n          \"description\": \"The S3 location of the script\"\
  \n        },\n        \"pythonVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The Python version being used\"\n        }\n      }\n    },\n    \"glueVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The Glue version to use for the job\"\n    },\n    \"workerType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Standard\", \"G.1X\", \"G.2X\", \"G.025X\"],\n      \"description\": \"The type of predefined worker\"\n    },\n    \"numberOfWorkers\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of workers allocated\"\n    },\n    \"maxRetries\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of times to retry a failed job\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"The job timeout in minutes\"\n    },\n    \"connections\": {\n      \"type\": \"object\",\n      \"description\": \"The connections used by the job\",\n      \"properties\": {\n       \
  \ \"connections\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"defaultArguments\": {\n      \"type\": \"object\",\n      \"description\": \"Default arguments for the job\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the job was created\"\n    },\n    \"lastModifiedOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the job was last modified\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/amazon-glue-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: Amazon Glue Job
---
