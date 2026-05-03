---
description: A FHIR R4 Patient resource as represented in the Orion Health platform. Contains demographic information, identifiers, contact details, and communication preferences for an individual receiving healthcare services.
layout: schema
name: Orion Health FHIR Patient
properties_list:
- description: FHIR resource type identifier
  name: resourceType
  type: string
- description: Logical ID of the patient resource
  name: id
  type: string
- description: ''
  name: meta
  type: object
- description: Patient identifiers including MRN, SSN, and organization-specific IDs
  name: identifier
  type: array
- description: Whether the patient record is in active use
  name: active
  type: boolean
- description: Names associated with the patient
  name: name
  type: array
- description: Contact details for the patient
  name: telecom
  type: array
- description: Administrative gender
  name: gender
  type: string
- description: Date of birth
  name: birthDate
  type: string
- description: Indicates if the patient is deceased
  name: deceasedBoolean
  type: boolean
- description: Date and time of death if deceased
  name: deceasedDateTime
  type: string
- description: Addresses for the patient
  name: address
  type: array
- description: Marital status of the patient
  name: maritalStatus
  type: object
- description: Whether patient is part of a multiple birth
  name: multipleBirthBoolean
  type: boolean
- description: Birth order in a multiple birth
  name: multipleBirthInteger
  type: integer
- description: Emergency contacts and next of kin
  name: contact
  type: array
- description: Languages the patient can communicate in
  name: communication
  type: array
- description: Patient's nominated primary care provider
  name: generalPractitioner
  type: array
- description: Organization managing the patient record
  name: managingOrganization
  type: object
- description: Links to other patient resources (e.g., merged records)
  name: link
  type: array
provider_name: Orion Health
provider_slug: orion
schema_file: json-schema/orion-patient-schema.json
slug: orion-patient
source_filename: orion-patient-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.orionhealth.com/fhir/patient.json\",\n  \"title\": \"Orion Health FHIR Patient\",\n  \"description\": \"A FHIR R4 Patient resource as represented in the Orion Health platform. Contains demographic information, identifiers, contact details, and communication preferences for an individual receiving healthcare services.\",\n  \"type\": \"object\",\n  \"required\": [\"resourceType\"],\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"const\": \"Patient\",\n      \"description\": \"FHIR resource type identifier\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Logical ID of the patient resource\"\n    },\n    \"meta\": {\n      \"$ref\": \"#/$defs/Meta\"\n    },\n    \"identifier\": {\n      \"type\": \"array\",\n      \"description\": \"Patient identifiers including MRN, SSN, and organization-specific IDs\",\n      \"\
  items\": {\n        \"$ref\": \"#/$defs/Identifier\"\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the patient record is in active use\"\n    },\n    \"name\": {\n      \"type\": \"array\",\n      \"description\": \"Names associated with the patient\",\n      \"items\": {\n        \"$ref\": \"#/$defs/HumanName\"\n      }\n    },\n    \"telecom\": {\n      \"type\": \"array\",\n      \"description\": \"Contact details for the patient\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ContactPoint\"\n      }\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"enum\": [\"male\", \"female\", \"other\", \"unknown\"],\n      \"description\": \"Administrative gender\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of birth\"\n    },\n    \"deceasedBoolean\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the patient is deceased\"\n\
  \    },\n    \"deceasedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time of death if deceased\"\n    },\n    \"address\": {\n      \"type\": \"array\",\n      \"description\": \"Addresses for the patient\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Address\"\n      }\n    },\n    \"maritalStatus\": {\n      \"$ref\": \"#/$defs/CodeableConcept\",\n      \"description\": \"Marital status of the patient\"\n    },\n    \"multipleBirthBoolean\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether patient is part of a multiple birth\"\n    },\n    \"multipleBirthInteger\": {\n      \"type\": \"integer\",\n      \"description\": \"Birth order in a multiple birth\"\n    },\n    \"contact\": {\n      \"type\": \"array\",\n      \"description\": \"Emergency contacts and next of kin\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"relationship\": {\n            \"type\"\
  : \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/CodeableConcept\"\n            }\n          },\n          \"name\": {\n            \"$ref\": \"#/$defs/HumanName\"\n          },\n          \"telecom\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/ContactPoint\"\n            }\n          },\n          \"address\": {\n            \"$ref\": \"#/$defs/Address\"\n          },\n          \"gender\": {\n            \"type\": \"string\",\n            \"enum\": [\"male\", \"female\", \"other\", \"unknown\"]\n          },\n          \"organization\": {\n            \"$ref\": \"#/$defs/Reference\"\n          }\n        }\n      }\n    },\n    \"communication\": {\n      \"type\": \"array\",\n      \"description\": \"Languages the patient can communicate in\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"language\": {\n            \"$ref\": \"#/$defs/CodeableConcept\"\n      \
  \    },\n          \"preferred\": {\n            \"type\": \"boolean\"\n          }\n        },\n        \"required\": [\"language\"]\n      }\n    },\n    \"generalPractitioner\": {\n      \"type\": \"array\",\n      \"description\": \"Patient's nominated primary care provider\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Reference\"\n      }\n    },\n    \"managingOrganization\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Organization managing the patient record\"\n    },\n    \"link\": {\n      \"type\": \"array\",\n      \"description\": \"Links to other patient resources (e.g., merged records)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"other\": {\n            \"$ref\": \"#/$defs/Reference\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"replaced-by\", \"replaces\", \"refer\", \"seealso\"]\n          }\n        },\n        \"required\": [\"other\", \"\
  type\"]\n      }\n    }\n  },\n  \"$defs\": {\n    \"Meta\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"versionId\": {\n          \"type\": \"string\"\n        },\n        \"lastUpdated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"profile\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        },\n        \"security\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Coding\"\n          }\n        },\n        \"tag\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Coding\"\n          }\n        }\n      }\n    },\n    \"Identifier\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\"\
  ,\n          \"enum\": [\"usual\", \"official\", \"temp\", \"secondary\", \"old\"]\n        },\n        \"type\": {\n          \"$ref\": \"#/$defs/CodeableConcept\"\n        },\n        \"system\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Namespace for the identifier value\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier value\"\n        },\n        \"period\": {\n          \"$ref\": \"#/$defs/Period\"\n        },\n        \"assigner\": {\n          \"$ref\": \"#/$defs/Reference\"\n        }\n      }\n    },\n    \"HumanName\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"usual\", \"official\", \"temp\", \"nickname\", \"anonymous\", \"old\", \"maiden\"]\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Full text representation of the name\"\
  \n        },\n        \"family\": {\n          \"type\": \"string\",\n          \"description\": \"Family name (surname)\"\n        },\n        \"given\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Given names (first, middle)\"\n        },\n        \"prefix\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"suffix\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"period\": {\n          \"$ref\": \"#/$defs/Period\"\n        }\n      }\n    },\n    \"ContactPoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"system\": {\n          \"type\": \"string\",\n          \"enum\": [\"phone\", \"fax\", \"email\", \"pager\", \"url\", \"sms\", \"other\"]\n        },\n        \"value\": {\n          \"type\": \"string\"\n    \
  \    },\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"home\", \"work\", \"temp\", \"old\", \"mobile\"]\n        },\n        \"rank\": {\n          \"type\": \"integer\",\n          \"minimum\": 1\n        },\n        \"period\": {\n          \"$ref\": \"#/$defs/Period\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"use\": {\n          \"type\": \"string\",\n          \"enum\": [\"home\", \"work\", \"temp\", \"old\", \"billing\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"postal\", \"physical\", \"both\"]\n        },\n        \"text\": {\n          \"type\": \"string\"\n        },\n        \"line\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"district\": {\n          \"type\": \"string\"\n        },\n\
  \        \"state\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        },\n        \"period\": {\n          \"$ref\": \"#/$defs/Period\"\n        }\n      }\n    },\n    \"CodeableConcept\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"coding\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Coding\"\n          }\n        },\n        \"text\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Coding\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"system\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"version\": {\n          \"type\": \"string\"\n        },\n        \"code\": {\n          \"type\": \"string\"\n        },\n        \"display\": {\n          \"type\": \"string\"\n        },\n        \"userSelected\"\
  : {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"reference\": {\n          \"type\": \"string\",\n          \"description\": \"Relative or absolute reference to a resource\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"identifier\": {\n          \"$ref\": \"#/$defs/Identifier\"\n        },\n        \"display\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Period\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/json-schema/orion-patient-schema.json
tags:
- EHR
- FHIR
- Health IT
- Healthcare
- HIE
- HL7
- Integration
- Interoperability
- Population Health
title: Orion Health FHIR Patient
---
