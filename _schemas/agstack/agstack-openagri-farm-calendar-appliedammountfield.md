---
description: ''
layout: schema
name: AppliedAmmountField
properties_list:
- description: ''
  name: unit
  type: string
- description: ''
  name: numericValue
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-appliedammountfield-schema.json
slug: agstack-openagri-farm-calendar-appliedammountfield
source_filename: agstack-openagri-farm-calendar-appliedammountfield-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/AppliedAmmountField.json\",\n  \"title\": \"AppliedAmmountField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unit\": {\n      \"type\": \"string\"\n    },\n    \"numericValue\": {\n      \"type\": \"string\",\n      \"format\": \"decimal\",\n      \"pattern\": \"^-?\\\\d{0,15}(?:\\\\.\\\\d{0,2})?$\"\n    }\n  },\n  \"required\": [\n    \"numericValue\",\n    \"unit\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-appliedammountfield-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: AppliedAmmountField
---
