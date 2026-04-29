---
description: A container for the UI customization information for a user pool's built-in app UI.
layout: schema
name: UICustomizationType
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ClientId
  type: object
- description: ''
  name: ImageUrl
  type: object
- description: ''
  name: CSS
  type: object
- description: ''
  name: CSSVersion
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: CreationDate
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-ui-customization-type-schema.json
slug: user-pools-ui-customization-type
source_filename: user-pools-ui-customization-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-ui-customization-type-schema.json\",\n  \"title\": \"UICustomizationType\",\n  \"description\": \"A container for the UI customization information for a user pool's built-in app UI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"ClientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientIdType\"\n        },\n        {\n          \"description\": \"The client ID for the client app.\"\n        }\n      ]\n    },\n    \"ImageUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageUrlType\"\
  \n        },\n        {\n          \"description\": \"The logo image for the UI customization.\"\n        }\n      ]\n    },\n    \"CSS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CSSType\"\n        },\n        {\n          \"description\": \"The CSS values in the UI customization.\"\n        }\n      ]\n    },\n    \"CSSVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CSSVersionType\"\n        },\n        {\n          \"description\": \"The CSS version number.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was modified.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\
  \n        },\n        {\n          \"description\": \"The date and time, in <a href=\\\"https://www.iso.org/iso-8601-date-and-time-format.html\\\">ISO 8601</a> format, when the item was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-ui-customization-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UICustomizationType
---
