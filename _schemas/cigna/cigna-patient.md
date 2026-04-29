---
description: FHIR R4 Patient resource as exposed by the Cigna Patient Access API. Aligned with the US Core Patient profile referenced by the HL7 Da Vinci PDex implementation guide.
layout: schema
name: CignaPatient
properties_list:
- description: ''
  name: resourceType
  type: string
- description: Logical identifier of the Patient resource.
  name: id
  type: string
- description: ''
  name: identifier
  type: array
- description: ''
  name: active
  type: boolean
- description: ''
  name: name
  type: array
- description: ''
  name: telecom
  type: array
- description: ''
  name: gender
  type: string
- description: ''
  name: birthDate
  type: string
- description: ''
  name: address
  type: array
- description: ''
  name: communication
  type: array
provider_name: Cigna
provider_slug: cigna
schema_file: json-schema/cigna-patient-schema.json
slug: cigna-patient
source_filename: cigna-patient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/json-schema/cigna-patient-schema.json\",\n  \"title\": \"CignaPatient\",\n  \"description\": \"FHIR R4 Patient resource as exposed by the Cigna Patient Access API. Aligned with the US Core Patient profile referenced by the HL7 Da Vinci PDex implementation guide.\",\n  \"type\": \"object\",\n  \"required\": [\"resourceType\", \"id\"],\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"const\": \"Patient\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Logical identifier of the Patient resource.\"\n    },\n    \"identifier\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"system\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"active\"\
  : { \"type\": \"boolean\" },\n    \"name\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"use\": { \"type\": \"string\" },\n          \"family\": { \"type\": \"string\" },\n          \"given\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          }\n        }\n      }\n    },\n    \"telecom\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"system\": { \"type\": \"string\" },\n          \"value\": { \"type\": \"string\" },\n          \"use\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\"male\", \"female\", \"other\", \"unknown\"]\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"address\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n \
  \       \"properties\": {\n          \"use\": { \"type\": \"string\" },\n          \"line\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" }\n          },\n          \"city\": { \"type\": \"string\" },\n          \"state\": { \"type\": \"string\" },\n          \"postalCode\": { \"type\": \"string\" },\n          \"country\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"communication\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"language\": { \"type\": \"object\" },\n          \"preferred\": { \"type\": \"boolean\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/json-schema/cigna-patient-schema.json
tags:
- CMS Interoperability
- Da Vinci
- Drug Formulary
- FHIR
- Health Insurance
- Healthcare
- Patient Access
- Provider Directory
- SMART on FHIR
title: CignaPatient
---
