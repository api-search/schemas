---
description: ''
layout: schema
name: UserResource
properties_list:
- description: ''
  name: schemas
  type: array
- description: ''
  name: id
  type: string
- description: ''
  name: externalId
  type: string
- description: Unique identifier for the User, typically used by the user to directly authenticate to the service provider. Each User MUST include a non-empty userName value. This identifier MUST be unique across th
  name: userName
  type: string
- description: The components of the user's real name. Providers MAY return just the full name as a single string in the formatted sub-attribute, or they MAY return just the individual component attributes using the
  name: name
  type: object
- description: Email addresses for the user. The value SHOULD be canonicalized by the service provider, e.g., 'bjensen@example.com' instead of 'bjensen@EXAMPLE.COM'.
  name: email
  type: string
- description: Phone numbers for the User. The value SHOULD be canonicalized by the service provider according to the format specified in RFC 3966, e.g., 'tel:+1-201-555-0123'. Canonical type values of 'main', 'work
  name: phoneNumbers
  type: array
- description: A list of groups to which the user belongs, either through direct membership, through nested groups, or dynamically calculated.
  name: groups
  type: array
- description: ''
  name: urn:scim:schemas:extension:FactSet:Core:1.0:User
  type: object
- description: ''
  name: urn:scim:schemas:extension:FactSet:VRS:1.0:User
  type: object
- description: ''
  name: meta
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-procure-to-pay-scim-user-resource-schema.json
slug: factset-procure-to-pay-scim-user-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schemas\": {\n      \"type\": \"array\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"externalId\": {\n      \"type\": \"string\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the User, typically used by the user to directly authenticate to the service provider. Each User MUST include a non-empty userName value.  This identifier MUST be unique across the service provider's entire set of Users.\"\n    },\n    \"name\": {\n      \"type\": \"object\",\n      \"description\": \"The components of the user's real name. Providers MAY return just the full name as a single string in the formatted sub-attribute, or they MAY return just the individual component attributes using the other sub-attributes, or they MAY return both.  If both variants are returned,\
  \ they SHOULD be describing the same name, with the formatted name indicating how the component attributes should be combined.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email addresses for the user.  The value SHOULD be canonicalized by the service provider, e.g., 'bjensen@example.com' instead of 'bjensen@EXAMPLE.COM'.\"\n    },\n    \"phoneNumbers\": {\n      \"type\": \"array\",\n      \"description\": \"Phone numbers for the User.  The value SHOULD be canonicalized by the service provider according to the format specified in RFC 3966, e.g., 'tel:+1-201-555-0123'. Canonical type values of 'main', 'work', 'mobile', and 'home'.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"A list of groups to which the user belongs, either through direct membership, through nested groups, or dynamically calculated.\"\n    },\n    \"urn:scim:schemas:extension:FactSet:Core:1.0:User\": {\n      \"type\": \"object\"\n    },\n   \
  \ \"urn:scim:schemas:extension:FactSet:VRS:1.0:User\": {\n      \"type\": \"object\"\n    },\n    \"meta\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-procure-to-pay-scim-user-resource-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: UserResource
---
