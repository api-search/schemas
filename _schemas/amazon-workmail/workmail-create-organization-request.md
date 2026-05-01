---
description: CreateOrganizationRequest schema from Amazon WorkMail API
layout: schema
name: CreateOrganizationRequest
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: Alias
  type: object
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: Domains
  type: object
- description: ''
  name: KmsKeyArn
  type: object
- description: ''
  name: EnableInteroperability
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-create-organization-request-schema.json
slug: workmail-create-organization-request
source_filename: workmail-create-organization-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Alias\"\n  ],\n  \"title\": \"CreateOrganizationRequest\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The AWS Directory Service directory ID.\"\n        }\n      ]\n    },\n    \"Alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationName\"\n        },\n        {\n          \"description\": \"The organization alias.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyClientToken\"\n        },\n        {\n          \"description\": \"The idempotency token associated with the request.\"\n        }\n      ]\n    },\n    \"Domains\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Domains\"\n        },\n        {\n          \"\
  description\": \"The email domains to associate with the organization.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a customer managed key from AWS KMS.\"\n        }\n      ]\n    },\n    \"EnableInteroperability\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"When <code>true</code>, allows organization interoperability between WorkMail and Microsoft Exchange. If <code>true</code>, you must include a AD Connector directory ID in the request.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-organization-request-schema.json\",\n  \"description\"\
  : \"CreateOrganizationRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-organization-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: CreateOrganizationRequest
---
