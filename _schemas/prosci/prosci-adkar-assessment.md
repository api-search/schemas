---
description: 'Schema for an ADKAR assessment based on Prosci''s ADKAR Model, measuring individual or group change readiness across five sequential dimensions: Awareness, Desire, Knowledge, Ability, and Reinforcement.'
layout: schema
name: Prosci ADKAR Assessment
properties_list:
- description: Unique identifier for the assessment
  name: id
  type: string
- description: Identifier of the associated change project
  name: projectId
  type: string
- description: Identifier of the assessed stakeholder or group
  name: stakeholderId
  type: string
- description: Name of the assessed stakeholder or group
  name: stakeholderName
  type: string
- description: Identifier of the impacted group
  name: groupId
  type: string
- description: Date the assessment was conducted
  name: assessmentDate
  type: string
- description: Awareness of the need for change - understanding why the change is necessary
  name: awareness
  type: object
- description: Desire to participate and support the change
  name: desire
  type: object
- description: Knowledge of how to change - understanding required skills and behaviors
  name: knowledge
  type: object
- description: Ability to implement required skills and behaviors on a day-to-day basis
  name: ability
  type: object
- description: Reinforcement to sustain the change and prevent regression
  name: reinforcement
  type: object
- description: Average score across all five ADKAR dimensions
  name: overallScore
  type: number
- description: The first ADKAR element scoring below the threshold (typically 3), indicating the primary barrier to change adoption. The ADKAR model is sequential, so barriers must be resolved in order.
  name: barrierPoint
  type: string
- description: Additional notes or observations from the assessor
  name: notes
  type: string
- description: Name or identifier of the person who conducted the assessment
  name: assessedBy
  type: string
- description: Timestamp when the assessment was created
  name: createdAt
  type: string
- description: Timestamp when the assessment was last updated
  name: updatedAt
  type: string
provider_name: Prosci
provider_slug: prosci
schema_file: json-schema/prosci-adkar-assessment-schema.json
slug: prosci-adkar-assessment
source_filename: prosci-adkar-assessment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.prosci.com/schemas/adkar-assessment.json\",\n  \"title\": \"Prosci ADKAR Assessment\",\n  \"description\": \"Schema for an ADKAR assessment based on Prosci's ADKAR Model, measuring individual or group change readiness across five sequential dimensions: Awareness, Desire, Knowledge, Ability, and Reinforcement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the assessment\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the associated change project\"\n    },\n    \"stakeholderId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the assessed stakeholder or group\"\n    },\n    \"stakeholderName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the assessed stakeholder or group\"\n    },\n    \"groupId\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the impacted group\"\n    },\n    \"assessmentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the assessment was conducted\"\n    },\n    \"awareness\": {\n      \"$ref\": \"#/$defs/adkarDimension\",\n      \"description\": \"Awareness of the need for change - understanding why the change is necessary\"\n    },\n    \"desire\": {\n      \"$ref\": \"#/$defs/adkarDimension\",\n      \"description\": \"Desire to participate and support the change\"\n    },\n    \"knowledge\": {\n      \"$ref\": \"#/$defs/adkarDimension\",\n      \"description\": \"Knowledge of how to change - understanding required skills and behaviors\"\n    },\n    \"ability\": {\n      \"$ref\": \"#/$defs/adkarDimension\",\n      \"description\": \"Ability to implement required skills and behaviors on a day-to-day basis\"\n    },\n    \"reinforcement\": {\n      \"$ref\": \"#/$defs/adkarDimension\"\
  ,\n      \"description\": \"Reinforcement to sustain the change and prevent regression\"\n    },\n    \"overallScore\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"maximum\": 5,\n      \"description\": \"Average score across all five ADKAR dimensions\"\n    },\n    \"barrierPoint\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"awareness\",\n        \"desire\",\n        \"knowledge\",\n        \"ability\",\n        \"reinforcement\",\n        \"none\"\n      ],\n      \"description\": \"The first ADKAR element scoring below the threshold (typically 3), indicating the primary barrier to change adoption. The ADKAR model is sequential, so barriers must be resolved in order.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Additional notes or observations from the assessor\"\n    },\n    \"assessedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Name or identifier of the person who conducted the assessment\"\n\
  \    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the assessment was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the assessment was last updated\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"projectId\",\n    \"assessmentDate\",\n    \"awareness\",\n    \"desire\",\n    \"knowledge\",\n    \"ability\",\n    \"reinforcement\"\n  ],\n  \"$defs\": {\n    \"adkarDimension\": {\n      \"type\": \"object\",\n      \"title\": \"ADKAR Dimension\",\n      \"description\": \"Score and qualitative details for a single ADKAR dimension\",\n      \"properties\": {\n        \"score\": {\n          \"type\": \"number\",\n          \"minimum\": 1,\n          \"maximum\": 5,\n          \"description\": \"Numeric score from 1 (low readiness) to 5 (high readiness). Scores of 3 or below typically indicate a barrier point\
  \ requiring targeted intervention.\"\n        },\n        \"notes\": {\n          \"type\": \"string\",\n          \"description\": \"Qualitative notes explaining the score\"\n        },\n        \"actions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Recommended corrective actions to improve this dimension\"\n        },\n        \"evidence\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Observable evidence supporting the assigned score\"\n        }\n      },\n      \"required\": [\n        \"score\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/json-schema/prosci-adkar-assessment-schema.json
tags:
- Change Management
- Methodology
- Training
title: Prosci ADKAR Assessment
---
