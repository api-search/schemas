---
description: A chemical or biologic substance, used as a medical therapy, that has a physiological effect on an organism.
layout: schema
name: Schema.org Drug
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the drug.
  name: name
  type: string
- description: A description of the drug.
  name: description
  type: string
- description: URL with information about the drug.
  name: url
  type: string
- description: An alias for the drug (e.g., brand names, generic names).
  name: alternateName
  type: object
- description: The generic name of this drug or supplement.
  name: nonProprietaryName
  type: string
- description: The proprietary name of this drug.
  name: proprietaryName
  type: string
- description: An active ingredient, typically chemical compounds and/or biologic substances.
  name: activeIngredient
  type: object
- description: The class of drug this belongs to.
  name: drugClass
  type: object
- description: A route by which this drug may be administered (e.g., oral, intravenous, topical).
  name: administrationRoute
  type: string
- description: A dosage form in which this drug/supplement is available (e.g., tablet, capsule, injection).
  name: dosageForm
  type: string
- description: A dosing schedule for the drug.
  name: doseSchedule
  type: object
- description: Recommended intake of this supplement for a given population.
  name: maximumIntake
  type: object
- description: The specific biochemical interaction through which this drug or supplement produces its pharmacological effect.
  name: mechanismOfAction
  type: string
- description: Another drug that is known to interact with this drug.
  name: interactingDrug
  type: object
- description: Any precaution, guidance, contraindication, etc. related to consumption of specific foods.
  name: foodWarning
  type: string
- description: Any precaution, guidance, contraindication, etc. related to consumption of alcohol.
  name: alcoholWarning
  type: string
- description: Any precaution, guidance, contraindication, etc. related to this drug's use during pregnancy.
  name: pregnancyWarning
  type: string
- description: Any precaution, guidance, contraindication, etc. related to this drug's use by breastfeeding mothers.
  name: breastfeedingWarning
  type: string
- description: Any FDA or other warnings about the drug.
  name: warning
  type: string
- description: Any information related to overdose on a drug.
  name: overdosage
  type: string
- description: Description of the absorption and elimination of drugs.
  name: clinicalPharmacology
  type: string
- description: An available dosage strength for the drug.
  name: availableStrength
  type: object
- description: True if this item's name is a proprietary/brand name.
  name: isProprietary
  type: boolean
- description: True if the drug is available in a generic form.
  name: isAvailableGenerically
  type: boolean
- description: Indicates whether this drug is available by prescription or over-the-counter.
  name: prescriptionStatus
  type: string
- description: The drug or supplement's legal status.
  name: legalStatus
  type: string
- description: The manufacturer of the product.
  name: manufacturer
  type: object
- description: A medical code for the drug.
  name: code
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-drug-schema.json
slug: schema-org-drug
source_filename: schema-org-drug-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/drug.json\",\n  \"title\": \"Schema.org Drug\",\n  \"description\": \"A chemical or biologic substance, used as a medical therapy, that has a physiological effect on an organism.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"Drug\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the drug.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the drug.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL with information about the drug.\"\n    },\n    \"alternateName\"\
  : {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"An alias for the drug (e.g., brand names, generic names).\"\n    },\n    \"nonProprietaryName\": {\n      \"type\": \"string\",\n      \"description\": \"The generic name of this drug or supplement.\"\n    },\n    \"proprietaryName\": {\n      \"type\": \"string\",\n      \"description\": \"The proprietary name of this drug.\"\n    },\n    \"activeIngredient\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"An active ingredient, typically chemical compounds and/or biologic substances.\"\n    },\n    \"drugClass\": {\n      \"type\": \"object\",\n      \"description\": \"The class of drug this belongs to.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"DrugClass\" },\n     \
  \   \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"administrationRoute\": {\n      \"type\": \"string\",\n      \"description\": \"A route by which this drug may be administered (e.g., oral, intravenous, topical).\"\n    },\n    \"dosageForm\": {\n      \"type\": \"string\",\n      \"description\": \"A dosage form in which this drug/supplement is available (e.g., tablet, capsule, injection).\"\n    },\n    \"doseSchedule\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/DoseSchedule\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/DoseSchedule\" } }\n      ],\n      \"description\": \"A dosing schedule for the drug.\"\n    },\n    \"maximumIntake\": {\n      \"$ref\": \"#/$defs/MaximumDoseSchedule\",\n      \"description\": \"Recommended intake of this supplement for a given population.\"\n    },\n    \"mechanismOfAction\": {\n      \"type\": \"string\",\n      \"description\": \"The specific biochemical interaction through which this drug or supplement\
  \ produces its pharmacological effect.\"\n    },\n    \"interactingDrug\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"Another drug that is known to interact with this drug.\"\n    },\n    \"foodWarning\": {\n      \"type\": \"string\",\n      \"description\": \"Any precaution, guidance, contraindication, etc. related to consumption of specific foods.\"\n    },\n    \"alcoholWarning\": {\n      \"type\": \"string\",\n      \"description\": \"Any precaution, guidance, contraindication, etc. related to consumption of alcohol.\"\n    },\n    \"pregnancyWarning\": {\n      \"type\": \"string\",\n      \"description\": \"Any precaution, guidance, contraindication, etc. related to this drug's use during pregnancy.\"\n    },\n    \"breastfeedingWarning\": {\n      \"type\": \"string\",\n      \"description\": \"Any precaution, guidance, contraindication, etc. related to this drug's use\
  \ by breastfeeding mothers.\"\n    },\n    \"warning\": {\n      \"type\": \"string\",\n      \"description\": \"Any FDA or other warnings about the drug.\"\n    },\n    \"overdosage\": {\n      \"type\": \"string\",\n      \"description\": \"Any information related to overdose on a drug.\"\n    },\n    \"clinicalPharmacology\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the absorption and elimination of drugs.\"\n    },\n    \"availableStrength\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/DrugStrength\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/DrugStrength\" } }\n      ],\n      \"description\": \"An available dosage strength for the drug.\"\n    },\n    \"isProprietary\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if this item's name is a proprietary/brand name.\"\n    },\n    \"isAvailableGenerically\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the drug is available in a generic\
  \ form.\"\n    },\n    \"prescriptionStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"OTC\", \"PrescriptionOnly\"],\n      \"description\": \"Indicates whether this drug is available by prescription or over-the-counter.\"\n    },\n    \"legalStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The drug or supplement's legal status.\"\n    },\n    \"manufacturer\": {\n      \"$ref\": \"schema-org-organization-schema.json\",\n      \"description\": \"The manufacturer of the product.\"\n    },\n    \"code\": {\n      \"type\": \"object\",\n      \"description\": \"A medical code for the drug.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MedicalCode\" },\n        \"codeValue\": { \"type\": \"string\" },\n        \"codingSystem\": { \"type\": \"string\" }\n      }\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\"\
  , \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  },\n  \"$defs\": {\n    \"DoseSchedule\": {\n      \"type\": \"object\",\n      \"description\": \"A specific dosing schedule for a drug or supplement.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"enum\": [\"DoseSchedule\", \"MaximumDoseSchedule\", \"RecommendedDoseSchedule\", \"ReportedDoseSchedule\"] },\n        \"doseUnit\": { \"type\": \"string\", \"description\": \"The unit of the dose (e.g., mg).\" },\n        \"doseValue\": { \"type\": \"number\", \"description\": \"The value of the dose.\" },\n        \"frequency\": { \"type\": \"string\", \"description\": \"How often the dose is taken.\" },\n        \"targetPopulation\": { \"type\": \"string\", \"description\": \"Characteristics of the population for which this is intended.\" }\n      }\n    },\n    \"MaximumDoseSchedule\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"The maximum dosing schedule considered safe.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MaximumDoseSchedule\" },\n        \"doseUnit\": { \"type\": \"string\" },\n        \"doseValue\": { \"type\": \"number\" },\n        \"frequency\": { \"type\": \"string\" },\n        \"targetPopulation\": { \"type\": \"string\" }\n      }\n    },\n    \"DrugStrength\": {\n      \"type\": \"object\",\n      \"description\": \"A specific strength in which a medical drug is available.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"DrugStrength\" },\n        \"activeIngredient\": { \"type\": \"string\" },\n        \"strengthUnit\": { \"type\": \"string\" },\n        \"strengthValue\": { \"type\": \"number\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-drug-schema.json
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
title: Schema.org Drug
---
