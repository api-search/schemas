---
description: Schema for a PointClickCare long-term care resident/patient record with demographic and admission data.
layout: schema
name: PointClickCare Patient
properties_list:
- description: PointClickCare system-generated patient identifier
  name: patientId
  type: string
- description: Facility where the patient resides
  name: facilityId
  type: string
- description: Medical record number
  name: mrn
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: middleName
  type: string
- description: ''
  name: dateOfBirth
  type: string
- description: M=Male, F=Female, U=Unknown/Not specified
  name: gender
  type: string
- description: Current admission status
  name: status
  type: string
- description: Date of most recent admission
  name: admissionDate
  type: string
- description: Discharge date if applicable
  name: dischargeDate
  type:
  - string
  - 'null'
- description: Unit or wing identifier
  name: unitId
  type: string
- description: ''
  name: roomNumber
  type: string
- description: ''
  name: bedNumber
  type: string
- description: Primary payer type
  name: payerType
  type: string
- description: Advance directive status
  name: advanceDirective
  type: string
- description: Preferred language (BCP 47 language tag)
  name: language
  type: string
- description: Known allergies
  name: allergies
  type: array
- description: ''
  name: primaryPhysician
  type: object
- description: ''
  name: lastUpdateDatetime
  type: string
provider_name: PointClickCare
provider_slug: pointclickcare
schema_file: json-schema/pointclickcare-patient-schema.json
slug: pointclickcare-patient
source_filename: pointclickcare-patient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/pointclickcare/json-schema/pointclickcare-patient-schema.json\",\n  \"title\": \"PointClickCare Patient\",\n  \"description\": \"Schema for a PointClickCare long-term care resident/patient record with demographic and admission data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"patientId\": {\n      \"type\": \"string\",\n      \"description\": \"PointClickCare system-generated patient identifier\"\n    },\n    \"facilityId\": {\n      \"type\": \"string\",\n      \"description\": \"Facility where the patient resides\"\n    },\n    \"mrn\": {\n      \"type\": \"string\",\n      \"description\": \"Medical record number\"\n    },\n    \"firstName\": {\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"type\": \"string\"\n    },\n    \"middleName\": {\n      \"type\": \"string\"\n    },\n    \"dateOfBirth\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"date\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\"M\", \"F\", \"U\"],\n      \"description\": \"M=Male, F=Female, U=Unknown/Not specified\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"ACTIVE\", \"DISCHARGED\", \"DECEASED\", \"RESPITE\", \"LOA\"],\n      \"description\": \"Current admission status\"\n    },\n    \"admissionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of most recent admission\"\n    },\n    \"dischargeDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Discharge date if applicable\"\n    },\n    \"unitId\": {\n      \"type\": \"string\",\n      \"description\": \"Unit or wing identifier\"\n    },\n    \"roomNumber\": {\n      \"type\": \"string\"\n    },\n    \"bedNumber\": {\n      \"type\": \"string\"\n    },\n    \"payerType\": {\n      \"type\": \"string\",\n      \"enum\": [\"\
  MEDICARE\", \"MEDICAID\", \"PRIVATE_PAY\", \"INSURANCE\", \"VA\"],\n      \"description\": \"Primary payer type\"\n    },\n    \"advanceDirective\": {\n      \"type\": \"string\",\n      \"enum\": [\"FULL_CODE\", \"DNR\", \"DNI\", \"COMFORT_CARE\", \"UNKNOWN\"],\n      \"description\": \"Advance directive status\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred language (BCP 47 language tag)\"\n    },\n    \"allergies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Known allergies\"\n    },\n    \"primaryPhysician\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"npi\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"lastUpdateDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"patientId\", \"facilityId\", \"firstName\", \"lastName\", \"dateOfBirth\"\
  , \"status\", \"admissionDate\"],\n  \"examples\": [\n    {\n      \"patientId\": \"PCC-FAC001-12345\",\n      \"facilityId\": \"FAC001\",\n      \"mrn\": \"MRN-98765\",\n      \"firstName\": \"Margaret\",\n      \"lastName\": \"Johnson\",\n      \"dateOfBirth\": \"1938-05-12\",\n      \"gender\": \"F\",\n      \"status\": \"ACTIVE\",\n      \"admissionDate\": \"2025-11-03\",\n      \"unitId\": \"UNIT-A\",\n      \"roomNumber\": \"104\",\n      \"bedNumber\": \"A\",\n      \"payerType\": \"MEDICARE\",\n      \"advanceDirective\": \"DNR\",\n      \"language\": \"en\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/json-schema/pointclickcare-patient-schema.json
tags:
- Healthcare
- Long-Term Care
- Post-Acute Care
- EHR
- FHIR
- Senior Care
- Interoperability
title: PointClickCare Patient
---
