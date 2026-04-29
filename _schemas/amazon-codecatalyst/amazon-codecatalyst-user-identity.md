---
description: Information about a user whose activity is recorded in an event for a space.
layout: schema
name: UserIdentity
properties_list:
- description: ''
  name: userType
  type: object
- description: ''
  name: principalId
  type: object
- description: ''
  name: userName
  type: object
- description: ''
  name: awsAccountId
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-user-identity-schema.json
slug: amazon-codecatalyst-user-identity
source_filename: amazon-codecatalyst-user-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-user-identity-schema.json\",\n  \"title\": \"UserIdentity\",\n  \"description\": \"Information about a user whose activity is recorded in an event for a space.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserType\"\n        },\n        {\n          \"description\": \"The role assigned to the user in a Amazon CodeCatalyst space or project when the event occurred.\"\n        }\n      ]\n    },\n    \"principalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of the Amazon CodeCatalyst service principal.\"\n        }\n      ]\n    },\n    \"userName\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The display name of the user in Amazon CodeCatalyst.\"\n        }\n      ]\n    },\n    \"awsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account number of the user in Amazon Web Services, if any.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"userType\",\n    \"principalId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-user-identity-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: UserIdentity
---
