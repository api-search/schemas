---
description: GetUserDetailsResponse schema from Amazon CodeCatalyst
layout: schema
name: GetUserDetailsResponse
properties_list:
- description: ''
  name: userId
  type: object
- description: ''
  name: userName
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: primaryEmail
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-get-user-details-response-schema.json
slug: amazon-codecatalyst-get-user-details-response
source_filename: amazon-codecatalyst-get-user-details-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-user-details-response-schema.json\",\n  \"title\": \"GetUserDetailsResponse\",\n  \"description\": \"GetUserDetailsResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the user.\"\n        }\n      ]\n    },\n    \"userName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the user as displayed in Amazon CodeCatalyst.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The friendly name displayed for the user in Amazon CodeCatalyst.\"\n        }\n      ]\n    },\n    \"primaryEmail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailAddress\"\n        },\n        {\n          \"description\": \"The email address provided by the user when they signed up.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-get-user-details-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: GetUserDetailsResponse
---
