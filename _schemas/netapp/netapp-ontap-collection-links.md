---
description: Pagination links for collection responses
layout: schema
name: CollectionLinks
properties_list:
- description: ''
  name: self
  type: object
- description: Link to the next page of results
  name: next
  type: object
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-collection-links-schema.json
slug: netapp-ontap-collection-links
source_filename: netapp-ontap-collection-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectionLinks\",\n  \"type\": \"object\",\n  \"description\": \"Pagination links for collection responses\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"object\"\n    },\n    \"next\": {\n      \"type\": \"object\",\n      \"description\": \"Link to the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-collection-links-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: CollectionLinks
---
