---
description: Represents an organizational unit within the Workday system, including supervisory organizations, cost centers, companies, and regions.
layout: schema
name: Organization
properties_list:
- description: The unique Workday identifier for the organization
  name: id
  type: string
- description: The display name of the organization
  name: descriptor
  type: string
- description: The type of organization (Supervisory, Cost Center, Company, etc.)
  name: organizationType
  type: object
- description: The unique code for the organization
  name: organizationCode
  type: string
- description: Whether the organization is currently active
  name: isActive
  type: boolean
- description: The manager of the organization
  name: manager
  type: object
- description: The parent organization in the hierarchy
  name: superior
  type: object
- description: The staffing model used by the organization (Position Management or Job Management)
  name: staffingModel
  type: string
- description: The date the organization configuration became effective
  name: effectiveDate
  type: string
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-organization-schema.json
slug: workday-integration-organization
source_filename: workday-integration-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/organization\",\n  \"title\": \"Organization\",\n  \"description\": \"Represents an organizational unit within the Workday system, including supervisory organizations, cost centers, companies, and regions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the organization\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the organization\"\n    },\n    \"organizationType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The type of organization (Supervisory, Cost Center, Company, etc.)\"\n    },\n    \"organizationCode\": {\n      \"type\": \"string\",\n      \"description\": \"The unique code for the organization\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n   \
  \   \"description\": \"Whether the organization is currently active\"\n    },\n    \"manager\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The manager of the organization\"\n    },\n    \"superior\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The parent organization in the hierarchy\"\n    },\n    \"staffingModel\": {\n      \"type\": \"string\",\n      \"description\": \"The staffing model used by the organization (Position Management or Job Management)\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the organization configuration became effective\"\n    }\n  },\n  \"required\": [\"id\", \"descriptor\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\"\n        },\n    \
  \    \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-organization-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Organization
---
