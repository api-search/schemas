---
description: A Linode compute instance representing a virtual machine running on the Akamai Connected Cloud platform. Instances have configurable CPU, memory, storage, and networking resources and can be deployed from distribution images or custom images.
layout: schema
name: Linode Instance
properties_list:
- description: The unique identifier for this Linode instance.
  name: id
  type: integer
- description: The display label for this Linode instance. Must begin with a letter and may only contain letters, numbers, dashes, and underscores.
  name: label
  type: string
- description: The region identifier where this Linode instance is deployed, such as us-east or eu-west.
  name: region
  type: string
- description: The Linode plan type identifier that determines the instance's hardware resources and pricing.
  name: type
  type: string
- description: The image identifier used to deploy this Linode instance, or null if deployed from a backup.
  name: image
  type:
  - string
  - 'null'
- description: The current operational status of the Linode instance.
  name: status
  type: string
- description: The IPv4 addresses assigned to this Linode instance.
  name: ipv4
  type: array
- description: The IPv6 SLAAC address for this Linode instance.
  name: ipv6
  type:
  - string
  - 'null'
- description: The date and time when this Linode instance was created.
  name: created
  type: string
- description: The date and time when this Linode instance was last updated.
  name: updated
  type: string
- description: User-defined tags applied to this Linode instance for organizational purposes.
  name: tags
  type: array
- description: The virtualization hypervisor this Linode instance runs on.
  name: hypervisor
  type: string
- description: Whether the Lassie watchdog is enabled to automatically restart this instance if it powers off unexpectedly.
  name: watchdog_enabled
  type: boolean
- description: ''
  name: specs
  type: object
- description: ''
  name: alerts
  type: object
- description: ''
  name: backups
  type: object
provider_name: linode
provider_slug: linode
schema_file: json-schema/linode-instance-schema.json
slug: linode-instance
source_filename: linode-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.linode.com/schemas/linode/instance.json\",\n  \"title\": \"Linode Instance\",\n  \"description\": \"A Linode compute instance representing a virtual machine running on the Akamai Connected Cloud platform. Instances have configurable CPU, memory, storage, and networking resources and can be deployed from distribution images or custom images.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"label\", \"region\", \"type\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier for this Linode instance.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"minLength\": 3,\n      \"maxLength\": 64,\n      \"pattern\": \"^[a-zA-Z]((?!--|__)[a-zA-Z0-9-_])+$\",\n      \"description\": \"The display label for this Linode instance. Must begin with a letter and may only contain letters, numbers, dashes,\
  \ and underscores.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The region identifier where this Linode instance is deployed, such as us-east or eu-west.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The Linode plan type identifier that determines the instance's hardware resources and pricing.\"\n    },\n    \"image\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The image identifier used to deploy this Linode instance, or null if deployed from a backup.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"running\",\n        \"offline\",\n        \"booting\",\n        \"rebooting\",\n        \"shutting_down\",\n        \"provisioning\",\n        \"deleting\",\n        \"migrating\",\n        \"rebuilding\",\n        \"cloning\",\n        \"restoring\",\n        \"stopped\"\n      ],\n      \"description\": \"The current operational status of the Linode\
  \ instance.\"\n    },\n    \"ipv4\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"ipv4\"\n      },\n      \"description\": \"The IPv4 addresses assigned to this Linode instance.\"\n    },\n    \"ipv6\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The IPv6 SLAAC address for this Linode instance.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when this Linode instance was created.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when this Linode instance was last updated.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-defined tags applied to this Linode instance for organizational purposes.\"\n    },\n    \"hypervisor\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The virtualization hypervisor this Linode instance runs on.\"\n    },\n    \"watchdog_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Lassie watchdog is enabled to automatically restart this instance if it powers off unexpectedly.\"\n    },\n    \"specs\": {\n      \"$ref\": \"#/$defs/InstanceSpecs\"\n    },\n    \"alerts\": {\n      \"$ref\": \"#/$defs/InstanceAlerts\"\n    },\n    \"backups\": {\n      \"$ref\": \"#/$defs/BackupInfo\"\n    }\n  },\n  \"$defs\": {\n    \"InstanceSpecs\": {\n      \"type\": \"object\",\n      \"description\": \"The hardware specifications for this Linode instance based on its plan type.\",\n      \"properties\": {\n        \"disk\": {\n          \"type\": \"integer\",\n          \"description\": \"The total disk space in megabytes.\"\n        },\n        \"memory\": {\n          \"type\": \"integer\",\n          \"description\": \"The total RAM in megabytes.\"\n        },\n\
  \        \"vcpus\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The number of virtual CPU cores.\"\n        },\n        \"gpus\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of GPUs, if applicable.\"\n        },\n        \"transfer\": {\n          \"type\": \"integer\",\n          \"description\": \"The monthly network transfer quota in gigabytes.\"\n        }\n      }\n    },\n    \"InstanceAlerts\": {\n      \"type\": \"object\",\n      \"description\": \"Alert thresholds for monitoring this Linode instance.\",\n      \"properties\": {\n        \"cpu\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The CPU usage percentage threshold for alerts.\"\n        },\n        \"io\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The disk IO rate threshold for alerts.\"\n        },\n        \"\
  network_in\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The incoming network traffic threshold in Mb/s for alerts.\"\n        },\n        \"network_out\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The outgoing network traffic threshold in Mb/s for alerts.\"\n        },\n        \"transfer_quota\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"The transfer quota usage percentage threshold for alerts.\"\n        }\n      }\n    },\n    \"BackupInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the backup service for this Linode instance.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the backup service is enabled for this instance.\"\n        },\n        \"available\": {\n          \"type\": \"boolean\",\n\
  \          \"description\": \"Whether any backups are currently available for restoration.\"\n        },\n        \"schedule\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"day\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"The day of the week for weekly automatic backups.\"\n            },\n            \"window\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"The two-hour UTC window for daily automatic backups.\"\n            }\n          },\n          \"description\": \"The schedule for automatic backups.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linode/refs/heads/main/json-schema/linode-instance-schema.json
tags: []
title: Linode Instance
---
