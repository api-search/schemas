---
description: Metadata describing a Dataflow template, including its name, description, parameters, and streaming capability. Templates define reusable pipeline structures that can be launched with different runtime parameters.
layout: schema
name: Google Cloud Dataflow Template
properties_list:
- description: Required. The name of the template.
  name: name
  type: string
- description: Optional. A description of the template.
  name: description
  type: string
- description: The parameters for the template, defining inputs that can be configured at launch time.
  name: parameters
  type: array
- description: If true, this template processes unbounded data streams.
  name: streaming
  type: boolean
- description: If true, this template supports at-least-once processing.
  name: supportsAtLeastOnce
  type: boolean
- description: If true, this template supports exactly-once processing.
  name: supportsExactlyOnce
  type: boolean
- description: The default streaming mode for the template.
  name: defaultStreamingMode
  type: string
- description: The type of the template.
  name: templateType
  type: string
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
schema_file: json-schema/google-cloud-dataflow-template-schema.json
slug: google-cloud-dataflow-template
source_filename: google-cloud-dataflow-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/google-cloud-dataflow/json-schema/google-cloud-dataflow-template-schema.json\",\n  \"title\": \"Google Cloud Dataflow Template\",\n  \"description\": \"Metadata describing a Dataflow template, including its name, description, parameters, and streaming capability. Templates define reusable pipeline structures that can be launched with different runtime parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Required. The name of the template.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional. A description of the template.\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"The parameters for the template, defining inputs that can be configured at launch time.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ParameterMetadata\"\
  \n      }\n    },\n    \"streaming\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, this template processes unbounded data streams.\"\n    },\n    \"supportsAtLeastOnce\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, this template supports at-least-once processing.\"\n    },\n    \"supportsExactlyOnce\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, this template supports exactly-once processing.\"\n    },\n    \"defaultStreamingMode\": {\n      \"type\": \"string\",\n      \"description\": \"The default streaming mode for the template.\"\n    },\n    \"templateType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the template.\",\n      \"enum\": [\n        \"UNKNOWN\",\n        \"LEGACY\",\n        \"FLEX\"\n      ]\n    }\n  },\n  \"required\": [\"name\"],\n  \"$defs\": {\n    \"ParameterMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata for a specific parameter used by\
  \ a template.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Required. The name of the parameter.\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"Required. The label to display for the parameter.\"\n        },\n        \"helpText\": {\n          \"type\": \"string\",\n          \"description\": \"Required. Help text to display for the parameter.\"\n        },\n        \"isOptional\": {\n          \"type\": \"boolean\",\n          \"description\": \"Optional. Whether the parameter is optional. Defaults to false.\"\n        },\n        \"regexes\": {\n          \"type\": \"array\",\n          \"description\": \"Optional. Regular expressions used to validate the parameter value.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"paramType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of the parameter.\"\
  ,\n          \"enum\": [\n            \"DEFAULT\",\n            \"TEXT\",\n            \"GCS_READ_BUCKET\",\n            \"GCS_WRITE_BUCKET\",\n            \"GCS_READ_FILE\",\n            \"GCS_WRITE_FILE\",\n            \"GCS_READ_FOLDER\",\n            \"GCS_WRITE_FOLDER\",\n            \"PUBSUB_TOPIC\",\n            \"PUBSUB_SUBSCRIPTION\",\n            \"BIGQUERY_TABLE\",\n            \"JAVASCRIPT_UDF_FILE\",\n            \"SERVICE_ACCOUNT\",\n            \"MACHINE_TYPE\",\n            \"KMS_KEY_NAME\",\n            \"WORKER_REGION\",\n            \"WORKER_ZONE\",\n            \"BOOLEAN\",\n            \"ENUM\",\n            \"NUMBER\",\n            \"KAFKA_TOPIC\",\n            \"KAFKA_READ_TOPIC\",\n            \"KAFKA_WRITE_TOPIC\"\n          ]\n        }\n      },\n      \"required\": [\"name\", \"label\", \"helpText\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/json-schema/google-cloud-dataflow-template-schema.json
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
title: Google Cloud Dataflow Template
---
