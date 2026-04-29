---
description: Represents a complete 1Password item stored in a vault, including its fields, sections, URLs, tags, and associated metadata. Items are the primary unit of secret storage in 1Password.
layout: schema
name: 1Password Item
properties_list:
- description: The unique identifier for the item.
  name: id
  type: string
- description: The title of the item displayed in the 1Password interface.
  name: title
  type: string
- description: ''
  name: vault
  type: object
- description: The category that determines the item template and available fields.
  name: category
  type: string
- description: URLs associated with the item, such as website login pages.
  name: urls
  type: array
- description: Whether the item is marked as a favorite.
  name: favorite
  type: boolean
- description: Tags applied to the item for organization.
  name: tags
  type: array
- description: The version number of the item, incremented on each update.
  name: version
  type: integer
- description: The current state of the item.
  name: state
  type: string
- description: The fields of the item containing secrets and metadata values.
  name: fields
  type: array
- description: Sections used to organize fields into logical groups within the item.
  name: sections
  type: array
- description: The ISO 8601 date and time the item was created.
  name: createdAt
  type: string
- description: The ISO 8601 date and time the item was last updated.
  name: updatedAt
  type: string
- description: The UUID of the user who last edited the item.
  name: lastEditedBy
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-item-schema.json
slug: 1password-item
source_filename: 1password-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.1password.com/schemas/1password/item.json\",\n  \"title\": \"1Password Item\",\n  \"description\": \"Represents a complete 1Password item stored in a vault, including its fields, sections, URLs, tags, and associated metadata. Items are the primary unit of secret storage in 1Password.\",\n  \"type\": \"object\",\n  \"required\": [\"vault\", \"category\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the item.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the item displayed in the 1Password interface.\"\n    },\n    \"vault\": {\n      \"$ref\": \"#/$defs/VaultRef\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category that determines the item template and available fields.\",\n      \"\
  enum\": [\n        \"LOGIN\",\n        \"PASSWORD\",\n        \"API_CREDENTIAL\",\n        \"SERVER\",\n        \"DATABASE\",\n        \"CREDIT_CARD\",\n        \"MEMBERSHIP\",\n        \"PASSPORT\",\n        \"SOFTWARE_LICENSE\",\n        \"OUTDOOR_LICENSE\",\n        \"SECURE_NOTE\",\n        \"WIRELESS_ROUTER\",\n        \"BANK_ACCOUNT\",\n        \"DRIVER_LICENSE\",\n        \"IDENTITY\",\n        \"REWARD_PROGRAM\",\n        \"DOCUMENT\",\n        \"EMAIL_ACCOUNT\",\n        \"SOCIAL_SECURITY_NUMBER\",\n        \"MEDICAL_RECORD\",\n        \"SSH_KEY\",\n        \"CUSTOM\"\n      ]\n    },\n    \"urls\": {\n      \"type\": \"array\",\n      \"description\": \"URLs associated with the item, such as website login pages.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Url\"\n      }\n    },\n    \"favorite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the item is marked as a favorite.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Tags applied to the item for organization.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version number of the item, incremented on each update.\",\n      \"minimum\": 0\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the item.\",\n      \"enum\": [\"ARCHIVED\", \"DELETED\"]\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"The fields of the item containing secrets and metadata values.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Field\"\n      }\n    },\n    \"sections\": {\n      \"type\": \"array\",\n      \"description\": \"Sections used to organize fields into logical groups within the item.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Section\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO\
  \ 8601 date and time the item was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 date and time the item was last updated.\"\n    },\n    \"lastEditedBy\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the user who last edited the item.\"\n    }\n  },\n  \"$defs\": {\n    \"VaultRef\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a 1Password vault by its unique identifier.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the vault.\"\n        }\n      }\n    },\n    \"Url\": {\n      \"type\": \"object\",\n      \"description\": \"A URL associated with an item.\",\n      \"properties\": {\n        \"primary\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Whether this is the primary URL for the item.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL value.\"\n        }\n      }\n    },\n    \"Field\": {\n      \"type\": \"object\",\n      \"description\": \"A field within an item that stores a single value such as a username, password, or other data.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the field.\"\n        },\n        \"section\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to the section this field belongs to.\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The unique identifier of the section.\"\n            }\n          }\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the\
  \ field.\",\n          \"enum\": [\n            \"STRING\",\n            \"EMAIL\",\n            \"CONCEALED\",\n            \"URL\",\n            \"TOTP\",\n            \"DATE\",\n            \"MONTH_YEAR\",\n            \"MENU\"\n          ]\n        },\n        \"purpose\": {\n          \"type\": \"string\",\n          \"description\": \"The purpose of the field indicating its role within the item.\",\n          \"enum\": [\"USERNAME\", \"PASSWORD\", \"NOTES\"]\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable label for the field.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value stored in the field.\"\n        },\n        \"generate\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the field value should be auto-generated.\"\n        },\n        \"entropy\": {\n          \"type\": \"number\",\n          \"description\": \"The entropy\
  \ (strength) of the generated value in bits.\"\n        },\n        \"recipe\": {\n          \"$ref\": \"#/$defs/GeneratorRecipe\"\n        }\n      }\n    },\n    \"GeneratorRecipe\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for generating a random value for a field.\",\n      \"properties\": {\n        \"length\": {\n          \"type\": \"integer\",\n          \"description\": \"The length of the generated value.\",\n          \"minimum\": 1,\n          \"maximum\": 64\n        },\n        \"characterSets\": {\n          \"type\": \"array\",\n          \"description\": \"The character sets to include when generating the value.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"LETTERS\", \"DIGITS\", \"SYMBOLS\"]\n          }\n        },\n        \"excludeCharacters\": {\n          \"type\": \"string\",\n          \"description\": \"Characters to exclude from the generated value.\"\n        }\n      }\n    },\n    \"Section\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"A section within an item used to organize fields into logical groups.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the section.\"\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"The human-readable label for the section.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-item-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: 1Password Item
---
