---
description: Subset of FHIR R4 Observation as exposed by CharmHealth EHR.
layout: schema
name: CharmHealth FHIR Observation
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: category
  type: array
- description: ''
  name: code
  type: object
- description: ''
  name: subject
  type: object
- description: ''
  name: effectiveDateTime
  type: string
- description: ''
  name: valueQuantity
  type: object
provider_name: CharmHealth
provider_slug: charmhealth
schema_file: json-schema/charmhealth-observation-schema.json
slug: charmhealth-observation
source_filename: charmhealth-observation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.charmhealth.com/schemas/observation.json\",\n  \"title\": \"CharmHealth FHIR Observation\",\n  \"description\": \"Subset of FHIR R4 Observation as exposed by CharmHealth EHR.\",\n  \"type\": \"object\",\n  \"required\": [\"resourceType\", \"status\", \"code\"],\n  \"properties\": {\n    \"resourceType\": { \"const\": \"Observation\" },\n    \"id\": { \"type\": \"string\" },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"registered\",\n        \"preliminary\",\n        \"final\",\n        \"amended\",\n        \"corrected\",\n        \"cancelled\",\n        \"entered-in-error\",\n        \"unknown\"\n      ]\n    },\n    \"category\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"coding\": {\n            \"type\": \"array\",\n            \"items\": { \"$ref\": \"#/$defs/coding\"\
  \ }\n          }\n        }\n      }\n    },\n    \"code\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"coding\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/coding\" }\n        }\n      }\n    },\n    \"subject\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"reference\": { \"type\": \"string\" }\n      }\n    },\n    \"effectiveDateTime\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"valueQuantity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": { \"type\": \"number\" },\n        \"unit\": { \"type\": \"string\" },\n        \"system\": { \"type\": \"string\" },\n        \"code\": { \"type\": \"string\" }\n      }\n    }\n  },\n  \"$defs\": {\n    \"coding\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"system\": { \"type\": \"string\" },\n        \"code\": { \"type\": \"string\" },\n        \"display\": { \"type\": \"string\" }\n      }\n  \
  \  }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/json-schema/charmhealth-observation-schema.json
tags:
- EHR
- EMR
- FHIR
- Healthcare
- HL7
- Patient Engagement
- Patients
- SMART on FHIR
- US Core
title: CharmHealth FHIR Observation
---
