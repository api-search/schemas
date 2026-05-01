---
description: Represents a Data Fusion instance, which is a managed environment for building and running data integration pipelines.
layout: schema
name: Google Cloud Data Fusion Instance
properties_list:
- description: Output only. The name of this instance in the format projects/{project}/locations/{location}/instances/{instance}.
  name: name
  type: string
- description: A description of this instance.
  name: description
  type: string
- description: The type of the Data Fusion instance.
  name: type
  type: string
- description: Option to enable Stackdriver Logging.
  name: enableStackdriverLogging
  type: boolean
- description: Option to enable Stackdriver Monitoring.
  name: enableStackdriverMonitoring
  type: boolean
- description: Specifies whether the Data Fusion instance should be private.
  name: privateInstance
  type: boolean
- description: Network configuration options for a private instance.
  name: networkConfig
  type: object
- description: The resource labels for instance to use to annotate any related underlying resources.
  name: labels
  type: object
- description: Map of additional options used to configure the behavior of Data Fusion instance.
  name: options
  type: object
- description: Output only. The time the instance was created.
  name: createTime
  type: string
- description: Output only. The time the instance was last updated.
  name: updateTime
  type: string
- description: Output only. The current state of this Data Fusion instance.
  name: state
  type: string
- description: Output only. Endpoint on which the Data Fusion UI is accessible.
  name: serviceEndpoint
  type: string
- description: Name of the zone in which the Data Fusion instance will be created.
  name: zone
  type: string
- description: Current version of Data Fusion.
  name: version
  type: string
- description: Display name for an instance.
  name: displayName
  type: string
- description: Output only. Endpoint on which the REST APIs is accessible.
  name: apiEndpoint
  type: string
provider_name: Google Cloud Data Fusion
provider_slug: google-cloud-data-fusion
schema_file: json-schema/google-cloud-data-fusion-instance-schema.json
slug: google-cloud-data-fusion-instance
source_filename: google-cloud-data-fusion-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-data-fusion/refs/heads/main/json-schema/google-cloud-data-fusion-instance-schema.json\",\n  \"title\": \"Google Cloud Data Fusion Instance\",\n  \"description\": \"Represents a Data Fusion instance, which is a managed environment for building and running data integration pipelines.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The name of this instance in the format projects/{project}/locations/{location}/instances/{instance}.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of this instance.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"BASIC\", \"ENTERPRISE\", \"DEVELOPER\"],\n      \"description\": \"The type of the Data Fusion instance.\"\n    },\n    \"enableStackdriverLogging\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Option to enable Stackdriver Logging.\"\n    },\n    \"enableStackdriverMonitoring\": {\n      \"type\": \"boolean\",\n      \"description\": \"Option to enable Stackdriver Monitoring.\"\n    },\n    \"privateInstance\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the Data Fusion instance should be private.\"\n    },\n    \"networkConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Network configuration options for a private instance.\",\n      \"properties\": {\n        \"network\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the network in the customer project.\"\n        },\n        \"ipAllocation\": {\n          \"type\": \"string\",\n          \"description\": \"The IP range in CIDR notation to use for the managed Data Fusion instance nodes.\"\n        }\n      }\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"The\
  \ resource labels for instance to use to annotate any related underlying resources.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"description\": \"Map of additional options used to configure the behavior of Data Fusion instance.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The time the instance was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The time the instance was last updated.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"STATE_UNSPECIFIED\",\n        \"CREATING\",\n        \"ACTIVE\",\n        \"FAILED\",\n        \"DELETING\",\n        \"UPGRADING\",\n        \"RESTARTING\",\n       \
  \ \"UPDATING\",\n        \"AUTO_UPDATING\",\n        \"AUTO_UPGRADING\",\n        \"DISABLED\"\n      ],\n      \"description\": \"Output only. The current state of this Data Fusion instance.\"\n    },\n    \"serviceEndpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Output only. Endpoint on which the Data Fusion UI is accessible.\"\n    },\n    \"zone\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the zone in which the Data Fusion instance will be created.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Current version of Data Fusion.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for an instance.\"\n    },\n    \"apiEndpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Output only. Endpoint on which the REST APIs is accessible.\"\n    }\n  },\n  \"required\": [\"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-data-fusion/refs/heads/main/json-schema/google-cloud-data-fusion-instance-schema.json
tags:
- Data Integration
- Data Pipelines
- ETL
- Google Cloud
title: Google Cloud Data Fusion Instance
---
