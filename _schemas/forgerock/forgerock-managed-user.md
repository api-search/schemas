---
description: A managed user identity object stored in the ForgeRock Identity Platform repository. Represents a person with attributes for authentication, profile data, and identity lifecycle management.
layout: schema
name: ForgeRock Managed User
properties_list:
- description: Unique identifier assigned by the system
  name: _id
  type: string
- description: Object revision string for optimistic concurrency control
  name: _rev
  type: string
- description: Unique login username for the identity
  name: userName
  type: string
- description: First name / given name
  name: givenName
  type: string
- description: Last name / surname
  name: sn
  type: string
- description: Primary email address
  name: mail
  type: string
- description: Primary telephone number
  name: telephoneNumber
  type: string
- description: Password (write-only, never returned in responses)
  name: password
  type: string
- description: Current account status
  name: accountStatus
  type: string
- description: User description or notes
  name: description
  type: string
- description: City of residence
  name: city
  type: string
- description: State or province
  name: stateProvince
  type: string
- description: Postal or ZIP code
  name: postalCode
  type: string
- description: Country code (ISO 3166-1 alpha-2)
  name: country
  type: string
- description: Full postal address
  name: postalAddress
  type: string
- description: User preferences such as marketing and update opt-ins
  name: preferences
  type: object
- description: Record of user consent for data sharing
  name: consentedMappings
  type: array
- description: Knowledge-based authentication (security questions)
  name: kbaInfo
  type: array
- description: Computed effective roles for the user (virtual property)
  name: effectiveRoles
  type: array
- description: Computed effective assignments derived from roles
  name: effectiveAssignments
  type: array
- description: Information about the last synchronization event
  name: lastSync
  type: object
provider_name: ForgeRock
provider_slug: forgerock
schema_file: json-schema/forgerock-managed-user-schema.json
slug: forgerock-managed-user
source_filename: forgerock-managed-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.forgerock.com/managed-user\",\n  \"title\": \"ForgeRock Managed User\",\n  \"description\": \"A managed user identity object stored in the ForgeRock Identity Platform repository. Represents a person with attributes for authentication, profile data, and identity lifecycle management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier assigned by the system\",\n      \"readOnly\": true\n    },\n    \"_rev\": {\n      \"type\": \"string\",\n      \"description\": \"Object revision string for optimistic concurrency control\",\n      \"readOnly\": true\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Unique login username for the identity\",\n      \"minLength\": 1\n    },\n    \"givenName\": {\n      \"type\": \"string\",\n      \"description\": \"First name / given\
  \ name\"\n    },\n    \"sn\": {\n      \"type\": \"string\",\n      \"description\": \"Last name / surname\"\n    },\n    \"mail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address\"\n    },\n    \"telephoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Primary telephone number\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password (write-only, never returned in responses)\",\n      \"writeOnly\": true\n    },\n    \"accountStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current account status\",\n      \"enum\": [\"active\", \"inactive\"]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User description or notes\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City of residence\"\n    },\n    \"stateProvince\": {\n      \"type\": \"string\",\n      \"description\": \"State or province\"\
  \n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Postal or ZIP code\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (ISO 3166-1 alpha-2)\"\n    },\n    \"postalAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Full postal address\"\n    },\n    \"preferences\": {\n      \"type\": \"object\",\n      \"description\": \"User preferences such as marketing and update opt-ins\",\n      \"properties\": {\n        \"updates\": {\n          \"type\": \"boolean\",\n          \"description\": \"Opted in to receive updates\"\n        },\n        \"marketing\": {\n          \"type\": \"boolean\",\n          \"description\": \"Opted in to receive marketing communications\"\n        }\n      }\n    },\n    \"consentedMappings\": {\n      \"type\": \"array\",\n      \"description\": \"Record of user consent for data sharing\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"mapping\": {\n            \"type\": \"string\"\n          },\n          \"consentDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"kbaInfo\": {\n      \"type\": \"array\",\n      \"description\": \"Knowledge-based authentication (security questions)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"customQuestion\": {\n            \"type\": \"string\"\n          },\n          \"selectedQuestion\": {\n            \"type\": \"string\"\n          },\n          \"answer\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"effectiveRoles\": {\n      \"type\": \"array\",\n      \"description\": \"Computed effective roles for the user (virtual property)\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"_ref\": {\n            \"type\": \"string\"\n \
  \         }\n        }\n      }\n    },\n    \"effectiveAssignments\": {\n      \"type\": \"array\",\n      \"description\": \"Computed effective assignments derived from roles\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"lastSync\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the last synchronization event\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"effectiveAssignments\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  },\n  \"required\": [\"userName\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/json-schema/forgerock-managed-user-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
title: ForgeRock Managed User
---
