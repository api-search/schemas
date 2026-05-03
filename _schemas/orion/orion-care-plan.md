---
description: Represents a care plan within the Orion Health Population Health Management platform, defining care goals, activities, and interventions for a patient enrolled in a care program.
layout: schema
name: Orion Health Population Health Care Plan
properties_list:
- description: Unique care plan identifier
  name: id
  type: string
- description: Patient identifier
  name: patientId
  type: string
- description: Associated care program identifier
  name: programId
  type: string
- description: Name of the associated care program
  name: programName
  type: string
- description: Current status of the care plan
  name: status
  type: string
- description: Level of authority for the care plan
  name: intent
  type: string
- description: Human-readable title for the care plan
  name: title
  type: string
- description: Summary of the care plan
  name: description
  type: string
- description: ''
  name: period
  type: object
- description: Members of the care team responsible for this plan
  name: careTeam
  type: array
- description: Conditions addressed by this care plan
  name: conditions
  type: array
- description: Care plan goals
  name: goals
  type: array
- description: Planned care activities and interventions
  name: activities
  type: array
- description: Current risk assessment for the patient
  name: riskAssessment
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: createdBy
  type: string
provider_name: Orion Health
provider_slug: orion
schema_file: json-schema/orion-care-plan-schema.json
slug: orion-care-plan
source_filename: orion-care-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.orionhealth.com/population-health/care-plan.json\",\n  \"title\": \"Orion Health Population Health Care Plan\",\n  \"description\": \"Represents a care plan within the Orion Health Population Health Management platform, defining care goals, activities, and interventions for a patient enrolled in a care program.\",\n  \"type\": \"object\",\n  \"required\": [\"patientId\", \"programId\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique care plan identifier\"\n    },\n    \"patientId\": {\n      \"type\": \"string\",\n      \"description\": \"Patient identifier\"\n    },\n    \"programId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Associated care program identifier\"\n    },\n    \"programName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Name of the associated care program\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"active\", \"on-hold\", \"completed\", \"revoked\"],\n      \"description\": \"Current status of the care plan\"\n    },\n    \"intent\": {\n      \"type\": \"string\",\n      \"enum\": [\"proposal\", \"plan\", \"order\"],\n      \"description\": \"Level of authority for the care plan\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable title for the care plan\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Summary of the care plan\"\n    },\n    \"period\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Care plan start date\"\n        },\n        \"end\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\":\
  \ \"Care plan end date\"\n        }\n      },\n      \"required\": [\"start\"]\n    },\n    \"careTeam\": {\n      \"type\": \"array\",\n      \"description\": \"Members of the care team responsible for this plan\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"memberId\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"role\": {\n            \"type\": \"string\",\n            \"enum\": [\"primary-care-physician\", \"care-manager\", \"specialist\", \"nurse\", \"social-worker\", \"pharmacist\", \"dietitian\", \"behavioral-health\"]\n          },\n          \"organization\": {\n            \"type\": \"string\"\n          },\n          \"phone\": {\n            \"type\": \"string\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"format\": \"email\"\n          }\n        },\n        \"required\": [\"memberId\", \"name\",\
  \ \"role\"]\n      }\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"description\": \"Conditions addressed by this care plan\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"ICD-10 or SNOMED code\"\n          },\n          \"codeSystem\": {\n            \"type\": \"string\",\n            \"enum\": [\"icd-10\", \"snomed\"]\n          },\n          \"display\": {\n            \"type\": \"string\"\n          },\n          \"clinicalStatus\": {\n            \"type\": \"string\",\n            \"enum\": [\"active\", \"recurrence\", \"relapse\", \"inactive\", \"remission\", \"resolved\"]\n          }\n        },\n        \"required\": [\"code\", \"display\"]\n      }\n    },\n    \"goals\": {\n      \"type\": \"array\",\n      \"description\": \"Care plan goals\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"\
  id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\"proposed\", \"planned\", \"accepted\", \"active\", \"on-hold\", \"completed\", \"cancelled\", \"entered-in-error\", \"rejected\"]\n          },\n          \"priority\": {\n            \"type\": \"string\",\n            \"enum\": [\"high\", \"medium\", \"low\"]\n          },\n          \"targetDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"targetValue\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"measure\": {\n                \"type\": \"string\",\n                \"description\": \"What is being measured (e.g., HbA1c, BMI, Blood Pressure)\"\n              },\n              \"targetValue\": {\n                \"type\": \"number\"\n     \
  \         },\n              \"unit\": {\n                \"type\": \"string\"\n              },\n              \"currentValue\": {\n                \"type\": \"number\"\n              },\n              \"currentValueDate\": {\n                \"type\": \"string\",\n                \"format\": \"date\"\n              }\n            }\n          },\n          \"achievedDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"notes\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"text\": {\n                  \"type\": \"string\"\n                },\n                \"authorName\": {\n                  \"type\": \"string\"\n                },\n                \"date\": {\n                  \"type\": \"string\",\n                  \"format\": \"date-time\"\n                }\n              }\n            }\n          }\n        },\n      \
  \  \"required\": [\"description\", \"status\"]\n      }\n    },\n    \"activities\": {\n      \"type\": \"array\",\n      \"description\": \"Planned care activities and interventions\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"enum\": [\"medication\", \"procedure\", \"encounter\", \"observation\", \"education\", \"referral\", \"self-management\", \"assessment\"]\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\"not-started\", \"scheduled\", \"in-progress\", \"on-hold\", \"completed\", \"cancelled\"]\n          },\n          \"frequency\": {\n            \"type\": \"string\",\n            \"description\": \"How often the activity should occur (e.g.,\
  \ daily, weekly, monthly)\"\n          },\n          \"scheduledDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"completedDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"assignedTo\": {\n            \"type\": \"string\",\n            \"description\": \"Care team member responsible\"\n          },\n          \"relatedGoalId\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\",\n            \"description\": \"Goal this activity contributes to\"\n          }\n        },\n        \"required\": [\"category\", \"description\", \"status\"]\n      }\n    },\n    \"riskAssessment\": {\n      \"type\": \"object\",\n      \"description\": \"Current risk assessment for the patient\",\n      \"properties\": {\n        \"riskLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\"low\", \"moderate\", \"high\", \"critical\"]\n        },\n        \"riskScore\"\
  : {\n          \"type\": \"number\"\n        },\n        \"model\": {\n          \"type\": \"string\"\n        },\n        \"assessedDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/json-schema/orion-care-plan-schema.json
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
title: Orion Health Population Health Care Plan
---
