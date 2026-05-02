---
description: An opportunity in Microsoft Dynamics 365 CRM, representing a potential sale or deal being pursued.
layout: schema
name: Opportunity
properties_list:
- description: The unique identifier of the opportunity.
  name: opportunityid
  type: string
- description: The name or subject of the opportunity.
  name: name
  type: string
- description: Additional details about the opportunity.
  name: description
  type: string
- description: The estimated revenue value.
  name: estimatedvalue
  type: number
- description: The estimated close date.
  name: estimatedclosedate
  type: string
- description: The actual revenue value when closed.
  name: actualvalue
  type: number
- description: The actual close date.
  name: actualclosedate
  type: string
- description: The probability of closing the opportunity (0-100).
  name: closeprobability
  type: integer
- description: Description of the current situation.
  name: currentsituation
  type: string
- description: Description of the customer need.
  name: customerneed
  type: string
- description: Description of the proposed solution.
  name: proposedsolution
  type: string
- description: The current step in the sales process.
  name: stepname
  type: string
- description: The state of the opportunity (0 = Open, 1 = Won, 2 = Lost).
  name: statecode
  type: integer
- description: The status reason code.
  name: statuscode
  type: integer
- description: The date and time the opportunity was created.
  name: createdon
  type: string
- description: The date and time the opportunity was last modified.
  name: modifiedon
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/opportunity.json
slug: opportunity
source_filename: opportunity.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/opportunity.json\",\n  \"title\": \"Opportunity\",\n  \"description\": \"An opportunity in Microsoft Dynamics 365 CRM, representing a potential sale or deal being pursued.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"opportunityid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the opportunity.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name or subject of the opportunity.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details about the opportunity.\"\n    },\n    \"estimatedvalue\": {\n      \"type\": \"number\",\n      \"description\": \"The estimated revenue value.\"\n    },\n    \"estimatedclosedate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The estimated close date.\"\n    },\n    \"actualvalue\": {\n      \"type\": \"number\",\n      \"description\": \"The actual revenue value when closed.\"\n    },\n    \"actualclosedate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The actual close date.\"\n    },\n    \"closeprobability\": {\n      \"type\": \"integer\",\n      \"description\": \"The probability of closing the opportunity (0-100).\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"currentsituation\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the current situation.\"\n    },\n    \"customerneed\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the customer need.\"\n    },\n    \"proposedsolution\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the proposed solution.\"\n    },\n    \"stepname\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The current step in the sales process.\"\n    },\n    \"statecode\": {\n      \"type\": \"integer\",\n      \"description\": \"The state of the opportunity (0 = Open, 1 = Won, 2 = Lost).\"\n    },\n    \"statuscode\": {\n      \"type\": \"integer\",\n      \"description\": \"The status reason code.\"\n    },\n    \"createdon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the opportunity was created.\",\n      \"readOnly\": true\n    },\n    \"modifiedon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the opportunity was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/opportunity.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Opportunity
---
