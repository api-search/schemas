---
description: Schema for a change management project managed using Prosci's methodology. A change project represents an organizational change initiative with associated stakeholders, assessments, and change plans.
layout: schema
name: Prosci Change Project
properties_list:
- description: Unique identifier for the project
  name: id
  type: string
- description: Name of the change project
  name: name
  type: string
- description: Detailed description of the change initiative including objectives and expected outcomes
  name: description
  type: string
- description: Current lifecycle status of the project
  name: status
  type: string
- description: Category of organizational change
  name: changeType
  type: string
- description: Organizational scope of the change initiative
  name: scope
  type: string
- description: Executive sponsor responsible for championing the change
  name: sponsor
  type: object
- description: Change management practitioner leading the change effort
  name: changeManager
  type: object
- description: Groups of employees impacted by the change
  name: impactedGroups
  type: array
- description: Total number of employees impacted by the change
  name: impactedEmployeeCount
  type: integer
- description: Overall assessed risk level of the change initiative
  name: riskLevel
  type: string
- description: Current phase in Prosci's 3-Phase Process
  name: phase
  type: string
- description: Project start date
  name: startDate
  type: string
- description: Target completion date for the change initiative
  name: targetCompletionDate
  type: string
- description: Actual completion date, if completed
  name: actualCompletionDate
  type: string
- description: Identifier of the parent organization
  name: organizationId
  type: string
- description: Name of the parent organization
  name: organizationName
  type: string
- description: Key objectives of the change initiative
  name: objectives
  type: array
- description: Metrics used to measure the success of the change
  name: successMetrics
  type: array
- description: Tags for categorization and search
  name: tags
  type: array
- description: Timestamp when the project was created
  name: createdAt
  type: string
- description: Timestamp when the project was last updated
  name: updatedAt
  type: string
provider_name: Prosci
provider_slug: prosci
schema_file: json-schema/prosci-change-project-schema.json
slug: prosci-change-project
source_filename: prosci-change-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.prosci.com/schemas/change-project.json\",\n  \"title\": \"Prosci Change Project\",\n  \"description\": \"Schema for a change management project managed using Prosci's methodology. A change project represents an organizational change initiative with associated stakeholders, assessments, and change plans.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the project\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the change project\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the change initiative including objectives and expected outcomes\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"planning\",\n        \"active\",\n        \"completed\",\n  \
  \      \"on-hold\",\n        \"cancelled\"\n      ],\n      \"description\": \"Current lifecycle status of the project\"\n    },\n    \"changeType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"process\",\n        \"technology\",\n        \"organizational\",\n        \"cultural\",\n        \"merger-acquisition\",\n        \"strategic\"\n      ],\n      \"description\": \"Category of organizational change\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"department\",\n        \"division\",\n        \"organization\",\n        \"enterprise\"\n      ],\n      \"description\": \"Organizational scope of the change initiative\"\n    },\n    \"sponsor\": {\n      \"type\": \"object\",\n      \"description\": \"Executive sponsor responsible for championing the change\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the sponsor\"\n        },\n        \"name\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Full name of the executive sponsor\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Job title of the sponsor\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address of the sponsor\"\n        }\n      },\n      \"required\": [\n        \"name\"\n      ]\n    },\n    \"changeManager\": {\n      \"type\": \"object\",\n      \"description\": \"Change management practitioner leading the change effort\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the change manager\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the change manager\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n       \
  \   \"description\": \"Email address of the change manager\"\n        },\n        \"certificationLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"certified-change-practitioner\",\n            \"certified-change-management-professional\",\n            \"certified-instructor\"\n          ],\n          \"description\": \"Prosci certification level held by the change manager\"\n        }\n      },\n      \"required\": [\n        \"name\"\n      ]\n    },\n    \"impactedGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the impacted group\"\n          },\n          \"size\": {\n            \"type\": \"integer\",\n            \"minimum\": 0,\n            \"description\": \"Number of people in the group\"\n          },\n          \"impactLevel\": {\n            \"type\": \"string\",\n            \"\
  enum\": [\n              \"low\",\n              \"moderate\",\n              \"high\",\n              \"critical\"\n            ],\n            \"description\": \"Degree to which this group is impacted by the change\"\n          },\n          \"department\": {\n            \"type\": \"string\",\n            \"description\": \"Department or business unit\"\n          }\n        },\n        \"required\": [\n          \"name\"\n        ]\n      },\n      \"description\": \"Groups of employees impacted by the change\"\n    },\n    \"impactedEmployeeCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total number of employees impacted by the change\"\n    },\n    \"riskLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"low\",\n        \"moderate\",\n        \"high\",\n        \"critical\"\n      ],\n      \"description\": \"Overall assessed risk level of the change initiative\"\n    },\n    \"phase\": {\n      \"type\": \"string\",\n\
  \      \"enum\": [\n        \"preparing-for-change\",\n        \"managing-change\",\n        \"reinforcing-change\"\n      ],\n      \"description\": \"Current phase in Prosci's 3-Phase Process\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Project start date\"\n    },\n    \"targetCompletionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Target completion date for the change initiative\"\n    },\n    \"actualCompletionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Actual completion date, if completed\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent organization\"\n    },\n    \"organizationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the parent organization\"\n    },\n    \"objectives\": {\n      \"type\": \"array\",\n      \"items\"\
  : {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key objectives of the change initiative\"\n    },\n    \"successMetrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the metric\"\n          },\n          \"target\": {\n            \"type\": \"string\",\n            \"description\": \"Target value for the metric\"\n          },\n          \"current\": {\n            \"type\": \"string\",\n            \"description\": \"Current value of the metric\"\n          },\n          \"unit\": {\n            \"type\": \"string\",\n            \"description\": \"Unit of measurement\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"target\"\n        ]\n      },\n      \"description\": \"Metrics used to measure the success of the change\"\n    },\n    \"tags\": {\n      \"type\": \"\
  array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags for categorization and search\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was last updated\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"status\",\n    \"changeType\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/json-schema/prosci-change-project-schema.json
tags:
- Change Management
- Methodology
- Training
title: Prosci Change Project
---
