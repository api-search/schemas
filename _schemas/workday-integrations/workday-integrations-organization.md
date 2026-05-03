---
description: Represents an organization in Workday, including supervisory organizations, cost centers, companies, regions, and custom organization types that form the organizational hierarchy.
layout: schema
name: Workday Organization
properties_list:
- description: Workday ID of the organization
  name: id
  type: string
- description: Display name of the organization
  name: descriptor
  type: string
- description: Type of organization
  name: organizationType
  type: string
- description: Organization reference code
  name: organizationCode
  type: string
- description: Whether the organization is currently active
  name: isActive
  type: boolean
- description: ''
  name: manager
  type: object
- description: ''
  name: superiorOrganization
  type: object
- description: Child organizations in the hierarchy
  name: subordinateOrganizations
  type: array
provider_name: Workday Integrations
provider_slug: workday-integrations
schema_file: json-schema/workday-integrations-organization-schema.json
slug: workday-integrations-organization
source_filename: workday-integrations-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-integrations/organization.json\",\n  \"title\": \"Workday Organization\",\n  \"description\": \"Represents an organization in Workday, including supervisory organizations, cost centers, companies, regions, and custom organization types that form the organizational hierarchy.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"descriptor\", \"organizationType\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Workday ID of the organization\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the organization\"\n    },\n    \"organizationType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Supervisory\", \"Cost_Center\", \"Company\", \"Region\", \"Custom\"],\n      \"description\": \"Type of organization\"\n    },\n    \"organizationCode\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"Organization reference code\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organization is currently active\"\n    },\n    \"manager\": {\n      \"$ref\": \"#/$defs/Reference\"\n    },\n    \"superiorOrganization\": {\n      \"$ref\": \"#/$defs/Reference\"\n    },\n    \"subordinateOrganizations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Reference\"\n      },\n      \"description\": \"Child organizations in the hierarchy\"\n    }\n  },\n  \"$defs\": {\n    \"Reference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a Workday business object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Workday ID of the referenced object\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the referenced object\"\
  \n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"API URL for the referenced resource\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/json-schema/workday-integrations-organization-schema.json
tags:
- Cloud
- Enterprise Software
- ERP
- Finance
- HCM
- HR
- Integration
title: Workday Organization
---
