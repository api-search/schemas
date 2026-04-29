---
description: A merchant or card acceptor registered in the Mastercard network. Represents businesses that accept Mastercard payments, with location, categorization, and terminal capability data. Used across Merchant Locations, Checkout Solutions, fraud reporting, and analytics APIs.
layout: schema
name: Mastercard Merchant
properties_list:
- description: Card acceptor or merchant unique identification number assigned by the acquirer.
  name: merchantId
  type: string
- description: Numerical merchant identifier within the Mastercard Merchant Locations system.
  name: id
  type: integer
- description: Legal or trade name of the merchant.
  name: merchantName
  type: string
- description: Doing Business As (DBA) name, the merchant name visible to cardholders.
  name: dbaName
  type: string
- description: Four-digit ISO 18245 Merchant Category Code (MCC) classifying the business type.
  name: merchantCategoryCode
  type: string
- description: Human-readable merchant category description from the Mastercard category taxonomy.
  name: category
  type: string
- description: Mastercard internal category identifier for the merchant.
  name: categoryId
  type: string
- description: Classification of the merchant by acceptance capability.
  name: merchantType
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: location
  type: object
- description: Distance from a search reference point to this merchant location.
  name: distance
  type: number
- description: Unit of measure for the distance value.
  name: distanceUnit
  type: string
- description: Geocoding result quality indicator for the merchant address.
  name: geocodingResult
  type: string
- description: ''
  name: terminalCapabilities
  type: object
- description: Maximum cashback amount permitted at this merchant location.
  name: cashbackMaximumAmount
  type: string
- description: ''
  name: dpa
  type: object
- description: ICA number of the acquiring institution for this merchant.
  name: acquirerId
  type: string
- description: Merchant identifier assigned by the acquirer.
  name: acquirerMerchantId
  type: string
- description: URL of the merchant website.
  name: websiteUrl
  type: string
- description: URL of the merchant logo image.
  name: logoUrl
  type: string
- description: Unique identifier representing the merchant as a sponsor of offers.
  name: offerMerchantId
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/merchant.json
slug: merchant
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/mastercard/blob/main/json-schema/merchant.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Mastercard Merchant\",\n  \"description\": \"A merchant or card acceptor registered in the Mastercard network. Represents businesses that accept Mastercard payments, with location, categorization, and terminal capability data. Used across Merchant Locations, Checkout Solutions, fraud reporting, and analytics APIs.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"merchantId\",\n    \"merchantName\"\n  ],\n  \"properties\": {\n    \"merchantId\": {\n      \"type\": \"string\",\n      \"description\": \"Card acceptor or merchant unique identification number assigned by the acquirer.\",\n      \"minLength\": 1,\n      \"maxLength\": 15,\n      \"examples\": [\"A42E51982100100\"]\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numerical merchant identifier within the\
  \ Mastercard Merchant Locations system.\",\n      \"format\": \"int32\",\n      \"examples\": [1505451132]\n    },\n    \"merchantName\": {\n      \"type\": \"string\",\n      \"description\": \"Legal or trade name of the merchant.\",\n      \"minLength\": 1,\n      \"maxLength\": 100,\n      \"examples\": [\"Ecom Holdings Online Inc\"]\n    },\n    \"dbaName\": {\n      \"type\": \"string\",\n      \"description\": \"Doing Business As (DBA) name, the merchant name visible to cardholders.\",\n      \"maxLength\": 100\n    },\n    \"merchantCategoryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Four-digit ISO 18245 Merchant Category Code (MCC) classifying the business type.\",\n      \"pattern\": \"^[0-9]{4}$\",\n      \"minLength\": 4,\n      \"maxLength\": 4,\n      \"examples\": [\"5411\"]\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable merchant category description from the Mastercard category taxonomy.\",\n      \"\
  examples\": [\"10 - Grocery Stores & Supermarkets\"]\n    },\n    \"categoryId\": {\n      \"type\": \"string\",\n      \"description\": \"Mastercard internal category identifier for the merchant.\",\n      \"minLength\": 1,\n      \"maxLength\": 2,\n      \"examples\": [\"10\"]\n    },\n    \"merchantType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the merchant by acceptance capability.\",\n      \"enum\": [\n        \"paypass\",\n        \"repower\",\n        \"easysavings\",\n        \"cashback\"\n      ]\n    },\n    \"address\": {\n      \"$ref\": \"#/$defs/MerchantAddress\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/GeoLocation\"\n    },\n    \"distance\": {\n      \"type\": \"number\",\n      \"description\": \"Distance from a search reference point to this merchant location.\",\n      \"format\": \"double\",\n      \"examples\": [1.75723]\n    },\n    \"distanceUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of\
  \ measure for the distance value.\",\n      \"enum\": [\"MILE\", \"KM\"],\n      \"examples\": [\"MILE\"]\n    },\n    \"geocodingResult\": {\n      \"type\": \"string\",\n      \"description\": \"Geocoding result quality indicator for the merchant address.\",\n      \"examples\": [\"S8HPNTSCZA\"]\n    },\n    \"terminalCapabilities\": {\n      \"$ref\": \"#/$defs/TerminalCapabilities\"\n    },\n    \"cashbackMaximumAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum cashback amount permitted at this merchant location.\",\n      \"examples\": [\"40\"]\n    },\n    \"dpa\": {\n      \"$ref\": \"#/$defs/DigitalPaymentApplication\"\n    },\n    \"acquirerId\": {\n      \"type\": \"string\",\n      \"description\": \"ICA number of the acquiring institution for this merchant.\",\n      \"minLength\": 3,\n      \"maxLength\": 7\n    },\n    \"acquirerMerchantId\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant identifier assigned by the acquirer.\",\n\
  \      \"maxLength\": 15,\n      \"examples\": [\"M123456\"]\n    },\n    \"websiteUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the merchant website.\",\n      \"format\": \"uri\",\n      \"examples\": [\"https://example.com/ecom-online-ltd/basket.html\"]\n    },\n    \"logoUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the merchant logo image.\",\n      \"format\": \"uri\",\n      \"examples\": [\"https://example.com/ecom-online-ltd/images/ecom-logo.png\"]\n    },\n    \"offerMerchantId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier representing the merchant as a sponsor of offers.\",\n      \"examples\": [\"1143109\"]\n    }\n  },\n  \"$defs\": {\n    \"MerchantAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Physical or mailing address of a merchant location.\",\n      \"properties\": {\n        \"addressLine1\": {\n          \"type\": \"string\",\n          \"description\": \"First line\
  \ of the street address, usually including street number and name.\",\n          \"examples\": [\"4033 Veterans Memorial Pkwy\"]\n        },\n        \"addressLine2\": {\n          \"type\": \"string\",\n          \"description\": \"Second line of the street address, such as suite or apartment number.\",\n          \"examples\": [\"Apt 1\"]\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name of the merchant location.\",\n          \"examples\": [\"SAINT PETERS\"]\n        },\n        \"stateProvinceCode\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter state or province code (US and Canada).\",\n          \"minLength\": 2,\n          \"maxLength\": 3,\n          \"examples\": [\"MO\"]\n        },\n        \"stateProvinceName\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the state or province.\",\n          \"examples\": [\"Missouri\"]\n        },\n        \"postalCode\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code for the merchant location.\",\n          \"maxLength\": 10,\n          \"examples\": [\"63376\"]\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-3 or alpha-2 country code for the merchant location.\",\n          \"minLength\": 2,\n          \"maxLength\": 3,\n          \"examples\": [\"USA\"]\n        },\n        \"countryName\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the country.\",\n          \"examples\": [\"United States\"]\n        }\n      }\n    },\n    \"GeoLocation\": {\n      \"type\": \"object\",\n      \"description\": \"Geographic coordinates for a merchant location.\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"string\",\n          \"description\": \"Latitude coordinate of the merchant location.\",\n          \"examples\": [\"38.795089\"]\n        },\n\
  \        \"longitude\": {\n          \"type\": \"string\",\n          \"description\": \"Longitude coordinate of the merchant location.\",\n          \"examples\": [\"-90.572346\"]\n        }\n      }\n    },\n    \"TerminalCapabilities\": {\n      \"type\": \"object\",\n      \"description\": \"Capabilities of terminals at the merchant location.\",\n      \"properties\": {\n        \"isPayPassConcession\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the concession area is equipped with a PayPass contactless reader.\"\n        },\n        \"isPayPassPharmacy\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the pharmacy is equipped with a PayPass contactless reader.\"\n        },\n        \"isPayPassFuelPump\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the fuel pump is equipped with a PayPass contactless reader.\"\n        },\n        \"isPayPassTollBooth\": {\n          \"type\": \"boolean\",\n  \
  \        \"description\": \"Whether the toll booth is equipped with a PayPass contactless reader.\"\n        },\n        \"isPayPassDriveThrough\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the drive-through is equipped with a PayPass contactless reader.\"\n        },\n        \"terminalId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique code identifying the terminal at the merchant location.\",\n          \"maxLength\": 8\n        },\n        \"terminalAttendanceIndicator\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates if the card acceptor was attending the terminal.\",\n          \"maxLength\": 1\n        },\n        \"terminalOperatingEnvironment\": {\n          \"type\": \"string\",\n          \"description\": \"Operating environment of the terminal (attended, unattended, etc.).\",\n          \"maxLength\": 1\n        },\n        \"terminalCapabilityIndicator\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Capability of the terminal to read card data.\",\n          \"maxLength\": 1\n        }\n      }\n    },\n    \"DigitalPaymentApplication\": {\n      \"type\": \"object\",\n      \"description\": \"A Digital Payment Application (DPA) representing a website or mobile app where consumers can purchase goods using Mastercard SRC (Secure Remote Commerce).\",\n      \"properties\": {\n        \"srcDpaId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the DPA within the SRC system.\",\n          \"examples\": [\"src_dpa_56068\"]\n        },\n        \"dpaName\": {\n          \"type\": \"string\",\n          \"description\": \"Legal name of the DPA operator.\",\n          \"examples\": [\"Ecom Holdings Online Inc\"]\n        },\n        \"dpaPresentationName\": {\n          \"type\": \"string\",\n          \"description\": \"Consumer-facing display name of the DPA.\"\n        },\n        \"programType\": {\n          \"\
  type\": \"string\",\n          \"description\": \"The program type for the DPA registration.\",\n          \"enum\": [\"SRC\", \"TOKEN\"]\n        },\n        \"serviceId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier assigned by Mastercard for which tokens are created.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/merchant.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Mastercard Merchant
---
