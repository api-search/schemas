---
description: ''
layout: schema
name: VisitorInfo
properties_list:
- description: ''
  name: capitalTours
  type: object
- description: ''
  name: visitorCenter
  type: object
- description: ''
  name: grounds
  type: object
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
schema_file: json-schema/aoc-data-api-visitor-info-schema.json
slug: aoc-data-api-visitor-info
source_filename: aoc-data-api-visitor-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-visitor-info-schema.json\",\n  \"title\": \"VisitorInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capitalTours\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"hours\": {\n          \"type\": \"string\"\n        },\n        \"reservationRequired\": {\n          \"type\": \"boolean\"\n        },\n        \"reservationUrl\": {\n          \"type\": \"string\"\n        },\n        \"phone\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"visitorCenter\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"hours\": {\n          \"type\": \"string\"\n        },\n        \"address\": {\n          \"type\": \"string\"\n        },\n        \"phone\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"\
  grounds\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"openDawn\": {\n          \"type\": \"boolean\"\n        },\n        \"closeDusk\": {\n          \"type\": \"boolean\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/json-schema/aoc-data-api-visitor-info-schema.json
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
title: VisitorInfo
---
