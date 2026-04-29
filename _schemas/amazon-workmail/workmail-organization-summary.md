---
description: The representation of an organization.
layout: schema
name: OrganizationSummary
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: Alias
  type: object
- description: ''
  name: DefaultMailDomain
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-organization-summary-schema.json
slug: workmail-organization-summary
source_filename: workmail-organization-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier associated with the organization.\"\n        }\n      ]\n    },\n    \"Alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationName\"\n        },\n        {\n          \"description\": \"The alias associated with the organization.\"\n        }\n      ]\n    },\n    \"DefaultMailDomain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The default email domain associated with the organization.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error message associated\
  \ with the organization. It is only present if unexpected behavior has occurred with regards to the organization. It provides insight or solutions regarding unexpected behavior.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The state associated with the organization.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The representation of an organization.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrganizationSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-organization-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-organization-summary-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: OrganizationSummary
---
