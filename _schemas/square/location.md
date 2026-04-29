---
description: Represents one of a business's locations where transactions occur, inventory is managed, and team members work.
layout: schema
name: Square Location
properties_list:
- description: A short generated string of letters and numbers that uniquely identifies this location instance.
  name: id
  type: string
- description: The name of the location. This information appears in the Seller Dashboard as the nickname. A location name must be unique within a seller account.
  name: name
  type: string
- description: The physical address of the location.
  name: address
  type: object
- description: The IANA time zone identifier for the time zone of the location. For example, America/Los_Angeles.
  name: timezone
  type: string
- description: The Square features that are enabled for the location.
  name: capabilities
  type: array
- description: The status of the location.
  name: status
  type: string
- description: The time when the location was created, in RFC 3339 format.
  name: created_at
  type: string
- description: The ID of the merchant that owns the location.
  name: merchant_id
  type: string
- description: The country of the location, in the two-letter format of ISO 3166. For example, US or JP.
  name: country
  type: string
- description: The language associated with the location, in BCP 47 format.
  name: language_code
  type: string
- description: The currency used for all transactions at this location, in ISO 4217 format. For example, USD.
  name: currency
  type: string
- description: The phone number of the location. For example, +1 855-700-6000.
  name: phone_number
  type: string
- description: The name of the location's overall business. This name is present on receipts and other customer-facing branding.
  name: business_name
  type: string
- description: The type of the location.
  name: type
  type: string
- description: The website URL of the location.
  name: website_url
  type: string
- description: The hours of operation for the location.
  name: business_hours
  type: object
- description: The email address of the location.
  name: business_email
  type: string
- description: The description of the location. For example, Main Street location.
  name: description
  type: string
- description: The Twitter username of the location without the '@' symbol.
  name: twitter_username
  type: string
- description: The Instagram username of the location without the '@' symbol.
  name: instagram_username
  type: string
- description: The Facebook profile URL of the location.
  name: facebook_url
  type: string
- description: The physical coordinates (latitude and longitude) of the location.
  name: coordinates
  type: object
- description: The URL of the logo image for the location.
  name: logo_url
  type: string
- description: The URL of the Point of Sale background image for the location.
  name: pos_background_url
  type: string
- description: The merchant category code (MCC) of the location as standardized by ISO 18245.
  name: mcc
  type: string
- description: The URL of a full-format logo image for the location.
  name: full_format_logo_url
  type: string
- description: The tax IDs for this location.
  name: tax_ids
  type: object
provider_name: Square
provider_slug: square
schema_file: json-schema/location.json
slug: location
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/square/blob/main/json-schema/location.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Square Location\",\n  \"description\": \"Represents one of a business's locations where transactions occur, inventory is managed, and team members work.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A short generated string of letters and numbers that uniquely identifies this location instance.\",\n      \"maxLength\": 32,\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the location. This information appears in the Seller Dashboard as the nickname. A location name must be unique within a seller account.\",\n      \"maxLength\": 255\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"The physical address of the location.\",\n   \
  \   \"properties\": {\n        \"address_line_1\": {\n          \"type\": \"string\",\n          \"description\": \"The first line of the address.\"\n        },\n        \"address_line_2\": {\n          \"type\": \"string\",\n          \"description\": \"The second line of the address, if any.\"\n        },\n        \"address_line_3\": {\n          \"type\": \"string\",\n          \"description\": \"The third line of the address, if any.\"\n        },\n        \"locality\": {\n          \"type\": \"string\",\n          \"description\": \"The city or town of the address.\"\n        },\n        \"sublocality\": {\n          \"type\": \"string\",\n          \"description\": \"A civil region within the address's locality, if any.\"\n        },\n        \"administrative_district_level_1\": {\n          \"type\": \"string\",\n          \"description\": \"A civil entity within the address's country. In the US, this is the state.\"\n        },\n        \"postal_code\": {\n          \"type\": \"\
  string\",\n          \"description\": \"The address's postal code.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The address's country, in the two-letter format of ISO 3166.\",\n          \"minLength\": 2,\n          \"maxLength\": 2\n        }\n      }\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"The IANA time zone identifier for the time zone of the location. For example, America/Los_Angeles.\",\n      \"maxLength\": 30\n    },\n    \"capabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"CREDIT_CARD_PROCESSING\", \"AUTOMATIC_TRANSFERS\"]\n      },\n      \"description\": \"The Square features that are enabled for the location.\",\n      \"readOnly\": true\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the location.\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\"]\n    },\n    \"created_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the location was created, in RFC 3339 format.\",\n      \"readOnly\": true\n    },\n    \"merchant_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the merchant that owns the location.\",\n      \"maxLength\": 32,\n      \"readOnly\": true\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country of the location, in the two-letter format of ISO 3166. For example, US or JP.\",\n      \"minLength\": 2,\n      \"maxLength\": 2,\n      \"readOnly\": true\n    },\n    \"language_code\": {\n      \"type\": \"string\",\n      \"description\": \"The language associated with the location, in BCP 47 format.\",\n      \"minLength\": 2,\n      \"maxLength\": 5\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The currency used for all transactions at this location, in ISO 4217 format. For example, USD.\"\
  ,\n      \"minLength\": 3,\n      \"maxLength\": 3,\n      \"readOnly\": true\n    },\n    \"phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the location. For example, +1 855-700-6000.\",\n      \"maxLength\": 17\n    },\n    \"business_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the location's overall business. This name is present on receipts and other customer-facing branding.\",\n      \"maxLength\": 255\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the location.\",\n      \"enum\": [\"PHYSICAL\", \"MOBILE\"]\n    },\n    \"website_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The website URL of the location.\",\n      \"maxLength\": 255\n    },\n    \"business_hours\": {\n      \"type\": \"object\",\n      \"description\": \"The hours of operation for the location.\",\n      \"properties\": {\n        \"periods\"\
  : {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"day_of_week\": {\n                \"type\": \"string\",\n                \"description\": \"The day of the week for this time period.\",\n                \"enum\": [\"SUN\", \"MON\", \"TUE\", \"WED\", \"THU\", \"FRI\", \"SAT\"]\n              },\n              \"start_local_time\": {\n                \"type\": \"string\",\n                \"description\": \"The start time of a business hours period, specified in local time using partial-time RFC 3339 format. For example, 08:30:00.\"\n              },\n              \"end_local_time\": {\n                \"type\": \"string\",\n                \"description\": \"The end time of a business hours period, specified in local time using partial-time RFC 3339 format. For example, 21:00:00.\"\n              }\n            }\n          },\n          \"description\": \"The list of time periods during which\
  \ the location is open.\"\n        }\n      }\n    },\n    \"business_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the location.\",\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the location. For example, Main Street location.\",\n      \"maxLength\": 1024\n    },\n    \"twitter_username\": {\n      \"type\": \"string\",\n      \"description\": \"The Twitter username of the location without the '@' symbol.\",\n      \"maxLength\": 15\n    },\n    \"instagram_username\": {\n      \"type\": \"string\",\n      \"description\": \"The Instagram username of the location without the '@' symbol.\",\n      \"maxLength\": 30\n    },\n    \"facebook_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The Facebook profile URL of the location.\",\n      \"maxLength\": 255\n    },\n    \"coordinates\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"The physical coordinates (latitude and longitude) of the location.\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"The latitude coordinate of the location.\"\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"The longitude coordinate of the location.\"\n        }\n      }\n    },\n    \"logo_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the logo image for the location.\",\n      \"readOnly\": true\n    },\n    \"pos_background_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the Point of Sale background image for the location.\",\n      \"readOnly\": true\n    },\n    \"mcc\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant category code (MCC) of the location as standardized by ISO 18245.\"\
  ,\n      \"minLength\": 4,\n      \"maxLength\": 4\n    },\n    \"full_format_logo_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of a full-format logo image for the location.\",\n      \"readOnly\": true\n    },\n    \"tax_ids\": {\n      \"type\": \"object\",\n      \"description\": \"The tax IDs for this location.\",\n      \"properties\": {\n        \"eu_vat\": {\n          \"type\": \"string\",\n          \"description\": \"The EU VAT number for this location.\"\n        },\n        \"fr_siret\": {\n          \"type\": \"string\",\n          \"description\": \"The SIRET number for this location (France).\"\n        },\n        \"fr_naf\": {\n          \"type\": \"string\",\n          \"description\": \"The NAF code for this location (France).\"\n        },\n        \"es_nif\": {\n          \"type\": \"string\",\n          \"description\": \"The NIF number for this location (Spain).\"\n        }\n      },\n      \"readOnly\": true\n\
  \    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/square/refs/heads/main/json-schema/location.json
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
title: Square Location
---
