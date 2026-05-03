---
description: A process of care used in either a diagnostic, therapeutic, preventive or palliative capacity that relies on invasive, non-invasive, or other techniques.
layout: schema
name: Schema.org MedicalProcedure
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the procedure.
  name: name
  type: string
- description: A description of the procedure.
  name: description
  type: string
- description: URL with information about the procedure.
  name: url
  type: string
- description: The type of procedure, for example Surgical, Noninvasive, or Percutaneous.
  name: procedureType
  type: string
- description: Location in the body of the anatomical structure.
  name: bodyLocation
  type: string
- description: Typical preparation that a patient must undergo before having the procedure performed.
  name: preparation
  type: string
- description: Typical or recommended followup care after the procedure is performed.
  name: followup
  type: string
- description: How the procedure is performed.
  name: howPerformed
  type: string
- description: The status of the procedure.
  name: status
  type: string
- description: A medical code for the procedure.
  name: code
  type: object
- description: A dosing schedule for the procedure (for therapeutic procedures).
  name: doseSchedule
  type: object
- description: Specifying a drug or medicine used in a medication procedure.
  name: drug
  type: object
- description: A possible complication and/or side effect of this therapy.
  name: adverseOutcome
  type: object
- description: A contraindication for this therapy.
  name: contraindication
  type: string
- description: A therapy that duplicates or overlaps this one.
  name: duplicateTherapy
  type: object
- description: A possible serious complication and/or serious side effect of this therapy.
  name: seriousAdverseOutcome
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-medical-procedure-schema.json
slug: schema-org-medical-procedure
source_filename: schema-org-medical-procedure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/medical-procedure.json\",\n  \"title\": \"Schema.org MedicalProcedure\",\n  \"description\": \"A process of care used in either a diagnostic, therapeutic, preventive or palliative capacity that relies on invasive, non-invasive, or other techniques.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"MedicalProcedure\", \"DiagnosticProcedure\", \"PalliativeProcedure\", \"PhysicalExam\", \"SurgicalProcedure\", \"TherapeuticProcedure\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the procedure.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"A description of the procedure.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL with information about the procedure.\"\n    },\n    \"procedureType\": {\n      \"type\": \"string\",\n      \"enum\": [\"NoninvasiveProcedure\", \"PercutaneousProcedure\", \"SurgicalProcedure\"],\n      \"description\": \"The type of procedure, for example Surgical, Noninvasive, or Percutaneous.\"\n    },\n    \"bodyLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Location in the body of the anatomical structure.\"\n    },\n    \"preparation\": {\n      \"type\": \"string\",\n      \"description\": \"Typical preparation that a patient must undergo before having the procedure performed.\"\n    },\n    \"followup\": {\n      \"type\": \"string\",\n      \"description\": \"Typical or recommended followup care after the procedure is performed.\"\n    },\n    \"howPerformed\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"How the procedure is performed.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"EvidenceNotAssessed\", \"MedicalEvidenceLevel\", \"TreatmentActive\", \"TreatmentComplete\", \"TreatmentDiscontinued\", \"TreatmentNotApplicable\", \"TreatmentPending\", \"TreatmentStopped\"],\n      \"description\": \"The status of the procedure.\"\n    },\n    \"code\": {\n      \"type\": \"object\",\n      \"description\": \"A medical code for the procedure.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MedicalCode\" },\n        \"codeValue\": { \"type\": \"string\", \"description\": \"The actual code.\" },\n        \"codingSystem\": { \"type\": \"string\", \"description\": \"The coding system (e.g., ICD-10-PCS, CPT).\" }\n      }\n    },\n    \"doseSchedule\": {\n      \"type\": \"object\",\n      \"description\": \"A dosing schedule for the procedure (for therapeutic procedures).\",\n      \"properties\": {\n        \"@type\": { \"\
  type\": \"string\", \"const\": \"DoseSchedule\" },\n        \"doseUnit\": { \"type\": \"string\" },\n        \"doseValue\": { \"type\": \"number\" },\n        \"frequency\": { \"type\": \"string\" }\n      }\n    },\n    \"drug\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-drug-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-drug-schema.json\" } }\n      ],\n      \"description\": \"Specifying a drug or medicine used in a medication procedure.\"\n    },\n    \"adverseOutcome\": {\n      \"type\": \"object\",\n      \"description\": \"A possible complication and/or side effect of this therapy.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MedicalEntity\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"contraindication\": {\n      \"type\": \"string\",\n      \"description\": \"A contraindication for this therapy.\"\n    },\n    \"duplicateTherapy\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"A therapy that duplicates or overlaps this one.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"seriousAdverseOutcome\": {\n      \"type\": \"object\",\n      \"description\": \"A possible serious complication and/or serious side effect of this therapy.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MedicalEntity\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-medical-procedure-schema.json
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
title: Schema.org MedicalProcedure
---
