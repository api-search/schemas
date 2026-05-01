---
description: 'Specifies the advanced security configuration: whether advanced security is enabled, whether the internal database option is enabled.'
layout: schema
name: AdvancedSecurityOptions
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: InternalUserDatabaseEnabled
  type: object
- description: ''
  name: SAMLOptions
  type: object
- description: ''
  name: AnonymousAuthDisableDate
  type: object
- description: ''
  name: AnonymousAuthEnabled
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-advanced-security-options-schema.json
slug: openapi-advanced-security-options
source_filename: openapi-advanced-security-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-advanced-security-options-schema.json\",\n  \"title\": \"AdvancedSecurityOptions\",\n  \"description\": \"Specifies the advanced security configuration: whether advanced security is enabled, whether the internal database option is enabled.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"True if advanced security is enabled.\"\n        }\n      ]\n    },\n    \"InternalUserDatabaseEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"True if the internal user database is enabled.\"\n        }\n      ]\n    },\n    \"SAMLOptions\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SAMLOptionsOutput\"\n        },\n        {\n          \"description\": \"Describes the SAML application configured for a domain.\"\n        }\n      ]\n    },\n    \"AnonymousAuthDisableDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisableTimestamp\"\n        },\n        {\n          \"description\": \"Specifies the Anonymous Auth Disable Date when Anonymous Auth is enabled.\"\n        }\n      ]\n    },\n    \"AnonymousAuthEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"True if Anonymous auth is enabled. Anonymous auth can be enabled only when AdvancedSecurity is enabled on existing domains.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-advanced-security-options-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: AdvancedSecurityOptions
---
