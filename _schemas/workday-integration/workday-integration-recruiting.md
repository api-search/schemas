---
description: Represents a job posting within the Workday Recruiting system, including the position details, requirements, and posting status.
layout: schema
name: Job Posting
properties_list:
- description: The unique Workday identifier for the job posting
  name: id
  type: string
- description: The display name of the job posting
  name: descriptor
  type: string
- description: The title of the job posting
  name: title
  type: string
- description: The date the job was posted
  name: postingDate
  type: string
- description: The date the posting closes
  name: closingDate
  type:
  - string
  - 'null'
- description: The current status of the job posting
  name: status
  type: string
- description: The location of the job
  name: location
  type: object
- description: The associated job requisition
  name: jobRequisition
  type: object
- description: The job profile for this posting
  name: jobProfile
  type: object
- description: The hiring manager for this position
  name: hiringManager
  type: object
- description: The full job description
  name: jobDescription
  type: string
- description: Whether this is an internal-only posting
  name: isInternal
  type: boolean
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-recruiting-schema.json
slug: workday-integration-recruiting
source_filename: workday-integration-recruiting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/jobPosting\",\n  \"title\": \"Job Posting\",\n  \"description\": \"Represents a job posting within the Workday Recruiting system, including the position details, requirements, and posting status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the job posting\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the job posting\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the job posting\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the job was posted\"\n    },\n    \"closingDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"\
  The date the posting closes\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the job posting\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The location of the job\"\n    },\n    \"jobRequisition\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The associated job requisition\"\n    },\n    \"jobProfile\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The job profile for this posting\"\n    },\n    \"hiringManager\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The hiring manager for this position\"\n    },\n    \"jobDescription\": {\n      \"type\": \"string\",\n      \"description\": \"The full job description\"\n    },\n    \"isInternal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an internal-only posting\"\n    }\n  },\n  \"required\": [\"id\", \"title\"\
  ],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-recruiting-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Job Posting
---
