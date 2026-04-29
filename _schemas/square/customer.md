---
description: Represents a Square customer profile in the Customer Directory of a Square seller. Customers can be associated with payments, orders, loyalty programs, gift cards, and bookings.
layout: schema
name: Square Customer
properties_list:
- description: A unique Square-assigned ID for the customer profile.
  name: id
  type: string
- description: The timestamp when the customer profile was created, in RFC 3339 format.
  name: created_at
  type: string
- description: The timestamp when the customer profile was last updated, in RFC 3339 format.
  name: updated_at
  type: string
- description: The given name (that is, the first name) associated with the customer profile.
  name: given_name
  type: string
- description: The family name (that is, the last name) associated with the customer profile.
  name: family_name
  type: string
- description: A nickname for the customer profile.
  name: nickname
  type: string
- description: A business name associated with the customer profile.
  name: company_name
  type: string
- description: The email address associated with the customer profile.
  name: email_address
  type: string
- description: The physical address associated with the customer profile.
  name: address
  type: object
- description: The phone number associated with the customer profile.
  name: phone_number
  type: string
- description: The birthday associated with the customer profile, in YYYY-MM-DD format. For example, 1998-09-21 represents September 21, 1998, and 0000-09-21 represents September 21 (without a birth year).
  name: birthday
  type: string
- description: An optional second ID used to associate the customer profile with an entity in another system.
  name: reference_id
  type: string
- description: A custom note associated with the customer profile.
  name: note
  type: string
- description: Represents general customer preferences.
  name: preferences
  type: object
- description: The method used to create the customer profile.
  name: creation_source
  type: string
- description: The IDs of customer groups the customer belongs to.
  name: group_ids
  type: array
- description: The IDs of customer segments the customer belongs to.
  name: segment_ids
  type: array
- description: The Square-assigned version number of the customer profile. The version number is incremented each time an update is committed to the customer profile.
  name: version
  type: integer
- description: The tax IDs associated with the customer profile. This field is available for customers of sellers in EU countries or the United Kingdom.
  name: tax_ids
  type: object
provider_name: Square
provider_slug: square
schema_file: json-schema/customer.json
slug: customer
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/square/blob/main/json-schema/customer.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Square Customer\",\n  \"description\": \"Represents a Square customer profile in the Customer Directory of a Square seller. Customers can be associated with payments, orders, loyalty programs, gift cards, and bookings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique Square-assigned ID for the customer profile.\",\n      \"readOnly\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the customer profile was created, in RFC 3339 format.\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the customer profile was last\
  \ updated, in RFC 3339 format.\",\n      \"readOnly\": true\n    },\n    \"given_name\": {\n      \"type\": \"string\",\n      \"description\": \"The given name (that is, the first name) associated with the customer profile.\"\n    },\n    \"family_name\": {\n      \"type\": \"string\",\n      \"description\": \"The family name (that is, the last name) associated with the customer profile.\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n      \"description\": \"A nickname for the customer profile.\"\n    },\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"A business name associated with the customer profile.\"\n    },\n    \"email_address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address associated with the customer profile.\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"The physical address associated with the customer profile.\",\n      \"properties\"\
  : {\n        \"address_line_1\": {\n          \"type\": \"string\",\n          \"description\": \"The first line of the address.\"\n        },\n        \"address_line_2\": {\n          \"type\": \"string\",\n          \"description\": \"The second line of the address, if any.\"\n        },\n        \"address_line_3\": {\n          \"type\": \"string\",\n          \"description\": \"The third line of the address, if any.\"\n        },\n        \"locality\": {\n          \"type\": \"string\",\n          \"description\": \"The city or town of the address.\"\n        },\n        \"sublocality\": {\n          \"type\": \"string\",\n          \"description\": \"A civil region within the address's locality, if any.\"\n        },\n        \"administrative_district_level_1\": {\n          \"type\": \"string\",\n          \"description\": \"A civil entity within the address's country. In the US, this is the state.\"\n        },\n        \"postal_code\": {\n          \"type\": \"string\",\n     \
  \     \"description\": \"The address's postal code.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The address's country, in the two-letter format of ISO 3166.\",\n          \"minLength\": 2,\n          \"maxLength\": 2\n        }\n      }\n    },\n    \"phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number associated with the customer profile.\"\n    },\n    \"birthday\": {\n      \"type\": \"string\",\n      \"description\": \"The birthday associated with the customer profile, in YYYY-MM-DD format. For example, 1998-09-21 represents September 21, 1998, and 0000-09-21 represents September 21 (without a birth year).\"\n    },\n    \"reference_id\": {\n      \"type\": \"string\",\n      \"description\": \"An optional second ID used to associate the customer profile with an entity in another system.\"\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"description\": \"A custom note associated\
  \ with the customer profile.\"\n    },\n    \"preferences\": {\n      \"type\": \"object\",\n      \"description\": \"Represents general customer preferences.\",\n      \"properties\": {\n        \"email_unsubscribed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the customer has unsubscribed from marketing campaign emails.\"\n        }\n      }\n    },\n    \"creation_source\": {\n      \"type\": \"string\",\n      \"description\": \"The method used to create the customer profile.\",\n      \"enum\": [\n        \"OTHER\",\n        \"APPOINTMENTS\",\n        \"COUPON\",\n        \"DELETION_RECOVERY\",\n        \"DIRECTORY\",\n        \"EGIFTING\",\n        \"EMAIL_COLLECTION\",\n        \"FEEDBACK\",\n        \"IMPORT\",\n        \"INVOICES\",\n        \"LOYALTY\",\n        \"MARKETING\",\n        \"MERGE\",\n        \"ONLINE_STORE\",\n        \"INSTANT_PROFILE\",\n        \"TERMINAL\",\n        \"THIRD_PARTY\",\n        \"THIRD_PARTY_IMPORT\",\n        \"\
  UNMERGE_RECOVERY\"\n      ],\n      \"readOnly\": true\n    },\n    \"group_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The IDs of customer groups the customer belongs to.\"\n    },\n    \"segment_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The IDs of customer segments the customer belongs to.\",\n      \"readOnly\": true\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The Square-assigned version number of the customer profile. The version number is incremented each time an update is committed to the customer profile.\",\n      \"readOnly\": true\n    },\n    \"tax_ids\": {\n      \"type\": \"object\",\n      \"description\": \"The tax IDs associated with the customer profile. This field is available for customers of sellers in EU countries or the United Kingdom.\"\
  ,\n      \"properties\": {\n        \"eu_vat\": {\n          \"type\": \"string\",\n          \"description\": \"The EU VAT identification number for the customer.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/square/refs/heads/main/json-schema/customer.json
tags:
- Bookings
- Catalog
- Checkout
- Customers
- Disputes
- Ecommerce
- Financial Technology
- Gift Cards
- Inventory
- Invoicing
- Labor
- Locations
- Loyalty
- Merchants
- Orders
- Payments
- Point of Sale
- Refunds
- Retail
- Subscriptions
- Team
- Terminal
- Webhooks
title: Square Customer
---
