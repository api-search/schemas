---
description: A FHIR R4 Observation resource as represented in the Orion Health platform. Captures measurements, test results, vital signs, and other clinical findings including laboratory results, imaging observations, and patient-reported data.
layout: schema
name: Orion Health FHIR Observation
properties_list:
- description: FHIR resource type identifier
  name: resourceType
  type: string
- description: Logical ID of the observation resource
  name: id
  type: string
- description: ''
  name: meta
  type: object
- description: ''
  name: identifier
  type: array
- description: Status of the observation
  name: status
  type: string
- description: Classification of the observation (e.g., vital-signs, laboratory)
  name: category
  type: array
- description: Type of observation (LOINC code)
  name: code
  type: object
- description: Patient the observation is about
  name: subject
  type: object
- description: Healthcare event during which observation was made
  name: encounter
  type: object
- description: Clinically relevant time for the observation
  name: effectiveDateTime
  type: string
- description: Clinically relevant time period
  name: effectivePeriod
  type: object
- description: Date/time the result was made available
  name: issued
  type: string
- description: Who performed the observation
  name: performer
  type: array
- description: Numeric result with units
  name: valueQuantity
  type: object
- description: Coded result value
  name: valueCodeableConcept
  type: object
- description: String result value
  name: valueString
  type: string
- description: Boolean result value
  name: valueBoolean
  type: boolean
- description: Integer result value
  name: valueInteger
  type: integer
- description: Date/time result value
  name: valueDateTime
  type: string
- description: Why the result is missing
  name: dataAbsentReason
  type: object
- description: High, low, normal interpretation
  name: interpretation
  type: array
- description: ''
  name: note
  type: array
- description: Body site of the observation
  name: bodySite
  type: object
- description: How the observation was performed
  name: method
  type: object
- description: Specimen used for the observation
  name: specimen
  type: object
- description: Device used to generate the observation
  name: device
  type: object
- description: Reference range for interpretation
  name: referenceRange
  type: array
- description: Component observations (e.g., systolic/diastolic for blood pressure)
  name: component
  type: array
provider_name: Orion Health
provider_slug: orion
schema_file: json-schema/orion-observation-schema.json
slug: orion-observation
source_filename: orion-observation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.orionhealth.com/fhir/observation.json\",\n  \"title\": \"Orion Health FHIR Observation\",\n  \"description\": \"A FHIR R4 Observation resource as represented in the Orion Health platform. Captures measurements, test results, vital signs, and other clinical findings including laboratory results, imaging observations, and patient-reported data.\",\n  \"type\": \"object\",\n  \"required\": [\"resourceType\", \"status\", \"code\"],\n  \"properties\": {\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"const\": \"Observation\",\n      \"description\": \"FHIR resource type identifier\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Logical ID of the observation resource\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"versionId\": {\n          \"type\": \"string\"\n        },\n        \"lastUpdated\"\
  : {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"profile\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          }\n        }\n      }\n    },\n    \"identifier\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"system\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"registered\", \"preliminary\", \"final\", \"amended\", \"corrected\", \"cancelled\", \"entered-in-error\", \"unknown\"],\n      \"description\": \"Status of the observation\"\n    },\n    \"category\": {\n      \"type\": \"array\",\n      \"description\": \"Classification of the observation (e.g., vital-signs, laboratory)\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/CodeableConcept\"\n      }\n    },\n    \"code\": {\n      \"$ref\": \"#/$defs/CodeableConcept\",\n      \"description\": \"Type of observation (LOINC code)\"\n    },\n    \"subject\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Patient the observation is about\"\n    },\n    \"encounter\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Healthcare event during which observation was made\"\n    },\n    \"effectiveDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Clinically relevant time for the observation\"\n    },\n    \"effectivePeriod\": {\n      \"$ref\": \"#/$defs/Period\",\n      \"description\": \"Clinically relevant time period\"\n    },\n    \"issued\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date/time the result was made available\"\n    },\n    \"performer\": {\n      \"type\":\
  \ \"array\",\n      \"description\": \"Who performed the observation\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Reference\"\n      }\n    },\n    \"valueQuantity\": {\n      \"$ref\": \"#/$defs/Quantity\",\n      \"description\": \"Numeric result with units\"\n    },\n    \"valueCodeableConcept\": {\n      \"$ref\": \"#/$defs/CodeableConcept\",\n      \"description\": \"Coded result value\"\n    },\n    \"valueString\": {\n      \"type\": \"string\",\n      \"description\": \"String result value\"\n    },\n    \"valueBoolean\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean result value\"\n    },\n    \"valueInteger\": {\n      \"type\": \"integer\",\n      \"description\": \"Integer result value\"\n    },\n    \"valueDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date/time result value\"\n    },\n    \"dataAbsentReason\": {\n      \"$ref\": \"#/$defs/CodeableConcept\",\n      \"description\": \"Why the\
  \ result is missing\"\n    },\n    \"interpretation\": {\n      \"type\": \"array\",\n      \"description\": \"High, low, normal interpretation\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CodeableConcept\"\n      }\n    },\n    \"note\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"text\": {\n            \"type\": \"string\"\n          },\n          \"time\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"authorReference\": {\n            \"$ref\": \"#/$defs/Reference\"\n          }\n        },\n        \"required\": [\"text\"]\n      }\n    },\n    \"bodySite\": {\n      \"$ref\": \"#/$defs/CodeableConcept\",\n      \"description\": \"Body site of the observation\"\n    },\n    \"method\": {\n      \"$ref\": \"#/$defs/CodeableConcept\",\n      \"description\": \"How the observation was performed\"\n    },\n    \"specimen\": {\n      \"$ref\": \"#/$defs/Reference\"\
  ,\n      \"description\": \"Specimen used for the observation\"\n    },\n    \"device\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Device used to generate the observation\"\n    },\n    \"referenceRange\": {\n      \"type\": \"array\",\n      \"description\": \"Reference range for interpretation\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"low\": {\n            \"$ref\": \"#/$defs/Quantity\"\n          },\n          \"high\": {\n            \"$ref\": \"#/$defs/Quantity\"\n          },\n          \"type\": {\n            \"$ref\": \"#/$defs/CodeableConcept\"\n          },\n          \"appliesTo\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/CodeableConcept\"\n            }\n          },\n          \"age\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"low\": {\n                \"$ref\": \"#/$defs/Quantity\"\n             \
  \ },\n              \"high\": {\n                \"$ref\": \"#/$defs/Quantity\"\n              }\n            }\n          },\n          \"text\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"component\": {\n      \"type\": \"array\",\n      \"description\": \"Component observations (e.g., systolic/diastolic for blood pressure)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"code\"],\n        \"properties\": {\n          \"code\": {\n            \"$ref\": \"#/$defs/CodeableConcept\"\n          },\n          \"valueQuantity\": {\n            \"$ref\": \"#/$defs/Quantity\"\n          },\n          \"valueCodeableConcept\": {\n            \"$ref\": \"#/$defs/CodeableConcept\"\n          },\n          \"valueString\": {\n            \"type\": \"string\"\n          },\n          \"interpretation\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/CodeableConcept\"\n       \
  \     }\n          },\n          \"referenceRange\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"low\": {\n                  \"$ref\": \"#/$defs/Quantity\"\n                },\n                \"high\": {\n                  \"$ref\": \"#/$defs/Quantity\"\n                },\n                \"text\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"CodeableConcept\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"coding\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Coding\"\n          }\n        },\n        \"text\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Coding\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"system\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"uri\"\n        },\n        \"code\": {\n          \"type\": \"string\"\n        },\n        \"display\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"reference\": {\n          \"type\": \"string\"\n        },\n        \"display\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Quantity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"number\"\n        },\n        \"comparator\": {\n          \"type\": \"string\",\n          \"enum\": [\"<\", \"<=\", \">=\", \">\"]\n        },\n        \"unit\": {\n          \"type\": \"string\"\n        },\n        \"system\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"code\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Period\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/json-schema/orion-observation-schema.json
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
title: Orion Health FHIR Observation
---
