---
description: Metadata for a learning object in a specific locale
layout: schema
name: LocalizedMetadata
properties_list:
- description: Description in the specified locale
  name: description
  type: string
- description: The locale code (e.g. en-US, fr-FR)
  name: locale
  type: string
- description: Name in the specified locale
  name: name
  type: string
- description: Overview or summary text
  name: overview
  type: string
- description: Rich text (HTML) overview content
  name: richTextOverview
  type: string
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-localized-metadata-schema.json
slug: prime-api-localized-metadata
source_filename: prime-api-localized-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-localized-metadata-schema.json\",\n  \"title\": \"LocalizedMetadata\",\n  \"description\": \"Metadata for a learning object in a specific locale\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description in the specified locale\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"The locale code (e.g. en-US, fr-FR)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name in the specified locale\"\n    },\n    \"overview\": {\n      \"type\": \"string\",\n      \"description\": \"Overview or summary text\"\n    },\n    \"richTextOverview\": {\n      \"type\": \"string\",\n      \"description\": \"Rich text (HTML) overview content\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-localized-metadata-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: LocalizedMetadata
---
