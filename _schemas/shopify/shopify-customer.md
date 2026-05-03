---
description: A customer of a Shopify store. Customers represent people who have purchased from the store or who have created an account.
layout: schema
name: Shopify Customer
properties_list:
- description: Unique numeric identifier for the customer
  name: id
  type: integer
- description: The customer email address
  name: email
  type:
  - string
  - 'null'
- description: The customer first name
  name: first_name
  type:
  - string
  - 'null'
- description: The customer last name
  name: last_name
  type:
  - string
  - 'null'
- description: The customer phone number in E.164 format
  name: phone
  type:
  - string
  - 'null'
- description: The number of orders placed by the customer
  name: orders_count
  type: integer
- description: The total amount spent by the customer as a decimal string
  name: total_spent
  type: string
- description: The state of the customer account
  name: state
  type: string
- description: A note about the customer visible to store staff
  name: note
  type:
  - string
  - 'null'
- description: Whether the customer has verified their email address
  name: verified_email
  type: boolean
- description: Whether the customer is exempt from paying taxes
  name: tax_exempt
  type: boolean
- description: Comma-separated list of tags associated with the customer
  name: tags
  type: string
- description: The three-letter ISO 4217 currency code for the customer
  name: currency
  type: string
- description: Whether the customer has consented to receive marketing emails
  name: accepts_marketing
  type: boolean
- description: When the marketing consent was last updated
  name: accepts_marketing_updated_at
  type:
  - string
  - 'null'
- description: The marketing subscription opt-in level
  name: marketing_opt_in_level
  type:
  - string
  - 'null'
- description: Tax exemptions that apply to the customer
  name: tax_exemptions
  type: array
- description: When the customer record was created
  name: created_at
  type: string
- description: When the customer record was last updated
  name: updated_at
  type: string
- description: The customer default mailing address
  name: default_address
  type: object
- description: All addresses associated with the customer
  name: addresses
  type: array
- description: The GraphQL Admin API identifier
  name: admin_graphql_api_id
  type: string
provider_name: Shopify
provider_slug: shopify
schema_file: json-schema/shopify-customer-schema.json
slug: shopify-customer
source_filename: shopify-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://shopify.dev/schemas/customer.json\",\n  \"title\": \"Shopify Customer\",\n  \"description\": \"A customer of a Shopify store. Customers represent people who have purchased from the store or who have created an account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the customer\"\n    },\n    \"email\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The customer email address\"\n    },\n    \"first_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The customer first name\"\n    },\n    \"last_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The customer last name\"\n    },\n    \"phone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The customer phone number\
  \ in E.164 format\"\n    },\n    \"orders_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of orders placed by the customer\"\n    },\n    \"total_spent\": {\n      \"type\": \"string\",\n      \"description\": \"The total amount spent by the customer as a decimal string\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the customer account\",\n      \"enum\": [\"disabled\", \"invited\", \"enabled\", \"declined\"]\n    },\n    \"note\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A note about the customer visible to store staff\"\n    },\n    \"verified_email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer has verified their email address\"\n    },\n    \"tax_exempt\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer is exempt from paying taxes\"\n    },\n    \"tags\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Comma-separated list of tags associated with the customer\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The three-letter ISO 4217 currency code for the customer\"\n    },\n    \"accepts_marketing\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the customer has consented to receive marketing emails\"\n    },\n    \"accepts_marketing_updated_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the marketing consent was last updated\"\n    },\n    \"marketing_opt_in_level\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The marketing subscription opt-in level\",\n      \"enum\": [\"single_opt_in\", \"confirmed_opt_in\", \"unknown\", null]\n    },\n    \"tax_exemptions\": {\n      \"type\": \"array\",\n      \"description\": \"Tax exemptions that apply to the customer\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"created_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the customer record was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the customer record was last updated\"\n    },\n    \"default_address\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"The customer default mailing address\"\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"description\": \"All addresses associated with the customer\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Address\"\n      }\n    },\n    \"admin_graphql_api_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL Admin API identifier\"\n    }\n  },\n  \"required\": [\"id\"],\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A customer mailing address\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"Unique numeric identifier for the address\"\n        },\n        \"customer_id\": {\n          \"type\": \"integer\"\n        },\n        \"first_name\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"last_name\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"company\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"address1\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Street address line 1\"\n        },\n        \"address2\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Street address line 2\"\n        },\n        \"city\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"province\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Province, state, or region\"\n        },\n        \"country\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"zip\": {\n  \
  \        \"type\": [\"string\", \"null\"],\n          \"description\": \"Postal or zip code\"\n        },\n        \"phone\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"province_code\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The two-letter province or state code\"\n        },\n        \"country_code\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The two-letter ISO 3166-1 country code\"\n        },\n        \"country_name\": {\n          \"type\": [\"string\", \"null\"]\n        },\n        \"default\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the customer default address\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/json-schema/shopify-customer-schema.json
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
title: Shopify Customer
---
