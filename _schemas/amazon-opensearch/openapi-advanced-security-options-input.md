---
description: 'Specifies the advanced security configuration: whether advanced security is enabled, whether the internal database option is enabled, master username and password (if internal database is enabled), and master user ARN (if IAM is enabled).'
layout: schema
name: AdvancedSecurityOptionsInput
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: InternalUserDatabaseEnabled
  type: object
- description: ''
  name: MasterUserOptions
  type: object
- description: ''
  name: SAMLOptions
  type: object
- description: ''
  name: AnonymousAuthEnabled
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-advanced-security-options-input-schema.json
slug: openapi-advanced-security-options-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-advanced-security-options-input-schema.json\",\n  \"title\": \"AdvancedSecurityOptionsInput\",\n  \"description\": \"Specifies the advanced security configuration: whether advanced security is enabled, whether the internal database option is enabled, master username and password (if internal database is enabled), and master user ARN (if IAM is enabled).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"True if advanced security is enabled.\"\n        }\n      ]\n    },\n    \"InternalUserDatabaseEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\"\
  : \"True if the internal user database is enabled.\"\n        }\n      ]\n    },\n    \"MasterUserOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MasterUserOptions\"\n        },\n        {\n          \"description\": \"Credentials for the master user: username and password, ARN, or both.\"\n        }\n      ]\n    },\n    \"SAMLOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SAMLOptionsInput\"\n        },\n        {\n          \"description\": \"Specifies the SAML application configuration for the domain.\"\n        }\n      ]\n    },\n    \"AnonymousAuthEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"True if Anonymous auth is enabled. Anonymous auth can be enabled only when AdvancedSecurity is enabled on existing domains.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-advanced-security-options-input-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AdvancedSecurityOptionsInput
---
