---
description: Details for updating an instance.
layout: schema
name: UpdateInstanceDetails
properties_list:
- description: A user-friendly name.
  name: displayName
  type: string
- description: The shape of the instance.
  name: shape
  type: string
- description: ''
  name: shapeConfig
  type: object
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/compute-update-instance-details-schema.json
slug: compute-update-instance-details
source_filename: compute-update-instance-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-update-instance-details-schema.json\",\n  \"title\": \"UpdateInstanceDetails\",\n  \"description\": \"Details for updating an instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name.\",\n      \"example\": \"updated-instance-name\"\n    },\n    \"shape\": {\n      \"type\": \"string\",\n      \"description\": \"The shape of the instance.\",\n      \"example\": \"VM.Standard.E4.Flex\"\n    },\n    \"shapeConfig\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"ocpus\": 4.0,\n        \"memoryInGBs\": 32.0\n      }\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"\
  type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-update-instance-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: UpdateInstanceDetails
---
