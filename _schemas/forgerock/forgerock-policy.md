---
description: An authorization policy in ForgeRock Access Management that defines access control rules for resources. Policies specify which subjects can perform which actions on which resources under what conditions.
layout: schema
name: ForgeRock Authorization Policy
properties_list:
- description: Unique policy name within the policy set
  name: name
  type: string
- description: Whether the policy is currently active and enforced
  name: active
  type: boolean
- description: Human-readable description of the policy
  name: description
  type: string
- description: The policy set (application) this policy belongs to
  name: applicationName
  type: string
- description: Map of action names to their allowed/denied values
  name: actionValues
  type: object
- description: Resource patterns this policy applies to (may include wildcards)
  name: resources
  type: array
- description: Subject condition defining who this policy applies to
  name: subject
  type: object
- description: Environment condition defining when this policy applies
  name: condition
  type: object
- description: UUID of the resource type associated with this policy
  name: resourceTypeUuid
  type: string
- description: Response attributes to include in policy decisions
  name: resourceAttributes
  type: array
- description: User who created the policy
  name: createdBy
  type: string
- description: Creation timestamp in milliseconds since epoch
  name: creationDate
  type: integer
- description: User who last modified the policy
  name: lastModifiedBy
  type: string
- description: Last modification timestamp in milliseconds since epoch
  name: lastModifiedDate
  type: integer
provider_name: ForgeRock
provider_slug: forgerock
schema_file: json-schema/forgerock-policy-schema.json
slug: forgerock-policy
source_filename: forgerock-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.forgerock.com/policy\",\n  \"title\": \"ForgeRock Authorization Policy\",\n  \"description\": \"An authorization policy in ForgeRock Access Management that defines access control rules for resources. Policies specify which subjects can perform which actions on which resources under what conditions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique policy name within the policy set\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy is currently active and enforced\",\n      \"default\": true\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the policy\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"The policy set (application) this policy belongs\
  \ to\"\n    },\n    \"actionValues\": {\n      \"type\": \"object\",\n      \"description\": \"Map of action names to their allowed/denied values\",\n      \"additionalProperties\": {\n        \"type\": \"boolean\"\n      },\n      \"examples\": [\n        {\n          \"GET\": true,\n          \"POST\": true,\n          \"DELETE\": false\n        }\n      ]\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"Resource patterns this policy applies to (may include wildcards)\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"https://api.example.com/resource/*\"]\n      ]\n    },\n    \"subject\": {\n      \"type\": \"object\",\n      \"description\": \"Subject condition defining who this policy applies to\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Subject condition type\",\n          \"enum\": [\n            \"Identity\",\n            \"AuthenticatedUsers\"\
  ,\n            \"JwtClaim\",\n            \"AND\",\n            \"OR\",\n            \"NOT\",\n            \"NONE\"\n          ]\n        },\n        \"subjectValues\": {\n          \"type\": \"array\",\n          \"description\": \"Values for the subject condition (e.g., user/group IDs)\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"condition\": {\n      \"type\": \"object\",\n      \"description\": \"Environment condition defining when this policy applies\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Condition type\",\n          \"enum\": [\n            \"AND\",\n            \"OR\",\n            \"NOT\",\n            \"IP\",\n            \"IPv4\",\n            \"IPv6\",\n            \"SimpleTime\",\n            \"LEAuthLevel\",\n            \"AuthLevel\",\n            \"AuthScheme\",\n            \"AuthenticateToService\",\n            \"AuthenticateToRealm\"\
  ,\n            \"Script\",\n            \"OAuth2Scope\",\n            \"ResourceEnvIP\"\n          ]\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"resourceTypeUuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"UUID of the resource type associated with this policy\"\n    },\n    \"resourceAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"Response attributes to include in policy decisions\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"propertyName\": {\n            \"type\": \"string\"\n          },\n          \"propertyValues\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the policy\"\
  ,\n      \"readOnly\": true\n    },\n    \"creationDate\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation timestamp in milliseconds since epoch\",\n      \"readOnly\": true\n    },\n    \"lastModifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who last modified the policy\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"integer\",\n      \"description\": \"Last modification timestamp in milliseconds since epoch\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"name\", \"resources\", \"applicationName\", \"resourceTypeUuid\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/json-schema/forgerock-policy-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
title: ForgeRock Authorization Policy
---
