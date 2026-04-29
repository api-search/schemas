---
description: Represents an organization in Workday. Organizations include supervisory organizations, cost centers, companies, regions, and other organizational types used to structure the enterprise.
layout: schema
name: Organization
properties_list:
- description: The Workday ID of the organization.
  name: id
  type: string
- description: A display descriptor for the organization.
  name: descriptor
  type: string
- description: The name of the organization.
  name: name
  type: string
- description: The organization reference ID or code.
  name: code
  type: string
- description: The type of organization (e.g., Supervisory, Cost Center, Company, Region).
  name: organizationType
  type: object
- description: The sub-type of the organization.
  name: organizationSubType
  type: object
- description: The parent organization in the hierarchy.
  name: superiorOrganization
  type: object
- description: The manager of the organization.
  name: manager
  type: object
- description: The primary location of the organization.
  name: location
  type: object
- description: The staffing model (e.g., Position Management, Job Management).
  name: staffingModel
  type: string
- description: The number of members in the organization.
  name: memberCount
  type: integer
- description: Subordinate organizations in the hierarchy.
  name: subordinateOrganizations
  type: array
- description: Positions within this organization.
  name: positions
  type: array
- description: Workers assigned to this organization.
  name: workers
  type: array
- description: Whether the organization is inactive.
  name: isInactive
  type: boolean
- description: Whether to include inactive subordinate organizations.
  name: includeInactiveSubOrganizations
  type: boolean
- description: The date the organization becomes available.
  name: availabilityDate
  type:
  - string
  - 'null'
- description: The last time the organization was updated.
  name: lastUpdated
  type: string
- description: An external system identifier for the organization.
  name: externalID
  type: string
- description: A link to the full organization resource.
  name: href
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/organization.json
slug: organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://workday.com/schemas/organization.json\",\n  \"title\": \"Organization\",\n  \"description\": \"Represents an organization in Workday. Organizations include supervisory organizations, cost centers, companies, regions, and other organizational types used to structure the enterprise.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the organization.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the organization.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the organization.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The organization reference ID or code.\"\n    },\n    \"organizationType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"\
  description\": \"The type of organization (e.g., Supervisory, Cost Center, Company, Region).\"\n    },\n    \"organizationSubType\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The sub-type of the organization.\"\n    },\n    \"superiorOrganization\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The parent organization in the hierarchy.\"\n    },\n    \"manager\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The manager of the organization.\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The primary location of the organization.\"\n    },\n    \"staffingModel\": {\n      \"type\": \"string\",\n      \"description\": \"The staffing model (e.g., Position Management, Job Management).\",\n      \"enum\": [\"Position_Management\", \"Job_Management\"]\n    },\n    \"memberCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number\
  \ of members in the organization.\"\n    },\n    \"subordinateOrganizations\": {\n      \"type\": \"array\",\n      \"description\": \"Subordinate organizations in the hierarchy.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ResourceReference\"\n      }\n    },\n    \"positions\": {\n      \"type\": \"array\",\n      \"description\": \"Positions within this organization.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ResourceReference\"\n      }\n    },\n    \"workers\": {\n      \"type\": \"array\",\n      \"description\": \"Workers assigned to this organization.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ResourceReference\"\n      }\n    },\n    \"isInactive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organization is inactive.\"\n    },\n    \"includeInactiveSubOrganizations\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to include inactive subordinate organizations.\"\n    },\n    \"availabilityDate\": {\n      \"\
  type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The date the organization becomes available.\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last time the organization was updated.\"\n    },\n    \"externalID\": {\n      \"type\": \"string\",\n      \"description\": \"An external system identifier for the organization.\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A link to the full organization resource.\"\n    }\n  },\n  \"required\": [\"id\", \"descriptor\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Workday resource.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The Workday ID of the referenced resource.\"\n        },\n        \"descriptor\": {\n          \"type\":\
  \ \"string\",\n          \"description\": \"A display descriptor for the referenced resource.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A link to the referenced resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/organization.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: Organization
---
