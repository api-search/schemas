---
description: DescribeUserResponse schema from AWS IAM Identity Center
layout: schema
name: DescribeUserResponse
properties_list:
- description: ''
  name: UserName
  type: object
- description: ''
  name: UserId
  type: object
- description: ''
  name: ExternalIds
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: DisplayName
  type: object
- description: ''
  name: NickName
  type: object
- description: ''
  name: ProfileUrl
  type: object
- description: ''
  name: Emails
  type: object
- description: ''
  name: Addresses
  type: object
- description: ''
  name: PhoneNumbers
  type: object
- description: ''
  name: UserType
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: PreferredLanguage
  type: object
- description: ''
  name: Locale
  type: object
- description: ''
  name: Timezone
  type: object
- description: ''
  name: IdentityStoreId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-describe-user-response-schema.json
slug: identitystore-describe-user-response
source_filename: identitystore-describe-user-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-describe-user-response-schema.json\",\n  \"title\": \"DescribeUserResponse\",\n  \"description\": \"DescribeUserResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"A unique string used to identify the user. The length limit is 128 characters. This value can consist of letters, accented characters, symbols, numbers, and punctuation. This value is specified at the time the user is created and stored as an attribute of the user object in the identity store.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\
  \n        },\n        {\n          \"description\": \"The identifier for a user in the identity store.\"\n        }\n      ]\n    },\n    \"ExternalIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalIds\"\n        },\n        {\n          \"description\": \"A list of <code>ExternalId</code> objects that contains the identifiers issued to this resource by an external identity provider.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the user.\"\n        }\n      ]\n    },\n    \"DisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"The display name of the user.\"\n        }\n      ]\n    },\n    \"NickName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\
  \n        },\n        {\n          \"description\": \"An alternative descriptive name for the user.\"\n        }\n      ]\n    },\n    \"ProfileUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A URL link for the user's profile.\"\n        }\n      ]\n    },\n    \"Emails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Emails\"\n        },\n        {\n          \"description\": \"The email address of the user.\"\n        }\n      ]\n    },\n    \"Addresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Addresses\"\n        },\n        {\n          \"description\": \"The physical address of the user.\"\n        }\n      ]\n    },\n    \"PhoneNumbers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PhoneNumbers\"\n        },\n        {\n          \"description\": \"A list of <code>PhoneNumber</code>\
  \ objects associated with a user.\"\n        }\n      ]\n    },\n    \"UserType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string indicating the type of user.\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing the title of the user.\"\n        }\n      ]\n    },\n    \"PreferredLanguage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"The preferred language of the user.\"\n        }\n      ]\n    },\n    \"Locale\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing the geographical region\
  \ or location of the user.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"The time zone for a user.\"\n        }\n      ]\n    },\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserId\",\n    \"IdentityStoreId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-describe-user-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: DescribeUserResponse
---
