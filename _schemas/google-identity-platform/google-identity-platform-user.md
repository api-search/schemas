---
description: Schema for a user record in Google Identity Platform, representing an authenticated user with their profile information, provider data, and authentication state.
layout: schema
name: Google Identity Platform User Record
properties_list:
- description: The unique user ID assigned by Identity Platform
  name: localId
  type: string
- description: The user's email address
  name: email
  type: string
- description: Whether the user's email has been verified
  name: emailVerified
  type: boolean
- description: The user's display name
  name: displayName
  type: string
- description: URL of the user's profile photo
  name: photoUrl
  type: string
- description: The user's phone number in E.164 format
  name: phoneNumber
  type: string
- description: Whether the user account is disabled
  name: disabled
  type: boolean
- description: Linked identity provider accounts
  name: providerUserInfo
  type: array
- description: Multi-factor authentication enrollments
  name: mfaInfo
  type: array
- description: The tenant ID if the user belongs to a specific tenant
  name: tenantId
  type: string
- description: Account creation timestamp in milliseconds since epoch
  name: createdAt
  type: string
- description: Last sign-in timestamp in milliseconds since epoch
  name: lastLoginAt
  type: string
- description: Custom claims JSON string set via Admin SDK
  name: customAttributes
  type: string
provider_name: Google Identity Platform
provider_slug: google-identity-platform
schema_file: json-schema/google-identity-platform-user-schema.json
slug: google-identity-platform-user
source_filename: google-identity-platform-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/identity-platform/user.json\",\n  \"title\": \"Google Identity Platform User Record\",\n  \"description\": \"Schema for a user record in Google Identity Platform, representing an authenticated user with their profile information, provider data, and authentication state.\",\n  \"type\": \"object\",\n  \"required\": [\"localId\"],\n  \"properties\": {\n    \"localId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique user ID assigned by Identity Platform\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The user's email address\"\n    },\n    \"emailVerified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user's email has been verified\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's display name\"\n    },\n\
  \    \"photoUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the user's profile photo\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The user's phone number in E.164 format\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is disabled\",\n      \"default\": false\n    },\n    \"providerUserInfo\": {\n      \"type\": \"array\",\n      \"description\": \"Linked identity provider accounts\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ProviderInfo\"\n      }\n    },\n    \"mfaInfo\": {\n      \"type\": \"array\",\n      \"description\": \"Multi-factor authentication enrollments\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MfaEnrollment\"\n      }\n    },\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"description\": \"The tenant ID if the user belongs to a specific tenant\"\n    },\n    \"createdAt\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Account creation timestamp in milliseconds since epoch\"\n    },\n    \"lastLoginAt\": {\n      \"type\": \"string\",\n      \"description\": \"Last sign-in timestamp in milliseconds since epoch\"\n    },\n    \"customAttributes\": {\n      \"type\": \"string\",\n      \"description\": \"Custom claims JSON string set via Admin SDK\"\n    }\n  },\n  \"$defs\": {\n    \"ProviderInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Information about a linked identity provider\",\n      \"properties\": {\n        \"providerId\": {\n          \"type\": \"string\",\n          \"description\": \"The provider identifier (e.g., google.com, facebook.com, password)\"\n        },\n        \"federatedId\": {\n          \"type\": \"string\",\n          \"description\": \"The user's unique ID at the provider\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        },\n        \"displayName\": {\n\
  \          \"type\": \"string\"\n        },\n        \"photoUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"MfaEnrollment\": {\n      \"type\": \"object\",\n      \"description\": \"A multi-factor authentication enrollment\",\n      \"properties\": {\n        \"mfaEnrollmentId\": {\n          \"type\": \"string\",\n          \"description\": \"The MFA enrollment ID\"\n        },\n        \"phoneInfo\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number for SMS-based MFA\"\n        },\n        \"totpInfo\": {\n          \"type\": \"object\",\n          \"description\": \"TOTP configuration for authenticator app MFA\"\n        },\n        \"enrolledAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When this factor was enrolled\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Friendly name\
  \ for this MFA enrollment\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-identity-platform/refs/heads/main/json-schema/google-identity-platform-user-schema.json
tags:
- Authentication
- Google Cloud
- Identity
- Multi-Tenancy
- OAuth
- OpenID Connect
- SAML
title: Google Identity Platform User Record
---
