---
description: Represents a job profile definition within the Workday system, defining the qualifications, responsibilities, and classification for positions.
layout: schema
name: Job Profile
properties_list:
- description: The unique Workday identifier for the job profile
  name: id
  type: string
- description: The display name of the job profile
  name: descriptor
  type: string
- description: The name of the job profile
  name: jobProfileName
  type: string
- description: The job family this profile belongs to
  name: jobFamily
  type: object
- description: The management level classification
  name: managementLevel
  type: object
- description: The job category classification
  name: jobCategory
  type: object
- description: Whether the job profile is currently active
  name: isActive
  type: boolean
- description: Whether this is classified as a critical job
  name: isCriticalJob
  type: boolean
- description: A summary description of the job profile
  name: summary
  type: string
- description: The effective date of the job profile
  name: effectiveDate
  type: string
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-job-profile-schema.json
slug: workday-integration-job-profile
source_filename: workday-integration-job-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/jobProfile\",\n  \"title\": \"Job Profile\",\n  \"description\": \"Represents a job profile definition within the Workday system, defining the qualifications, responsibilities, and classification for positions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the job profile\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the job profile\"\n    },\n    \"jobProfileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job profile\"\n    },\n    \"jobFamily\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The job family this profile belongs to\"\n    },\n    \"managementLevel\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\"\
  : \"The management level classification\"\n    },\n    \"jobCategory\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The job category classification\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the job profile is currently active\"\n    },\n    \"isCriticalJob\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is classified as a critical job\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"A summary description of the job profile\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The effective date of the job profile\"\n    }\n  },\n  \"required\": [\"id\", \"descriptor\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\"\
  : \"string\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-job-profile-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Job Profile
---
