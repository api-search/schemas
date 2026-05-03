---
description: A Scaleway virtual machine instance with compute, storage, and networking configuration
layout: schema
name: Scaleway Instance
properties_list:
- description: Unique identifier of the Instance
  name: id
  type: string
- description: Display name of the Instance
  name: name
  type: string
- description: Current state of the Instance
  name: state
  type: string
- description: Commercial type of the Instance (e.g., GP1-S, DEV1-S, RENDER-S)
  name: commercial_type
  type: string
- description: OS image used by the Instance
  name: image
  type: object
- description: Storage volumes attached to the Instance
  name: volumes
  type: object
- description: Public IP address assigned to the Instance
  name: public_ip
  type: object
- description: Private IP address of the Instance
  name: private_ip
  type: string
- description: Availability zone where the Instance is located
  name: zone
  type: string
- description: Organization ID that owns the Instance
  name: organization
  type: string
- description: Project ID that the Instance belongs to
  name: project
  type: string
- description: User-defined tags for the Instance
  name: tags
  type: array
- description: Security group applied to the Instance
  name: security_group
  type: object
- description: Whether IPv6 is enabled for the Instance
  name: enable_ipv6
  type: boolean
- description: IPv6 configuration
  name: ipv6
  type: object
- description: Timestamp when the Instance was created
  name: creation_date
  type: string
- description: Timestamp when the Instance was last modified
  name: modification_date
  type: string
provider_name: Scaleway
provider_slug: scaleway
schema_file: json-schema/scaleway-instance-schema.json
slug: scaleway-instance
source_filename: scaleway-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scaleway/main/json-schema/scaleway-instance-schema.json\",\n  \"title\": \"Scaleway Instance\",\n  \"description\": \"A Scaleway virtual machine instance with compute, storage, and networking configuration\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"state\", \"commercial_type\", \"zone\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of the Instance\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the Instance\",\n      \"maxLength\": 255\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"running\", \"stopped\", \"stopped in place\", \"starting\", \"stopping\", \"locked\"],\n      \"description\": \"Current state of the Instance\"\n    },\n    \"commercial_type\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Commercial type of the Instance (e.g., GP1-S, DEV1-S, RENDER-S)\",\n      \"examples\": [\"GP1-S\", \"GP1-M\", \"DEV1-S\", \"PRO2-S\"]\n    },\n    \"image\": {\n      \"type\": \"object\",\n      \"description\": \"OS image used by the Instance\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"arch\": {\n          \"type\": \"string\",\n          \"enum\": [\"x86_64\", \"arm64\"]\n        }\n      }\n    },\n    \"volumes\": {\n      \"type\": \"object\",\n      \"description\": \"Storage volumes attached to the Instance\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n    \
  \      },\n          \"size\": {\n            \"type\": \"integer\",\n            \"description\": \"Volume size in bytes\"\n          },\n          \"volume_type\": {\n            \"type\": \"string\",\n            \"enum\": [\"l_ssd\", \"b_ssd\", \"sbs_volume\"]\n          }\n        }\n      }\n    },\n    \"public_ip\": {\n      \"type\": \"object\",\n      \"description\": \"Public IP address assigned to the Instance\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"ipv4\"\n        },\n        \"dynamic\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"private_ip\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"Private IP address of the Instance\"\n    },\n    \"zone\": {\n      \"type\": \"string\",\n      \"description\": \"Availability zone where the Instance is located\",\n      \"examples\": [\"fr-par-1\", \"nl-ams-1\", \"pl-waw-1\", \"it-mil-1\"]\n    },\n\
  \    \"organization\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Organization ID that owns the Instance\"\n    },\n    \"project\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Project ID that the Instance belongs to\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-defined tags for the Instance\"\n    },\n    \"security_group\": {\n      \"type\": \"object\",\n      \"description\": \"Security group applied to the Instance\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"enable_ipv6\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether IPv6 is enabled for the Instance\"\n    },\n    \"ipv6\": {\n      \"type\": \"object\",\n      \"\
  description\": \"IPv6 configuration\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"ipv6\"\n        },\n        \"netmask\": {\n          \"type\": \"string\"\n        },\n        \"gateway\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"creation_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the Instance was created\"\n    },\n    \"modification_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the Instance was last modified\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/json-schema/scaleway-instance-schema.json
tags:
- AI
- Cloud Computing
- Containers
- Database
- European Cloud
- Infrastructure
- Kubernetes
- Serverless
- Storage
title: Scaleway Instance
---
