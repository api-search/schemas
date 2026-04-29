---
description: Request body for creating or updating a library.
layout: schema
name: LibraryInput
properties_list:
- description: Name of the library.
  name: name
  type: string
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
schema_file: json-schema/creative-cloud-libraries-library-input-schema.json
slug: creative-cloud-libraries-library-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-library-input-schema.json\",\n  \"title\": \"LibraryInput\",\n  \"description\": \"Request body for creating or updating a library.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the library.\",\n      \"example\": \"New Video Assets Library\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/json-schema/creative-cloud-libraries-library-input-schema.json
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
title: LibraryInput
---
