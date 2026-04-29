---
description: Reference to an asynchronous job
layout: schema
name: JobLink
properties_list:
- description: Job UUID
  name: uuid
  type: string
- description: ''
  name: _links
  type: object
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-job-link-schema.json
slug: netapp-ontap-job-link
source_filename: netapp-ontap-job-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobLink\",\n  \"type\": \"object\",\n  \"description\": \"Reference to an asynchronous job\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Job UUID\"\n    },\n    \"_links\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-job-link-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: JobLink
---
