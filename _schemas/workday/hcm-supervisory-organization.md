---
description: ''
layout: schema
name: SupervisoryOrganization
properties_list:
- description: The Workday ID of the organization.
  name: id
  type: string
- description: A display descriptor for the organization.
  name: descriptor
  type: string
- description: The name of the supervisory organization.
  name: name
  type: string
- description: The organization reference ID.
  name: code
  type: string
- description: Whether the organization is inactive.
  name: isInactive
  type: boolean
- description: The staffing model for the organization.
  name: staffingModel
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/hcm-supervisory-organization-schema.json
slug: hcm-supervisory-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SupervisoryOrganization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the organization.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the organization.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the supervisory organization.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The organization reference ID.\"\n    },\n    \"isInactive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organization is inactive.\"\n    },\n    \"staffingModel\": {\n      \"type\": \"string\",\n      \"description\": \"The staffing model for the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/hcm-supervisory-organization-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: SupervisoryOrganization
---
