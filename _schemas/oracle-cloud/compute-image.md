---
description: A boot disk image for launching compute instances.
layout: schema
name: Image
properties_list:
- description: The OCID of the image.
  name: id
  type: string
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: A user-friendly name.
  name: displayName
  type: string
- description: The image operating system.
  name: operatingSystem
  type: string
- description: The image operating system version.
  name: operatingSystemVersion
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: Size of the image in megabytes.
  name: sizeInMBs
  type: integer
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/compute-image-schema.json
slug: compute-image
source_filename: compute-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-image-schema.json\",\n  \"title\": \"Image\",\n  \"description\": \"A boot disk image for launching compute instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the image.\",\n      \"example\": \"ocid1.image.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name.\",\n      \"example\": \"Oracle-Linux-8.8-2026.01.01-0\"\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"The image operating system.\",\n      \"example\"\
  : \"Oracle Linux\"\n    },\n    \"operatingSystemVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The image operating system version.\",\n      \"example\": \"8.8\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['PROVISIONING', 'IMPORTING', 'AVAILABLE', 'EXPORTING', 'DISABLED', 'DELETED']\",\n      \"example\": \"PROVISIONING\"\n    },\n    \"sizeInMBs\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the image in megabytes.\",\n      \"example\": 47694\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-image-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Image
---
