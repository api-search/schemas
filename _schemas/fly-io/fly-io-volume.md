---
description: A Fly Volume is a persistent block storage resource that can be attached to a Fly Machine for durable data storage. Volumes are region-specific, encrypted by default, and support automatic daily snapshots with configurable retention periods. Volumes are identified by a unique ID and can be extended in size but not shrunk.
layout: schema
name: Fly.io Volume
properties_list:
- description: Unique identifier for this Fly Volume.
  name: id
  type: string
- description: Human-readable name for the volume, used for identification within an app.
  name: name
  type: string
- description: Current operational state of the volume.
  name: state
  type: string
- description: Current size of the volume in gigabytes.
  name: size_gb
  type: integer
- description: The region code where this volume is provisioned.
  name: region
  type: string
- description: The availability zone within the region where this volume resides.
  name: zone
  type: string
- description: Whether the volume is encrypted at rest using platform-managed keys. Enabled by default for all volumes.
  name: encrypted
  type: boolean
- description: The ID of the Fly Machine this volume is currently attached to. Null if unattached.
  name: attached_machine_id
  type:
  - string
  - 'null'
- description: The allocation ID of the Machine this volume is attached to.
  name: attached_alloc_id
  type:
  - string
  - 'null'
- description: The filesystem type provisioned on this volume.
  name: filesystem_type
  type: string
- description: Number of days automatic snapshots are retained. Defaults to 5. Minimum 1, maximum 60.
  name: snapshot_retention
  type: integer
- description: Block size of the volume filesystem in bytes.
  name: block_size
  type: integer
- description: Total number of filesystem blocks.
  name: blocks
  type: integer
- description: Number of free filesystem blocks available for use.
  name: blocks_free
  type: integer
- description: Number of filesystem blocks available to non-root users.
  name: blocks_avail
  type: integer
- description: ISO 8601 timestamp of when the volume was created.
  name: created_at
  type: string
provider_name: fly-io
provider_slug: fly-io
schema_file: json-schema/fly-io-volume-schema.json
slug: fly-io-volume
source_filename: fly-io-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fly.io/schemas/volume.json\",\n  \"title\": \"Fly.io Volume\",\n  \"description\": \"A Fly Volume is a persistent block storage resource that can be attached to a Fly Machine for durable data storage. Volumes are region-specific, encrypted by default, and support automatic daily snapshots with configurable retention periods. Volumes are identified by a unique ID and can be extended in size but not shrunk.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"size_gb\", \"region\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this Fly Volume.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the volume, used for identification within an app.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational state of\
  \ the volume.\",\n      \"enum\": [\"created\", \"hydrating\", \"available\", \"attached\", \"deleting\", \"deleted\"]\n    },\n    \"size_gb\": {\n      \"type\": \"integer\",\n      \"description\": \"Current size of the volume in gigabytes.\",\n      \"minimum\": 1\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The region code where this volume is provisioned.\",\n      \"pattern\": \"^[a-z]{3}$\",\n      \"example\": \"iad\"\n    },\n    \"zone\": {\n      \"type\": \"string\",\n      \"description\": \"The availability zone within the region where this volume resides.\"\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the volume is encrypted at rest using platform-managed keys. Enabled by default for all volumes.\"\n    },\n    \"attached_machine_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the Fly Machine this volume is currently attached to. Null if unattached.\"\
  \n    },\n    \"attached_alloc_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The allocation ID of the Machine this volume is attached to.\"\n    },\n    \"filesystem_type\": {\n      \"type\": \"string\",\n      \"description\": \"The filesystem type provisioned on this volume.\",\n      \"example\": \"ext4\"\n    },\n    \"snapshot_retention\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days automatic snapshots are retained. Defaults to 5. Minimum 1, maximum 60.\",\n      \"default\": 5,\n      \"minimum\": 1,\n      \"maximum\": 60\n    },\n    \"block_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Block size of the volume filesystem in bytes.\"\n    },\n    \"blocks\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of filesystem blocks.\"\n    },\n    \"blocks_free\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of free filesystem blocks available for use.\"\n    },\n\
  \    \"blocks_avail\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of filesystem blocks available to non-root users.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of when the volume was created.\"\n    }\n  },\n  \"$defs\": {\n    \"VolumeSnapshot\": {\n      \"type\": \"object\",\n      \"description\": \"A point-in-time snapshot of a Fly Volume, used for backup and disaster recovery.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for this snapshot.\"\n        },\n        \"size\": {\n          \"type\": \"integer\",\n          \"description\": \"Size of the snapshot data in bytes.\"\n        },\n        \"digest\": {\n          \"type\": \"string\",\n          \"description\": \"Content hash of the snapshot for data integrity verification.\"\n        },\n    \
  \    \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the snapshot.\",\n          \"enum\": [\"created\", \"pending\", \"failed\"]\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp of when the snapshot was created.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fly-io/refs/heads/main/json-schema/fly-io-volume-schema.json
tags: []
title: Fly.io Volume
---
