---
description: AcceptInvitationRequest schema from Amazon Macie API
layout: schema
name: AcceptInvitationRequest
properties_list:
- description: ''
  name: administratorAccountId
  type: object
- description: ''
  name: invitationId
  type: object
- description: ''
  name: masterAccount
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-accept-invitation-request-schema.json
slug: amazon-macie-accept-invitation-request
source_filename: amazon-macie-accept-invitation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-accept-invitation-request-schema.json\",\n  \"title\": \"AcceptInvitationRequest\",\n  \"description\": \"AcceptInvitationRequest schema from Amazon Macie API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"administratorAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the account that sent the invitation.\"\n        }\n      ]\n    },\n    \"invitationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the invitation to accept.\"\n        }\n      ]\n    },\n    \"masterAccount\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"(Deprecated) The Amazon Web Services account ID for the account that sent the invitation. This property has been replaced by the administratorAccountId property and is retained only for backward compatibility.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"invitationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-accept-invitation-request-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AcceptInvitationRequest
---
