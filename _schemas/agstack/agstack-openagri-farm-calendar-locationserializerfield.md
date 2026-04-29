---
description: ''
layout: schema
name: LocationSerializerField
properties_list:
- description: ''
  name: lat
  type: string
- description: ''
  name: long
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-locationserializerfield-schema.json
slug: agstack-openagri-farm-calendar-locationserializerfield
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/LocationSerializerField.json\",\n  \"title\": \"LocationSerializerField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lat\": {\n      \"type\": \"string\",\n      \"format\": \"decimal\",\n      \"pattern\": \"^-?\\\\d{0,3}(?:\\\\.\\\\d{0,14})?$\"\n    },\n    \"long\": {\n      \"type\": \"string\",\n      \"format\": \"decimal\",\n      \"pattern\": \"^-?\\\\d{0,3}(?:\\\\.\\\\d{0,14})?$\"\n    }\n  },\n  \"required\": [\n    \"lat\",\n    \"long\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-locationserializerfield-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: LocationSerializerField
---
