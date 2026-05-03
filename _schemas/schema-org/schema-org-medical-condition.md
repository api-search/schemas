---
description: Any condition of the human body that affects the normal functioning of a person, whether physically or mentally.
layout: schema
name: Schema.org MedicalCondition
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the condition.
  name: name
  type: string
- description: A description of the condition.
  name: description
  type: string
- description: URL with information about the condition.
  name: url
  type: string
- description: An alias for the condition.
  name: alternateName
  type: object
- description: A medical code for the condition.
  name: code
  type: object
- description: The anatomy or anatomical system affected.
  name: associatedAnatomy
  type: object
- description: One of a set of differential diagnoses for the condition.
  name: differentialDiagnosis
  type: object
- description: A sign or symptom of this condition.
  name: signOrSymptom
  type: object
- description: A possible treatment to address this condition.
  name: possibleTreatment
  type: object
- description: A modifiable or non-modifiable factor that increases the risk of a patient contracting this condition.
  name: riskFactor
  type: object
- description: The likely outcome in either the short or long term.
  name: expectedPrognosis
  type: string
- description: The expected progression of the condition if it is not treated.
  name: naturalProgression
  type: string
- description: The stage of the condition.
  name: stage
  type: object
- description: The status of the condition.
  name: status
  type: string
- description: The characteristics of associated patients, such as age, gender, race etc.
  name: epidemiology
  type: string
- description: Changes in the normal mechanical, physical, and biochemical functions.
  name: pathophysiology
  type: string
- description: A medical test typically performed given this condition.
  name: typicalTest
  type: object
- description: A preventative therapy used to prevent an initial occurrence of the medical condition.
  name: primaryPrevention
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-medical-condition-schema.json
slug: schema-org-medical-condition
source_filename: schema-org-medical-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/medical-condition.json\",\n  \"title\": \"Schema.org MedicalCondition\",\n  \"description\": \"Any condition of the human body that affects the normal functioning of a person, whether physically or mentally.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"MedicalCondition\", \"InfectiousDisease\", \"MedicalSignOrSymptom\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the condition.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the condition.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"uri\",\n      \"description\": \"URL with information about the condition.\"\n    },\n    \"alternateName\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"An alias for the condition.\"\n    },\n    \"code\": {\n      \"$ref\": \"#/$defs/MedicalCode\",\n      \"description\": \"A medical code for the condition.\"\n    },\n    \"associatedAnatomy\": {\n      \"type\": \"object\",\n      \"description\": \"The anatomy or anatomical system affected.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"enum\": [\"AnatomicalStructure\", \"AnatomicalSystem\", \"SuperficialAnatomy\"] },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"differentialDiagnosis\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/DDxElement\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/DDxElement\" } }\n      ],\n      \"description\"\
  : \"One of a set of differential diagnoses for the condition.\"\n    },\n    \"signOrSymptom\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/MedicalSignOrSymptom\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/MedicalSignOrSymptom\" } }\n      ],\n      \"description\": \"A sign or symptom of this condition.\"\n    },\n    \"possibleTreatment\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/MedicalTherapy\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/MedicalTherapy\" } }\n      ],\n      \"description\": \"A possible treatment to address this condition.\"\n    },\n    \"riskFactor\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/MedicalRiskFactor\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/MedicalRiskFactor\" } }\n      ],\n      \"description\": \"A modifiable or non-modifiable factor that increases the risk of a patient contracting this condition.\"\n    },\n    \"expectedPrognosis\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"The likely outcome in either the short or long term.\"\n    },\n    \"naturalProgression\": {\n      \"type\": \"string\",\n      \"description\": \"The expected progression of the condition if it is not treated.\"\n    },\n    \"stage\": {\n      \"type\": \"object\",\n      \"description\": \"The stage of the condition.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MedicalConditionStage\" },\n        \"stageAsNumber\": { \"type\": \"number\" },\n        \"subStageSuffix\": { \"type\": \"string\" }\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"EvidenceNotAssessed\", \"MedicalEvidenceLevel\", \"TreatmentActive\", \"TreatmentComplete\", \"TreatmentDiscontinued\", \"TreatmentNotApplicable\", \"TreatmentPending\", \"TreatmentStopped\"],\n      \"description\": \"The status of the condition.\"\n    },\n    \"epidemiology\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"The characteristics of associated patients, such as age, gender, race etc.\"\n    },\n    \"pathophysiology\": {\n      \"type\": \"string\",\n      \"description\": \"Changes in the normal mechanical, physical, and biochemical functions.\"\n    },\n    \"typicalTest\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/MedicalTest\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/MedicalTest\" } }\n      ],\n      \"description\": \"A medical test typically performed given this condition.\"\n    },\n    \"primaryPrevention\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/MedicalTherapy\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/MedicalTherapy\" } }\n      ],\n      \"description\": \"A preventative therapy used to prevent an initial occurrence of the medical condition.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\"\
  : { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  },\n  \"$defs\": {\n    \"MedicalCode\": {\n      \"type\": \"object\",\n      \"description\": \"A code for a medical entity.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MedicalCode\" },\n        \"codeValue\": { \"type\": \"string\", \"description\": \"The actual code.\" },\n        \"codingSystem\": { \"type\": \"string\", \"description\": \"The coding system (e.g., ICD-10, SNOMED CT).\" }\n      }\n    },\n    \"DDxElement\": {\n      \"type\": \"object\",\n      \"description\": \"An alternative, closely-related condition to consider as part of differential diagnosis.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"DDxElement\" },\n        \"diagnosis\": { \"$ref\": \"#\", \"description\": \"The condition being considered.\" },\n \
  \       \"distinguishingSign\": { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/MedicalSignOrSymptom\" } }\n      }\n    },\n    \"MedicalSignOrSymptom\": {\n      \"type\": \"object\",\n      \"description\": \"Any feature associated or not with a medical condition.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"enum\": [\"MedicalSign\", \"MedicalSymptom\", \"MedicalSignOrSymptom\"] },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the sign or symptom.\" },\n        \"possibleTreatment\": { \"type\": \"object\", \"properties\": { \"@type\": { \"type\": \"string\" }, \"name\": { \"type\": \"string\" } } }\n      }\n    },\n    \"MedicalTherapy\": {\n      \"type\": \"object\",\n      \"description\": \"Any medical intervention designed to prevent, treat, and cure human diseases and medical conditions.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"enum\": [\"MedicalTherapy\", \"DrugTherapy\", \"PhysicalTherapy\"\
  , \"RadiationTherapy\"] },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the therapy.\" },\n        \"description\": { \"type\": \"string\", \"description\": \"A description of the therapy.\" }\n      }\n    },\n    \"MedicalRiskFactor\": {\n      \"type\": \"object\",\n      \"description\": \"A risk factor is anything that increases a person's likelihood of developing or contracting a disease, medical condition, or complication.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MedicalRiskFactor\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the risk factor.\" },\n        \"increasesRiskOf\": { \"type\": \"object\", \"properties\": { \"@type\": { \"type\": \"string\" }, \"name\": { \"type\": \"string\" } } }\n      }\n    },\n    \"MedicalTest\": {\n      \"type\": \"object\",\n      \"description\": \"Any medical test, typically used for diagnosis.\",\n      \"properties\": {\n        \"@type\"\
  : { \"type\": \"string\", \"enum\": [\"MedicalTest\", \"BloodTest\", \"ImagingTest\", \"PathologyTest\"] },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the test.\" },\n        \"usedToDiagnose\": { \"type\": \"object\", \"properties\": { \"@type\": { \"type\": \"string\" }, \"name\": { \"type\": \"string\" } } }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-medical-condition-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org MedicalCondition
---
