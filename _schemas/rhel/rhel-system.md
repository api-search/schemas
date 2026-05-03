---
description: A Red Hat Enterprise Linux system registered with Subscription Management
layout: schema
name: RHEL System
properties_list:
- description: Unique system identifier
  name: uuid
  type: string
- description: System hostname
  name: name
  type: string
- description: System type
  name: type
  type: string
- description: System registration date
  name: created
  type: string
- description: Last update timestamp
  name: lastUpdated
  type: string
- description: Number of active entitlements
  name: entitlementCount
  type: integer
- description: Overall entitlement validity status
  name: entitlementStatus
  type: string
- description: Service level agreement tier
  name: serviceLevel
  type: string
- description: System usage designation
  name: usage
  type: string
- description: System hardware and software inventory facts
  name: facts
  type: object
provider_name: Red Hat Enterprise Linux
provider_slug: rhel
schema_file: json-schema/rhel-system-schema.json
slug: rhel-system
source_filename: rhel-system-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://github.com/api-evangelist/rhel/blob/main/json-schema/rhel-system-schema.json\",\n  \"title\": \"RHEL System\",\n  \"description\": \"A Red Hat Enterprise Linux system registered with Subscription Management\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique system identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"System hostname\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"System type\",\n      \"enum\": [\"physical\", \"virtual\", \"hypervisor\", \"container\"]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"System registration date\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Last update timestamp\"\n    },\n    \"entitlementCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active entitlements\",\n      \"minimum\": 0\n    },\n    \"entitlementStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall entitlement validity status\",\n      \"enum\": [\"valid\", \"invalid\", \"partial\"]\n    },\n    \"serviceLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Service level agreement tier\",\n      \"example\": \"Premium\"\n    },\n    \"usage\": {\n      \"type\": \"string\",\n      \"description\": \"System usage designation\",\n      \"example\": \"Production\"\n    },\n    \"facts\": {\n      \"type\": \"object\",\n      \"description\": \"System hardware and software inventory facts\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"uuid\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rhel/refs/heads/main/json-schema/rhel-system-schema.json
tags:
- Automation
- Compliance
- Enterprise
- Linux
- Operating System
- Red Hat
- RHEL
- Security
- Subscription Management
- Vulnerability Management
title: RHEL System
---
