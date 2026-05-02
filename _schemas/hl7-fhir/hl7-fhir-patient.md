---
description: JSON Schema for the HL7 FHIR R4 Patient resource. Represents a person receiving care, including demographics, identifiers, and contact information. Based on https://www.hl7.org/fhir/R4/patient.html
layout: schema
name: HL7 FHIR R4 Patient
properties_list:
- description: FHIR resource type discriminator
  name: resourceType
  type: string
- description: Logical id of this artifact (server-assigned)
  name: id
  type: string
- description: ''
  name: meta
  type: object
- description: ''
  name: text
  type: object
- description: ''
  name: extension
  type: array
- description: Patient identifiers (MRN, SSN, driver's license, etc.)
  name: identifier
  type: array
- description: Whether this patient record is in active use
  name: active
  type: boolean
- description: A name associated with the patient
  name: name
  type: array
- description: Contact details (phone, email) for the patient
  name: telecom
  type: array
- description: Administrative gender
  name: gender
  type: string
- description: Patient date of birth
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
  name: multipleBirthBoolean
  type: boolean
- description: ''
  name: multipleBirthInteger
  type: integer
- description: ''
  name: photo
  type: array
- description: Emergency contacts and next of kin
  name: contact
  type: array
- description: ''
  name: communication
  type: array
- description: Patient's nominated primary care provider
  name: generalPractitioner
  type: array
- description: Organization that is the custodian of the patient record
  name: managingOrganization
  type: object
- description: ''
  name: link
  type: array
provider_name: HL7 FHIR
provider_slug: hl7-fhir
schema_file: json-schema/hl7-fhir-patient-schema.json
slug: hl7-fhir-patient
source_filename: hl7-fhir-patient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/hl7-fhir/json-schema/hl7-fhir-patient-schema.json\",\n  \"title\": \"HL7 FHIR R4 Patient\",\n  \"description\": \"JSON Schema for the HL7 FHIR R4 Patient resource. Represents a person receiving care, including demographics, identifiers, and contact information. Based on https://www.hl7.org/fhir/R4/patient.html\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"const\": \"Patient\",\n      \"description\": \"FHIR resource type discriminator\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Logical id of this artifact (server-assigned)\"\n    },\n    \"meta\": { \"$ref\": \"#/$defs/Meta\" },\n    \"text\": { \"$ref\": \"#/$defs/Narrative\" },\n    \"extension\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Extension\" }\n    },\n    \"identifier\":\
  \ {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Identifier\" },\n      \"description\": \"Patient identifiers (MRN, SSN, driver's license, etc.)\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this patient record is in active use\"\n    },\n    \"name\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/HumanName\" },\n      \"description\": \"A name associated with the patient\"\n    },\n    \"telecom\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/ContactPoint\" },\n      \"description\": \"Contact details (phone, email) for the patient\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\"male\", \"female\", \"other\", \"unknown\"],\n      \"description\": \"Administrative gender\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Patient date of birth\"\n    },\n    \"deceasedBoolean\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"deceasedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"address\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Address\" }\n    },\n    \"maritalStatus\": { \"$ref\": \"#/$defs/CodeableConcept\" },\n    \"multipleBirthBoolean\": {\n      \"type\": \"boolean\"\n    },\n    \"multipleBirthInteger\": {\n      \"type\": \"integer\"\n    },\n    \"photo\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Attachment\" }\n    },\n    \"contact\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/PatientContact\" },\n      \"description\": \"Emergency contacts and next of kin\"\n    },\n    \"communication\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"language\": { \"$ref\": \"#/$defs/CodeableConcept\" },\n          \"preferred\": { \"type\": \"boolean\" }\n   \
  \     },\n        \"required\": [\"language\"]\n      }\n    },\n    \"generalPractitioner\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Reference\" },\n      \"description\": \"Patient's nominated primary care provider\"\n    },\n    \"managingOrganization\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Organization that is the custodian of the patient record\"\n    },\n    \"link\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"other\": { \"$ref\": \"#/$defs/Reference\" },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"replaced-by\", \"replaces\", \"refer\", \"seealso\"]\n          }\n        },\n        \"required\": [\"other\", \"type\"]\n      }\n    }\n  },\n  \"required\": [\"resourceType\"],\n  \"$defs\": {\n    \"Meta\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"versionId\": { \"type\": \"string\"\
  \ },\n        \"lastUpdated\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"source\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"profile\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\", \"format\": \"uri\" }\n        }\n      }\n    },\n    \"Narrative\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"generated\", \"extensions\", \"additional\", \"empty\"]\n        },\n        \"div\": { \"type\": \"string\", \"description\": \"XHTML narrative content\" }\n      },\n      \"required\": [\"status\", \"div\"]\n    },\n    \"Extension\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"valueString\": { \"type\": \"string\" },\n        \"valueBoolean\": { \"type\": \"boolean\" },\n        \"valueCode\": { \"type\": \"string\" },\n        \"valueCodeableConcept\"\
  : { \"$ref\": \"#/$defs/CodeableConcept\" }\n      },\n      \"required\": [\"url\"]\n    },\n    \"Identifier\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"usual\", \"official\", \"temp\", \"secondary\", \"old\"]\n        },\n        \"type\": { \"$ref\": \"#/$defs/CodeableConcept\" },\n        \"system\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"value\": { \"type\": \"string\" }\n      }\n    },\n    \"HumanName\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"usual\", \"official\", \"temp\", \"nickname\", \"anonymous\", \"old\", \"maiden\"]\n        },\n        \"text\": { \"type\": \"string\", \"description\": \"Full text of the name\" },\n        \"family\": { \"type\": \"string\", \"description\": \"Family name (surname)\" },\n        \"given\": {\n          \"type\": \"array\",\n        \
  \  \"items\": { \"type\": \"string\" },\n          \"description\": \"Given names (forenames, including middle names)\"\n        },\n        \"prefix\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"suffix\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"ContactPoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"system\": {\n          \"type\": \"string\",\n          \"enum\": [\"phone\", \"fax\", \"email\", \"pager\", \"url\", \"sms\", \"other\"]\n        },\n        \"value\": { \"type\": \"string\" },\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"home\", \"work\", \"temp\", \"old\", \"mobile\"]\n        },\n        \"rank\": { \"type\": \"integer\", \"minimum\": 1 }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\"\
  ,\n          \"enum\": [\"home\", \"work\", \"temp\", \"old\", \"billing\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"postal\", \"physical\", \"both\"]\n        },\n        \"text\": { \"type\": \"string\" },\n        \"line\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"city\": { \"type\": \"string\" },\n        \"district\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\" }\n      }\n    },\n    \"CodeableConcept\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"coding\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/Coding\" }\n        },\n        \"text\": { \"type\": \"string\" }\n      }\n    },\n    \"Coding\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"system\": { \"type\": \"string\"\
  , \"format\": \"uri\" },\n        \"version\": { \"type\": \"string\" },\n        \"code\": { \"type\": \"string\" },\n        \"display\": { \"type\": \"string\" },\n        \"userSelected\": { \"type\": \"boolean\" }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"reference\": { \"type\": \"string\" },\n        \"type\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"identifier\": { \"$ref\": \"#/$defs/Identifier\" },\n        \"display\": { \"type\": \"string\" }\n      }\n    },\n    \"Attachment\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"contentType\": { \"type\": \"string\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"title\": { \"type\": \"string\" }\n      }\n    },\n    \"PatientContact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"relationship\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/CodeableConcept\"\
  \ }\n        },\n        \"name\": { \"$ref\": \"#/$defs/HumanName\" },\n        \"telecom\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/ContactPoint\" }\n        },\n        \"address\": { \"$ref\": \"#/$defs/Address\" },\n        \"gender\": {\n          \"type\": \"string\",\n          \"enum\": [\"male\", \"female\", \"other\", \"unknown\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hl7-fhir/refs/heads/main/json-schema/hl7-fhir-patient-schema.json
tags:
- Clinical
- FHIR
- Healthcare
- HL7
- Interoperability
title: HL7 FHIR R4 Patient
---
