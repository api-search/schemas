---
description: Subset of FHIR R4 Patient as exposed by CharmHealth EHR.
layout: schema
name: CharmHealth FHIR Patient
properties_list:
- description: ''
  name: resourceType
  type: object
- description: ''
  name: id
  type: string
- description: ''
  name: identifier
  type: array
- description: ''
  name: name
  type: array
- description: ''
  name: gender
  type: string
- description: ''
  name: birthDate
  type: string
- description: ''
  name: telecom
  type: array
- description: ''
  name: address
  type: array
provider_name: CharmHealth
provider_slug: charmhealth
schema_file: json-schema/charmhealth-patient-schema.json
slug: charmhealth-patient
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.charmhealth.com/schemas/patient.json\",\n  \"title\": \"CharmHealth FHIR Patient\",\n  \"description\": \"Subset of FHIR R4 Patient as exposed by CharmHealth EHR.\",\n  \"type\": \"object\",\n  \"required\": [\"resourceType\", \"id\"],\n  \"properties\": {\n    \"resourceType\": { \"const\": \"Patient\" },\n    \"id\": { \"type\": \"string\" },\n    \"identifier\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"system\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"name\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"use\": { \"type\": \"string\" },\n          \"family\": { \"type\": \"string\" },\n          \"given\": { \"type\": \"array\", \"items\": { \"type\": \"string\"\
  \ } }\n        }\n      }\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\"male\", \"female\", \"other\", \"unknown\"]\n    },\n    \"birthDate\": { \"type\": \"string\", \"format\": \"date\" },\n    \"telecom\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"system\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" },\n          \"use\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"address\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"line\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n          \"city\": { \"type\": \"string\" },\n          \"state\": { \"type\": \"string\" },\n          \"postalCode\": { \"type\": \"string\" },\n          \"country\": { \"type\": \"string\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/json-schema/charmhealth-patient-schema.json
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
title: CharmHealth FHIR Patient
---
