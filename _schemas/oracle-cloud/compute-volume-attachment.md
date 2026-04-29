---
description: A volume attached to a compute instance.
layout: schema
name: VolumeAttachment
properties_list:
- description: The OCID of the volume attachment.
  name: id
  type: string
- description: The OCID of the instance.
  name: instanceId
  type: string
- description: The OCID of the volume.
  name: volumeId
  type: string
- description: A user-friendly name.
  name: displayName
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
- description: The type of volume attachment.
  name: attachmentType
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/compute-volume-attachment-schema.json
slug: compute-volume-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-volume-attachment-schema.json\",\n  \"title\": \"VolumeAttachment\",\n  \"description\": \"A volume attached to a compute instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the volume attachment.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the instance.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"volumeId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the volume.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name.\"\
  ,\n      \"example\": \"my-resource\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['ATTACHING', 'ATTACHED', 'DETACHING', 'DETACHED']\",\n      \"example\": \"ATTACHING\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"attachmentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of volume attachment.\",\n      \"enum\": \"['iscsi', 'paravirtualized']\",\n      \"example\": \"iscsi\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-volume-attachment-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: VolumeAttachment
---
