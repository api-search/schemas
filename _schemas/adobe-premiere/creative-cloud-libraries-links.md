---
description: Hypermedia links for a resource.
layout: schema
name: Links
properties_list:
- description: URL of the resource itself.
  name: self
  type: string
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schema_file: json-schema/creative-cloud-libraries-links-schema.json
slug: creative-cloud-libraries-links
source_filename: creative-cloud-libraries-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-links-schema.json\",\n  \"title\": \"Links\",\n  \"description\": \"Hypermedia links for a resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the resource itself.\",\n      \"example\": \"https://cc-libraries.adobe.io/api/v1/libraries/lib-abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-links-schema.json
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
title: Links
---
