---
description: Represents a security domain in the Gravitee Access Management platform that defines authentication and authorization boundaries for applications and users.
layout: schema
name: Gravitee Security Domain
properties_list:
- description: Unique identifier for the security domain.
  name: id
  type: string
- description: Name of the security domain.
  name: name
  type: string
- description: Description of the security domain.
  name: description
  type: string
- description: Whether the domain is currently active and processing requests.
  name: enabled
  type: boolean
- description: Context path for the domain used in URL routing.
  name: path
  type: string
- description: OpenID Connect protocol configuration.
  name: oidc
  type: object
- description: SCIM protocol configuration for user provisioning.
  name: scim
  type: object
- description: Login page customization settings.
  name: loginSettings
  type: object
- description: Timestamp when the domain was created.
  name: createdAt
  type: string
- description: Timestamp when the domain was last updated.
  name: updatedAt
  type: string
provider_name: Gravitee
provider_slug: gravitee
schema_file: json-schema/gravitee-domain-schema.json
slug: gravitee-domain
source_filename: gravitee-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://gravitee.io/schemas/gravitee/domain.json\",\n  \"title\": \"Gravitee Security Domain\",\n  \"description\": \"Represents a security domain in the Gravitee Access Management platform that defines authentication and authorization boundaries for applications and users.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the security domain.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the security domain.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the security domain.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is currently active and processing requests.\",\n      \"default\": true\n\
  \    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Context path for the domain used in URL routing.\"\n    },\n    \"oidc\": {\n      \"type\": \"object\",\n      \"description\": \"OpenID Connect protocol configuration.\",\n      \"additionalProperties\": true\n    },\n    \"scim\": {\n      \"type\": \"object\",\n      \"description\": \"SCIM protocol configuration for user provisioning.\",\n      \"additionalProperties\": true\n    },\n    \"loginSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Login page customization settings.\",\n      \"properties\": {\n        \"inherited\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether settings are inherited from the organization level.\"\n        },\n        \"forgotPasswordEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the forgot password feature is enabled.\"\n        },\n        \"registerEnabled\": {\n          \"type\": \"boolean\"\
  ,\n          \"description\": \"Whether self-registration is enabled.\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the domain was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the domain was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/json-schema/gravitee-domain-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Gravitee Security Domain
---
