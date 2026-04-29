---
description: ListPermissionsResponse schema from Amazon Private CA API
layout: schema
name: ListPermissionsResponse
properties_list:
- description: ''
  name: Permissions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-list-permissions-response-schema.json
slug: amazon-private-ca-list-permissions-response
source_filename: amazon-private-ca-list-permissions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-list-permissions-response-schema.json\",\n  \"title\": \"ListPermissionsResponse\",\n  \"description\": \"ListPermissionsResponse schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Permissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionList\"\n        },\n        {\n          \"description\": \"Summary information about each permission assigned by the specified private CA, including the action enabled, the policy provided, and the time of creation.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"When the list is truncated, this value is present and should be\
  \ used for the <b>NextToken</b> parameter in a subsequent pagination request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-list-permissions-response-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: ListPermissionsResponse
---
