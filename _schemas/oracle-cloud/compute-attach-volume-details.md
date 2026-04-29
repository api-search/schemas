---
description: Details for attaching a volume.
layout: schema
name: AttachVolumeDetails
properties_list:
- description: The OCID of the instance.
  name: instanceId
  type: string
- description: The OCID of the volume.
  name: volumeId
  type: string
- description: The type of volume attachment.
  name: type
  type: string
- description: A user-friendly name.
  name: displayName
  type: string
- description: Whether the attachment is read-only.
  name: isReadOnly
  type: boolean
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/compute-attach-volume-details-schema.json
slug: compute-attach-volume-details
source_filename: compute-attach-volume-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-attach-volume-details-schema.json\",\n  \"title\": \"AttachVolumeDetails\",\n  \"description\": \"Details for attaching a volume.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"instanceId\",\n    \"volumeId\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the instance.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"volumeId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the volume.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of volume attachment.\",\n      \"enum\": \"['iscsi', 'paravirtualized']\",\n      \"example\": \"iscsi\"\n    },\n    \"\
  displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name.\",\n      \"example\": \"my-resource\"\n    },\n    \"isReadOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the attachment is read-only.\",\n      \"example\": false,\n      \"default\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/compute-attach-volume-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: AttachVolumeDetails
---
