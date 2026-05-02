---
description: FHIR R4 Patient resource as implemented by Meditech Expanse (US Core Patient Profile)
layout: schema
name: Meditech FHIR R4 Patient
properties_list:
- description: ''
  name: resourceType
  type: string
- description: FHIR logical ID
  name: id
  type: string
- description: ''
  name: meta
  type: object
- description: Patient identifiers (MRN, SSN, etc.)
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
  name: deceasedBoolean
  type: boolean
- description: ''
  name: deceasedDateTime
  type: string
- description: ''
  name: address
  type: array
- description: ''
  name: maritalStatus
  type: object
- description: ''
  name: communication
  type: array
- description: ''
  name: generalPractitioner
  type: array
- description: ''
  name: managingOrganization
  type: object
provider_name: meditech
provider_slug: meditech
schema_file: json-schema/meditech-patient-schema.json
slug: meditech-patient
source_filename: meditech-patient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/json-schema/meditech-patient-schema.json\",\n  \"title\": \"Meditech FHIR R4 Patient\",\n  \"description\": \"FHIR R4 Patient resource as implemented by Meditech Expanse (US Core Patient Profile)\",\n  \"type\": \"object\",\n  \"required\": [\"resourceType\", \"id\"],\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"const\": \"Patient\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"FHIR logical ID\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"versionId\": { \"type\": \"string\" },\n        \"lastUpdated\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"profile\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\", \"format\": \"uri\" }\n        }\n      }\n    },\n\
  \    \"identifier\": {\n      \"type\": \"array\",\n      \"description\": \"Patient identifiers (MRN, SSN, etc.)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Identifier\"\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/HumanName\"\n      }\n    },\n    \"telecom\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ContactPoint\"\n      }\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\"male\", \"female\", \"other\", \"unknown\"]\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"deceasedBoolean\": {\n      \"type\": \"boolean\"\n    },\n    \"deceasedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"address\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Address\"\n      }\n    },\n\
  \    \"maritalStatus\": {\n      \"$ref\": \"#/$defs/CodeableConcept\"\n    },\n    \"communication\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"language\"],\n        \"properties\": {\n          \"language\": { \"$ref\": \"#/$defs/CodeableConcept\" },\n          \"preferred\": { \"type\": \"boolean\" }\n        }\n      }\n    },\n    \"generalPractitioner\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Reference\" }\n    },\n    \"managingOrganization\": {\n      \"$ref\": \"#/$defs/Reference\"\n    }\n  },\n  \"$defs\": {\n    \"Identifier\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"usual\", \"official\", \"temp\", \"secondary\", \"old\"]\n        },\n        \"type\": { \"$ref\": \"#/$defs/CodeableConcept\" },\n        \"system\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"value\": { \"type\"\
  : \"string\" }\n      }\n    },\n    \"HumanName\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"usual\", \"official\", \"temp\", \"nickname\", \"anonymous\", \"old\", \"maiden\"]\n        },\n        \"family\": { \"type\": \"string\" },\n        \"given\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"prefix\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"suffix\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"ContactPoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"system\": {\n          \"type\": \"string\",\n          \"enum\": [\"phone\", \"fax\", \"email\", \"pager\", \"url\", \"sms\", \"other\"]\n        },\n        \"value\": { \"type\": \"string\" },\n        \"use\": {\n        \
  \  \"type\": \"string\",\n          \"enum\": [\"home\", \"work\", \"temp\", \"old\", \"mobile\"]\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"home\", \"work\", \"temp\", \"old\", \"billing\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"postal\", \"physical\", \"both\"]\n        },\n        \"line\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"city\": { \"type\": \"string\" },\n        \"district\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\" }\n      }\n    },\n    \"CodeableConcept\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"coding\": {\n          \"type\": \"array\",\n          \"items\": {\n       \
  \     \"type\": \"object\",\n            \"properties\": {\n              \"system\": { \"type\": \"string\", \"format\": \"uri\" },\n              \"version\": { \"type\": \"string\" },\n              \"code\": { \"type\": \"string\" },\n              \"display\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"text\": { \"type\": \"string\" }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"reference\": { \"type\": \"string\" },\n        \"type\": { \"type\": \"string\" },\n        \"display\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/json-schema/meditech-patient-schema.json
tags: []
title: Meditech FHIR R4 Patient
---
