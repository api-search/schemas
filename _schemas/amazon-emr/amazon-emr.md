---
description: Represents an Amazon EMR cluster with its associated configuration, state, and metadata.
layout: schema
name: Amazon EMR Cluster
properties_list:
- description: The unique identifier of the cluster
  name: id
  type: string
- description: The name of the cluster
  name: name
  type: string
- description: The current status of the cluster
  name: status
  type: object
- description: The Amazon EMR release label (e.g., emr-6.10.0)
  name: releaseLabel
  type: string
- description: The applications installed on the cluster
  name: applications
  type: array
- description: The instance collection type
  name: instanceCollectionType
  type: string
- description: The S3 path for log storage
  name: logUri
  type: string
- description: Whether the cluster auto-terminates after steps complete
  name: autoTerminate
  type: boolean
- description: Tags associated with the cluster
  name: tags
  type: array
provider_name: Amazon EMR
provider_slug: amazon-emr
schema_file: json-schema/amazon-emr-schema.json
slug: amazon-emr
source_filename: amazon-emr-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/emr/cluster.json\",\n  \"title\": \"Amazon EMR Cluster\",\n  \"description\": \"Represents an Amazon EMR cluster with its associated configuration, state, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cluster\",\n      \"pattern\": \"^j-[A-Z0-9]{13}$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster\"\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"The current status of the cluster\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"STARTING\", \"BOOTSTRAPPING\", \"RUNNING\", \"WAITING\", \"TERMINATING\", \"TERMINATED\", \"TERMINATED_WITH_ERRORS\"\
  ],\n          \"description\": \"The current state of the cluster\"\n        },\n        \"stateChangeReason\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\",\n              \"description\": \"The programmatic code for the state change reason\"\n            },\n            \"message\": {\n              \"type\": \"string\",\n              \"description\": \"The descriptive message for the state change reason\"\n            }\n          }\n        },\n        \"timeline\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"creationDateTime\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            },\n            \"readyDateTime\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            },\n            \"endDateTime\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n         \
  \   }\n          }\n        }\n      }\n    },\n    \"releaseLabel\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon EMR release label (e.g., emr-6.10.0)\"\n    },\n    \"applications\": {\n      \"type\": \"array\",\n      \"description\": \"The applications installed on the cluster\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the application (e.g., Spark, Hadoop, Hive)\"\n          },\n          \"version\": {\n            \"type\": \"string\",\n            \"description\": \"The version of the application\"\n          }\n        }\n      }\n    },\n    \"instanceCollectionType\": {\n      \"type\": \"string\",\n      \"enum\": [\"INSTANCE_FLEET\", \"INSTANCE_GROUP\"],\n      \"description\": \"The instance collection type\"\n    },\n    \"logUri\": {\n      \"type\": \"string\",\n      \"description\": \"The S3 path for log storage\"\
  \n    },\n    \"autoTerminate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster auto-terminates after steps complete\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the cluster\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-emr/refs/heads/main/json-schema/amazon-emr-schema.json
tags:
- Amazon Web Services
- Analytics
- Apache Spark
- Big Data
- Data Processing
- Hadoop
title: Amazon EMR Cluster
---
