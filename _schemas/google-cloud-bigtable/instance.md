---
description: A Cloud Bigtable instance resource representing a container for clusters, tables, and application profiles.
layout: schema
name: Google Cloud Bigtable Instance
properties_list:
- description: The unique name of the instance in the format projects/{project}/instances/{instance}.
  name: name
  type: string
- description: The descriptive name for this instance as it appears in the UI.
  name: displayName
  type: string
- description: The current state of the instance.
  name: state
  type: string
- description: The type of the instance. PRODUCTION instances have a minimum of three nodes and can have replication configured. DEVELOPMENT instances are single-node and do not support replication.
  name: type
  type: string
- description: Labels for the instance as key-value pairs.
  name: labels
  type: object
- description: The creation time of the instance.
  name: createTime
  type: string
- description: Whether the instance satisfies the zone separation requirements.
  name: satisfiesPzs
  type: boolean
provider_name: Google Cloud Bigtable
provider_slug: google-cloud-bigtable
schema_file: json-schema/instance-schema.json
slug: instance
source_filename: instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-bigtable/refs/heads/main/json-schema/instance-schema.json\",\n  \"title\": \"Google Cloud Bigtable Instance\",\n  \"description\": \"A Cloud Bigtable instance resource representing a container for clusters, tables, and application profiles.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the instance in the format projects/{project}/instances/{instance}.\",\n      \"pattern\": \"^projects/[^/]+/instances/[^/]+$\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The descriptive name for this instance as it appears in the UI.\",\n      \"minLength\": 4,\n      \"maxLength\": 30\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"STATE_NOT_KNOWN\", \"READY\", \"CREATING\"],\n      \"description\"\
  : \"The current state of the instance.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"TYPE_UNSPECIFIED\", \"PRODUCTION\", \"DEVELOPMENT\"],\n      \"description\": \"The type of the instance. PRODUCTION instances have a minimum of three nodes and can have replication configured. DEVELOPMENT instances are single-node and do not support replication.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels for the instance as key-value pairs.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation time of the instance.\"\n    },\n    \"satisfiesPzs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the instance satisfies the zone separation requirements.\"\n    }\n  },\n  \"required\": [\"displayName\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-bigtable/refs/heads/main/json-schema/instance-schema.json
tags:
- Bigtable
- Database
- Google Cloud
- NoSQL
- Wide Column
title: Google Cloud Bigtable Instance
---
