---
description: A storage volume is a logical container for data. Volumes are created within SVMs and reside on aggregates. They provide the primary unit of data management in ONTAP.
layout: schema
name: Volume
properties_list:
- description: Unique identifier for the volume
  name: uuid
  type: string
- description: Volume name (unique within the SVM)
  name: name
  type: string
- description: Volume type. rw = read-write, dp = data-protection, ls = load-sharing
  name: type
  type: string
- description: Volume operational state
  name: state
  type: string
- description: Volume style
  name: style
  type: string
- description: Volume size in bytes
  name: size
  type: integer
- description: Optional comment or description for the volume
  name: comment
  type: string
- description: Language encoding for the volume
  name: language
  type: string
- description: Time when the volume was created
  name: create_time
  type: string
- description: Aggregates hosting the volume. A FlexVol has one aggregate; a FlexGroup can span multiple aggregates.
  name: aggregates
  type: array
- description: Volume space usage and configuration
  name: space
  type: object
- description: NAS protocol configuration
  name: nas
  type: object
- description: Space guarantee configuration
  name: guarantee
  type: object
- description: Snapshot policy assigned to the volume
  name: snapshot_policy
  type: object
- description: Quality of service configuration
  name: qos
  type: object
- description: FabricPool tiering configuration
  name: tiering
  type: object
- description: Volume encryption configuration
  name: encryption
  type: object
- description: Volume autosize configuration
  name: autosize
  type: object
- description: Clone information if this volume is a clone
  name: clone
  type: object
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-volume-schema.json
slug: netapp-ontap-volume
source_filename: netapp-ontap-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Volume\",\n  \"type\": \"object\",\n  \"description\": \"A storage volume is a logical container for data. Volumes are created within SVMs and reside on aggregates. They provide the primary unit of data management in ONTAP.\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the volume\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Volume name (unique within the SVM)\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Volume type. rw = read-write, dp = data-protection, ls = load-sharing\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Volume operational state\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"Volume style\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Volume size in bytes\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment or description for the volume\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language encoding for the volume\"\n    },\n    \"create_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the volume was created\"\n    },\n    \"aggregates\": {\n      \"type\": \"array\",\n      \"description\": \"Aggregates hosting the volume. A FlexVol has one aggregate; a FlexGroup can span multiple aggregates.\"\n    },\n    \"space\": {\n      \"type\": \"object\",\n      \"description\": \"Volume space usage and configuration\"\n    },\n    \"nas\": {\n      \"type\": \"object\",\n      \"description\": \"NAS protocol configuration\"\n    },\n    \"guarantee\": {\n      \"type\": \"object\",\n      \"description\": \"Space guarantee configuration\"\n    },\n    \"snapshot_policy\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Snapshot policy assigned to the volume\"\n    },\n    \"qos\": {\n      \"type\": \"object\",\n      \"description\": \"Quality of service configuration\"\n    },\n    \"tiering\": {\n      \"type\": \"object\",\n      \"description\": \"FabricPool tiering configuration\"\n    },\n    \"encryption\": {\n      \"type\": \"object\",\n      \"description\": \"Volume encryption configuration\"\n    },\n    \"autosize\": {\n      \"type\": \"object\",\n      \"description\": \"Volume autosize configuration\"\n    },\n    \"clone\": {\n      \"type\": \"object\",\n      \"description\": \"Clone information if this volume is a clone\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-volume-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: Volume
---
