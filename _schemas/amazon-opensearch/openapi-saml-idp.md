---
description: Specifies the SAML Identity Provider's information.
layout: schema
name: SAMLIdp
properties_list:
- description: ''
  name: MetadataContent
  type: object
- description: ''
  name: EntityId
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-saml-idp-schema.json
slug: openapi-saml-idp
source_filename: openapi-saml-idp-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-saml-idp-schema.json\",\n  \"title\": \"SAMLIdp\",\n  \"description\": \"Specifies the SAML Identity Provider's information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetadataContent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SAMLMetadata\"\n        },\n        {\n          \"description\": \"The Metadata of the SAML application in xml format.\"\n        }\n      ]\n    },\n    \"EntityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SAMLEntityId\"\n        },\n        {\n          \"description\": \"The unique Entity ID of the application in SAML Identity Provider.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MetadataContent\",\n    \"EntityId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-saml-idp-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: SAMLIdp
---
