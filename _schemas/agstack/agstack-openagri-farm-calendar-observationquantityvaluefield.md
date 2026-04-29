---
description: ''
layout: schema
name: ObservationQuantityValueField
properties_list:
- description: ''
  name: unit
  type: string
- description: ''
  name: hasValue
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-observationquantityvaluefield-schema.json
slug: agstack-openagri-farm-calendar-observationquantityvaluefield
source_filename: agstack-openagri-farm-calendar-observationquantityvaluefield-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/ObservationQuantityValueField.json\",\n  \"title\": \"ObservationQuantityValueField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unit\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"nullable\": true\n    },\n    \"hasValue\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"hasValue\",\n    \"unit\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-observationquantityvaluefield-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: ObservationQuantityValueField
---
