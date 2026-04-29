---
description: Schema representing a construction project in the CMiC ERP system.
layout: schema
name: CMiC Construction Project
properties_list:
- description: Unique project identifier in CMiC
  name: projectId
  type: string
- description: Project name
  name: projectName
  type: string
- description: CMiC company code for multi-company setups
  name: companyCode
  type: string
- description: Project description
  name: description
  type: string
- description: Project status
  name: status
  type: string
- description: Project manager name or employee ID
  name: projectManager
  type: string
- description: Project owner organization name
  name: owner
  type: string
- description: Project start date
  name: startDate
  type: string
- description: Project completion date
  name: endDate
  type: string
- description: Project site address
  name: address
  type: object
- description: Project financial summary
  name: financials
  type: object
- description: List of job IDs associated with this project
  name: jobs
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: CMiC
provider_slug: cmic
schema_file: json-schema/cmic-project-schema.json
slug: cmic-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.cmic.ca/rest/schemas/project\",\n  \"title\": \"CMiC Construction Project\",\n  \"description\": \"Schema representing a construction project in the CMiC ERP system.\",\n  \"type\": \"object\",\n  \"required\": [\"projectId\", \"projectName\", \"companyCode\"],\n  \"properties\": {\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique project identifier in CMiC\"\n    },\n    \"projectName\": {\n      \"type\": \"string\",\n      \"description\": \"Project name\",\n      \"maxLength\": 255\n    },\n    \"companyCode\": {\n      \"type\": \"string\",\n      \"description\": \"CMiC company code for multi-company setups\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Project description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Project status\",\n      \"enum\": [\"ACTIVE\"\
  , \"INACTIVE\", \"COMPLETE\", \"BIDDING\", \"ON_HOLD\"]\n    },\n    \"projectManager\": {\n      \"type\": \"string\",\n      \"description\": \"Project manager name or employee ID\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Project owner organization name\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Project start date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Project completion date\"\n    },\n    \"address\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"Project site address\"\n    },\n    \"financials\": {\n      \"$ref\": \"#/$defs/ProjectFinancials\",\n      \"description\": \"Project financial summary\"\n    },\n    \"jobs\": {\n      \"type\": \"array\",\n      \"description\": \"List of job IDs associated with this project\",\n      \"items\": {\n        \"type\": \"string\"\n \
  \     }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": { \"type\": \"string\", \"pattern\": \"^[A-Z]{2}$\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\", \"default\": \"US\" }\n      }\n    },\n    \"ProjectFinancials\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"contractAmount\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Original contract amount in USD\",\n          \"minimum\": 0\n        },\n        \"originalBudget\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\"\
  : \"Original approved budget\",\n          \"minimum\": 0\n        },\n        \"revisedBudget\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Current revised budget including change orders\",\n          \"minimum\": 0\n        },\n        \"actualCost\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Total actual cost incurred to date\",\n          \"minimum\": 0\n        },\n        \"committedCost\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Total committed costs (POs, subcontracts)\",\n          \"minimum\": 0\n        },\n        \"costToComplete\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Estimated cost to complete the project\"\n        },\n        \"variance\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\"\
  : \"Budget variance (positive = under budget)\"\n        },\n        \"percentComplete\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Project completion percentage\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cmic/refs/heads/main/json-schema/cmic-project-schema.json
tags:
- Construction
- ERP
- Finance
- Project Management
title: CMiC Construction Project
---
