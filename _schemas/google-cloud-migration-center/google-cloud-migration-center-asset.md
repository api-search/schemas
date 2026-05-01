---
description: Schema for a Migration Center asset representing a discovered infrastructure resource in a customer environment.
layout: schema
name: Google Cloud Migration Center Asset
properties_list:
- description: The full resource name of the asset
  name: name
  type: string
- description: Timestamp when the asset was created
  name: createTime
  type: string
- description: Timestamp when the asset was last updated
  name: updateTime
  type: string
- description: Labels applied to the asset
  name: labels
  type: object
- description: Generic asset attributes
  name: attributes
  type: object
- description: Details of the machine if the asset is a machine
  name: machineDetails
  type: object
- description: Groups the asset is assigned to
  name: assignedGroups
  type: array
- description: The sources that contributed to this asset
  name: sources
  type: array
provider_name: Google Cloud Migration Center
provider_slug: google-cloud-migration-center
schema_file: json-schema/google-cloud-migration-center-asset-schema.json
slug: google-cloud-migration-center-asset
source_filename: google-cloud-migration-center-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/migrationcenter/asset.json\",\n  \"title\": \"Google Cloud Migration Center Asset\",\n  \"description\": \"Schema for a Migration Center asset representing a discovered infrastructure resource in a customer environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full resource name of the asset\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the asset was created\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the asset was last updated\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels applied\
  \ to the asset\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Generic asset attributes\"\n    },\n    \"machineDetails\": {\n      \"$ref\": \"#/$defs/MachineDetails\",\n      \"description\": \"Details of the machine if the asset is a machine\"\n    },\n    \"assignedGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Groups the asset is assigned to\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The sources that contributed to this asset\"\n    }\n  },\n  \"$defs\": {\n    \"MachineDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details of a machine asset including hardware and software information\",\n      \"properties\": {\n        \"uuid\": {\n          \"type\": \"string\",\n  \
  \        \"description\": \"Machine unique identifier\"\n        },\n        \"machineName\": {\n          \"type\": \"string\",\n          \"description\": \"Machine name\"\n        },\n        \"coreCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of CPU cores\",\n          \"minimum\": 0\n        },\n        \"memoryMb\": {\n          \"type\": \"integer\",\n          \"description\": \"Memory size in megabytes\",\n          \"minimum\": 0\n        },\n        \"diskCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of disks\",\n          \"minimum\": 0\n        },\n        \"totalDiskSizeGb\": {\n          \"type\": \"integer\",\n          \"description\": \"Total disk size in gigabytes\",\n          \"minimum\": 0\n        },\n        \"platform\": {\n          \"type\": \"string\",\n          \"description\": \"Platform information for the machine\"\n        },\n        \"powerState\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Power state of the machine\",\n          \"enum\": [\"POWER_STATE_UNSPECIFIED\", \"PENDING\", \"ACTIVE\", \"SUSPENDING\", \"SUSPENDED\", \"DELETING\", \"DELETED\"]\n        },\n        \"networkAdapters\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/NetworkAdapter\"\n          },\n          \"description\": \"Network adapters attached to the machine\"\n        },\n        \"guestOs\": {\n          \"$ref\": \"#/$defs/GuestOsDetails\",\n          \"description\": \"Guest operating system information\"\n        }\n      }\n    },\n    \"NetworkAdapter\": {\n      \"type\": \"object\",\n      \"description\": \"A network adapter on a machine\",\n      \"properties\": {\n        \"adapterType\": {\n          \"type\": \"string\",\n          \"description\": \"Network adapter type\"\n        },\n        \"macAddress\": {\n          \"type\": \"string\",\n          \"description\": \"MAC address of the adapter\"\n\
  \        },\n        \"ipAddresses\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"IP addresses assigned to the adapter\"\n        }\n      }\n    },\n    \"GuestOsDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Guest operating system details\",\n      \"properties\": {\n        \"osName\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system name\"\n        },\n        \"family\": {\n          \"type\": \"string\",\n          \"description\": \"OS family (e.g., LINUX, WINDOWS)\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system version\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-migration-center/refs/heads/main/json-schema/google-cloud-migration-center-asset-schema.json
tags:
- Assessment
- Cloud Migration
- Discovery
- Infrastructure
- Migration
- Planning
title: Google Cloud Migration Center Asset
---
