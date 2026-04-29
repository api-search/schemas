---
description: Response from the Get File Versions endpoint.
layout: schema
name: GetFileVersionsResponse
properties_list:
- description: An array of version history entries.
  name: versions
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-get-file-versions-response-schema.json
slug: figma-rest-get-file-versions-response
source_filename: figma-rest-get-file-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetFileVersionsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the Get File Versions endpoint.\",\n  \"properties\": {\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"An array of version history entries.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-get-file-versions-response-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetFileVersionsResponse
---
