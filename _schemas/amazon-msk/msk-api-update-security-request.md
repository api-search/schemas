---
description: UpdateSecurityRequest schema from Amazon MSK API
layout: schema
name: UpdateSecurityRequest
properties_list:
- description: ''
  name: ClientAuthentication
  type: object
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: EncryptionInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-security-request-schema.json
slug: msk-api-update-security-request
source_filename: msk-api-update-security-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-security-request-schema.json\",\n  \"title\": \"UpdateSecurityRequest\",\n  \"description\": \"UpdateSecurityRequest schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientAuthentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientAuthentication\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientAuthentication\"\n          },\n          \"description\": \"\\n            <p>Includes all client authentication related information.</p>\"\n        }\n      ]\n    },\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\"\
  : \"\\n            <p>The version of the MSK cluster to update. Cluster versions aren't simple numbers. You can describe an MSK cluster to find its version. When this update operation is successful, it generates a new cluster version.</p>\"\n        }\n      ]\n    },\n    \"EncryptionInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionInfo\"\n          },\n          \"description\": \"\\n            <p>Includes all encryption-related information.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrentVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-security-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateSecurityRequest
---
