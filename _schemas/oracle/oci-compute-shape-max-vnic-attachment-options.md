---
description: Options for configuring max VNIC attachments on a flexible shape
layout: schema
name: ShapeMaxVnicAttachmentOptions
properties_list:
- description: The minimum number of VNIC attachments
  name: min
  type: integer
- description: The maximum number of VNIC attachments
  name: max
  type: number
- description: The default number of VNIC attachments per OCPU
  name: defaultPerOcpu
  type: number
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-shape-max-vnic-attachment-options-schema.json
slug: oci-compute-shape-max-vnic-attachment-options
source_filename: oci-compute-shape-max-vnic-attachment-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShapeMaxVnicAttachmentOptions\",\n  \"type\": \"object\",\n  \"description\": \"Options for configuring max VNIC attachments on a flexible shape\",\n  \"properties\": {\n    \"min\": {\n      \"type\": \"integer\",\n      \"description\": \"The minimum number of VNIC attachments\"\n    },\n    \"max\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum number of VNIC attachments\"\n    },\n    \"defaultPerOcpu\": {\n      \"type\": \"number\",\n      \"description\": \"The default number of VNIC attachments per OCPU\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-shape-max-vnic-attachment-options-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: ShapeMaxVnicAttachmentOptions
---
