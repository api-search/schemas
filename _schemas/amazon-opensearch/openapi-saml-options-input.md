---
description: Specifies the SAML application configuration for the domain.
layout: schema
name: SAMLOptionsInput
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: Idp
  type: object
- description: ''
  name: MasterUserName
  type: object
- description: ''
  name: MasterBackendRole
  type: object
- description: ''
  name: SubjectKey
  type: object
- description: ''
  name: RolesKey
  type: object
- description: ''
  name: SessionTimeoutMinutes
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-saml-options-input-schema.json
slug: openapi-saml-options-input
source_filename: openapi-saml-options-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-saml-options-input-schema.json\",\n  \"title\": \"SAMLOptionsInput\",\n  \"description\": \"Specifies the SAML application configuration for the domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"True if SAML is enabled.\"\n        }\n      ]\n    },\n    \"Idp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SAMLIdp\"\n        },\n        {\n          \"description\": \"Specifies the SAML Identity Provider's information.\"\n        }\n      ]\n    },\n    \"MasterUserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Username\"\n        },\n        {\n          \"description\"\
  : \"The SAML master username, which is stored in the Amazon Elasticsearch Service domain's internal database.\"\n        }\n      ]\n    },\n    \"MasterBackendRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BackendRole\"\n        },\n        {\n          \"description\": \"The backend role to which the SAML master user is mapped to.\"\n        }\n      ]\n    },\n    \"SubjectKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The key to use for matching the SAML Subject attribute.\"\n        }\n      ]\n    },\n    \"RolesKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The key to use for matching the SAML Roles attribute.\"\n        }\n      ]\n    },\n    \"SessionTimeoutMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\
  \n        },\n        {\n          \"description\": \"The duration, in minutes, after which a user session becomes inactive. Acceptable values are between 1 and 1440, and the default value is 60.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-saml-options-input-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: SAMLOptionsInput
---
