---
description: A Cloud Spanner instance resource that provides compute and storage capacity for Spanner databases.
layout: schema
name: Google Cloud Spanner Instance
properties_list:
- description: The unique name of the instance in the format projects/{project}/instances/{instance}.
  name: name
  type: string
- description: The name of the instance's configuration (e.g., projects/{project}/instanceConfigs/{config}).
  name: config
  type: string
- description: The descriptive name for the instance.
  name: displayName
  type: string
- description: The number of nodes allocated to this instance. At most one of nodeCount or processingUnits should be present.
  name: nodeCount
  type: integer
- description: The number of processing units allocated (100 processing units = 1 node).
  name: processingUnits
  type: integer
- description: The current state of the instance.
  name: state
  type: string
- description: Cloud labels for this instance.
  name: labels
  type: object
- description: The endpoint URIs for this instance.
  name: endpointUris
  type: array
- description: The creation time of the instance.
  name: createTime
  type: string
- description: The last update time of the instance.
  name: updateTime
  type: string
provider_name: Google Cloud Spanner
provider_slug: google-cloud-spanner
schema_file: json-schema/instance-schema.json
slug: instance
source_filename: instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-spanner/refs/heads/main/json-schema/instance-schema.json\",\n  \"title\": \"Google Cloud Spanner Instance\",\n  \"description\": \"A Cloud Spanner instance resource that provides compute and storage capacity for Spanner databases.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the instance in the format projects/{project}/instances/{instance}.\",\n      \"pattern\": \"^projects/[^/]+/instances/[^/]+$\"\n    },\n    \"config\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the instance's configuration (e.g., projects/{project}/instanceConfigs/{config}).\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The descriptive name for the instance.\",\n      \"minLength\": 4,\n      \"maxLength\"\
  : 30\n    },\n    \"nodeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of nodes allocated to this instance. At most one of nodeCount or processingUnits should be present.\",\n      \"minimum\": 1\n    },\n    \"processingUnits\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of processing units allocated (100 processing units = 1 node).\",\n      \"minimum\": 100\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"STATE_UNSPECIFIED\", \"CREATING\", \"READY\"],\n      \"description\": \"The current state of the instance.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Cloud labels for this instance.\"\n    },\n    \"endpointUris\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      },\n      \"description\": \"The endpoint URIs for this\
  \ instance.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation time of the instance.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last update time of the instance.\"\n    }\n  },\n  \"required\": [\"config\", \"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-spanner/refs/heads/main/json-schema/instance-schema.json
tags:
- Database
- Distributed
- Google Cloud
- Relational
- SQL
title: Google Cloud Spanner Instance
---
