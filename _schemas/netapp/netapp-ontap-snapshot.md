---
description: A point-in-time copy of a volume
layout: schema
name: Snapshot
properties_list:
- description: Snapshot UUID
  name: uuid
  type: string
- description: Snapshot name
  name: name
  type: string
- description: Time when the snapshot was created
  name: create_time
  type: string
- description: Time when the snapshot expires and can be automatically deleted
  name: expiry_time
  type: string
- description: Optional comment for the snapshot
  name: comment
  type: string
- description: Amount of space consumed by the snapshot in bytes
  name: size
  type: integer
- description: Snapshot state
  name: state
  type: string
- description: SnapMirror label used for policy-based selection
  name: snapmirror_label
  type: string
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-snapshot-schema.json
slug: netapp-ontap-snapshot
source_filename: netapp-ontap-snapshot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Snapshot\",\n  \"type\": \"object\",\n  \"description\": \"A point-in-time copy of a volume\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Snapshot UUID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Snapshot name\"\n    },\n    \"create_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the snapshot was created\"\n    },\n    \"expiry_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the snapshot expires and can be automatically deleted\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional comment for the snapshot\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount of space consumed by the snapshot in bytes\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Snapshot state\"\n    },\n    \"snapmirror_label\": {\n      \"type\": \"string\",\n      \"description\": \"SnapMirror label used for policy-based selection\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-snapshot-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: Snapshot
---
