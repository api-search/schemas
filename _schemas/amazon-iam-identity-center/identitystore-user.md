---
description: A user object that contains the metadata and attributes for a specified user.
layout: schema
name: User
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
schema_file: json-schema/identitystore-user-schema.json
slug: identitystore-user
source_filename: identitystore-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A user object that contains the metadata and attributes for a specified user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"A unique string used to identify the user. The length limit is 128 characters. This value can consist of letters, accented characters, symbols, numbers, and punctuation. This value is specified at the time the user is created and stored as an attribute of the user object in the identity store.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n \
  \       },\n        {\n          \"description\": \"The identifier for a user in the identity store.\"\n        }\n      ]\n    },\n    \"ExternalIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalIds\"\n        },\n        {\n          \"description\": \"A list of <code>ExternalId</code> objects that contains the identifiers issued to this resource by an external identity provider.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"An object containing the name of the user.\"\n        }\n      ]\n    },\n    \"DisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing the name of the user that is formatted for display when the user is referenced. For example, \\\"John Doe.\\\"\"\n        }\n\
  \      ]\n    },\n    \"NickName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing an alternate name for the user.\"\n        }\n      ]\n    },\n    \"ProfileUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing a URL that might be associated with the user.\"\n        }\n      ]\n    },\n    \"Emails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Emails\"\n        },\n        {\n          \"description\": \"A list of <code>Email</code> objects containing email addresses associated with the user.\"\n        }\n      ]\n    },\n    \"Addresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Addresses\"\n        },\n        {\n          \"description\": \"A list of <code>Address</code>\
  \ objects containing addresses associated with the user.\"\n        }\n      ]\n    },\n    \"PhoneNumbers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PhoneNumbers\"\n        },\n        {\n          \"description\": \"A list of <code>PhoneNumber</code> objects containing phone numbers associated with the user.\"\n        }\n      ]\n    },\n    \"UserType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string indicating the type of user. Possible values are left unspecified. The value can vary based on your specific use case.\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing the title of the user. Possible values are left unspecified. The value can vary based on your specific use\
  \ case.\"\n        }\n      ]\n    },\n    \"PreferredLanguage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing the preferred language of the user. For example, \\\"American English\\\" or \\\"en-us.\\\"\"\n        }\n      ]\n    },\n    \"Locale\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing the geographical region or location of the user.\"\n        }\n      ]\n    },\n    \"Timezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing the time zone of the user.\"\n        }\n      ]\n    },\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n \
  \       },\n        {\n          \"description\": \"The globally unique identifier for the identity store.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserId\",\n    \"IdentityStoreId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-user-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: User
---
