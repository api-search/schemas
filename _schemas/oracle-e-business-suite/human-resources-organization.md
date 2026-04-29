---
description: ''
layout: schema
name: Organization
properties_list:
- description: Organization identifier
  name: organizationId
  type: integer
- description: Organization name
  name: name
  type: string
- description: Business group identifier
  name: businessGroupId
  type: integer
- description: Organization start date
  name: dateFrom
  type: string
- description: Organization end date
  name: dateTo
  type: string
- description: Location identifier
  name: locationId
  type: integer
- description: Organization type
  name: type
  type: string
- description: ''
  name: internalExternalFlag
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-organization-schema.json
slug: human-resources-organization
source_filename: human-resources-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Organization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organizationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name\"\n    },\n    \"businessGroupId\": {\n      \"type\": \"integer\",\n      \"description\": \"Business group identifier\"\n    },\n    \"dateFrom\": {\n      \"type\": \"string\",\n      \"description\": \"Organization start date\"\n    },\n    \"dateTo\": {\n      \"type\": \"string\",\n      \"description\": \"Organization end date\"\n    },\n    \"locationId\": {\n      \"type\": \"integer\",\n      \"description\": \"Location identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Organization type\"\n    },\n    \"internalExternalFlag\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-organization-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Organization
---
