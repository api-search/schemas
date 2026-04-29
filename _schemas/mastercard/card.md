---
description: A Mastercard payment card representing a physical or virtual card instrument issued to a cardholder. Covers prepaid, debit, credit, and commercial card products across Card Issuance, BIN Lookup, Benefit Eligibility, and tokenization services.
layout: schema
name: Mastercard Card
properties_list:
- description: Primary Account Number (PAN) for the card. Must pass Luhn algorithm validation.
  name: cardNumber
  type: string
- description: Unique system-generated identifier for the card within the Mastercard issuing platform.
  name: cardId
  type: string
- description: Identifier for the card pack, used in card issuance and fulfillment.
  name: cardPackId
  type: string
- description: Classification of the card product.
  name: cardType
  type: string
- description: Three-character code identifying the specific card product (e.g., MSI for Mastercard Standard, MWE for World Elite, MWO for World).
  name: cardProductCode
  type: string
- description: Card plan code defining the card product configuration and features.
  name: planCode
  type: string
- description: Program code for the card product within the issuing institution.
  name: programCode
  type: string
- description: Card brand within the Mastercard network.
  name: brand
  type: string
- description: Card tier or level indicating the product benefits tier.
  name: tier
  type: string
- description: Current lifecycle status of the card.
  name: status
  type: string
- description: Date the card was issued, in ISO 8601 date format.
  name: issuedDate
  type: string
- description: Card expiration date in MMYY format.
  name: expirationDate
  type: string
- description: Name embossed or printed on the physical card.
  name: embossedName
  type: string
- description: Indicates whether the card number is printed on the physical card. True means the number is not printed.
  name: numberless
  type: boolean
- description: Indicates whether the card was issued as an instant card (immediately generated).
  name: instant
  type: boolean
- description: Indicates whether this is a virtual card with no physical plastic.
  name: virtual
  type: boolean
- description: Indicates whether the card supports contactless (NFC/PayPass) transactions.
  name: contactless
  type: boolean
- description: Indicates whether a photo is required on the card.
  name: photoIndicator
  type: string
- description: Mode of card delivery to the cardholder.
  name: deliveryMode
  type: string
- description: Date the card was delivered or handed over to the client, in ISO 8601 format.
  name: deliveryDate
  type: string
- description: MDES (Mastercard Digital Enablement Service) token representing this card for digital transactions.
  name: tokenNumber
  type: string
- description: Bank Identification Number (BIN), the first 6-8 digits of the card number identifying the issuing institution.
  name: binNumber
  type: string
- description: ICA (Interbank Card Association) number of the issuing institution.
  name: issuerId
  type: string
- description: Name of the financial institution that issued the card.
  name: issuerName
  type: string
- description: ISO 3166-1 alpha-3 country code of the issuing institution.
  name: issuerCountryCode
  type: string
- description: ''
  name: cardholder
  type: object
- description: ''
  name: limits
  type: object
- description: Type of card issuance application.
  name: applicationType
  type: string
- description: Unique code of the corporate entity for commercial/corporate cards.
  name: corporateCode
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/card.json
slug: card
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/mastercard/blob/main/json-schema/card.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Mastercard Card\",\n  \"description\": \"A Mastercard payment card representing a physical or virtual card instrument issued to a cardholder. Covers prepaid, debit, credit, and commercial card products across Card Issuance, BIN Lookup, Benefit Eligibility, and tokenization services.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"cardNumber\",\n    \"cardType\"\n  ],\n  \"properties\": {\n    \"cardNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Primary Account Number (PAN) for the card. Must pass Luhn algorithm validation.\",\n      \"pattern\": \"^[0-9]{12,19}$\",\n      \"minLength\": 12,\n      \"maxLength\": 19,\n      \"examples\": [\"5505135664572870000\"]\n    },\n    \"cardId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique system-generated identifier\
  \ for the card within the Mastercard issuing platform.\",\n      \"maxLength\": 36\n    },\n    \"cardPackId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the card pack, used in card issuance and fulfillment.\",\n      \"maxLength\": 36\n    },\n    \"cardType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the card product.\",\n      \"enum\": [\n        \"CREDIT\",\n        \"DEBIT\",\n        \"PREPAID\",\n        \"COMMERCIAL\",\n        \"VIRTUAL\"\n      ]\n    },\n    \"cardProductCode\": {\n      \"type\": \"string\",\n      \"description\": \"Three-character code identifying the specific card product (e.g., MSI for Mastercard Standard, MWE for World Elite, MWO for World).\",\n      \"minLength\": 3,\n      \"maxLength\": 3,\n      \"examples\": [\"MSI\"]\n    },\n    \"planCode\": {\n      \"type\": \"string\",\n      \"description\": \"Card plan code defining the card product configuration and features.\",\n      \"maxLength\"\
  : 10\n    },\n    \"programCode\": {\n      \"type\": \"string\",\n      \"description\": \"Program code for the card product within the issuing institution.\",\n      \"maxLength\": 20\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Card brand within the Mastercard network.\",\n      \"enum\": [\n        \"MASTERCARD\",\n        \"MAESTRO\",\n        \"CIRRUS\"\n      ],\n      \"default\": \"MASTERCARD\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"description\": \"Card tier or level indicating the product benefits tier.\",\n      \"enum\": [\n        \"STANDARD\",\n        \"GOLD\",\n        \"PLATINUM\",\n        \"TITANIUM\",\n        \"WORLD\",\n        \"WORLD_ELITE\",\n        \"BLACK\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the card.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"INACTIVE\",\n        \"SUSPENDED\",\n        \"BLOCKED\",\n  \
  \      \"EXPIRED\",\n        \"CANCELLED\",\n        \"PENDING_ACTIVATION\"\n      ]\n    },\n    \"issuedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the card was issued, in ISO 8601 date format.\",\n      \"format\": \"date\",\n      \"examples\": [\"2024-01-26\"]\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"description\": \"Card expiration date in MMYY format.\",\n      \"pattern\": \"^(0[1-9]|1[0-2])[0-9]{2}$\",\n      \"minLength\": 4,\n      \"maxLength\": 4\n    },\n    \"embossedName\": {\n      \"type\": \"string\",\n      \"description\": \"Name embossed or printed on the physical card.\",\n      \"maxLength\": 26\n    },\n    \"numberless\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the card number is printed on the physical card. True means the number is not printed.\",\n      \"default\": false\n    },\n    \"instant\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates\
  \ whether the card was issued as an instant card (immediately generated).\",\n      \"default\": false\n    },\n    \"virtual\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this is a virtual card with no physical plastic.\",\n      \"default\": false\n    },\n    \"contactless\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the card supports contactless (NFC/PayPass) transactions.\",\n      \"default\": true\n    },\n    \"photoIndicator\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether a photo is required on the card.\",\n      \"enum\": [\"PHOTO\", \"NO_PHOTO\"]\n    },\n    \"deliveryMode\": {\n      \"type\": \"string\",\n      \"description\": \"Mode of card delivery to the cardholder.\",\n      \"enum\": [\n        \"BRANCH\",\n        \"COURIER\",\n        \"MAIL\",\n        \"DIGITAL\",\n        \"SELF_COLLECT\"\n      ]\n    },\n    \"deliveryDate\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Date the card was delivered or handed over to the client, in ISO 8601 format.\",\n      \"format\": \"date\"\n    },\n    \"tokenNumber\": {\n      \"type\": \"string\",\n      \"description\": \"MDES (Mastercard Digital Enablement Service) token representing this card for digital transactions.\",\n      \"pattern\": \"^[0-9]{12,19}$\",\n      \"minLength\": 12,\n      \"maxLength\": 19\n    },\n    \"binNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Bank Identification Number (BIN), the first 6-8 digits of the card number identifying the issuing institution.\",\n      \"pattern\": \"^[0-9]{6,8}$\",\n      \"minLength\": 6,\n      \"maxLength\": 8\n    },\n    \"issuerId\": {\n      \"type\": \"string\",\n      \"description\": \"ICA (Interbank Card Association) number of the issuing institution.\",\n      \"minLength\": 3,\n      \"maxLength\": 7\n    },\n    \"issuerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the\
  \ financial institution that issued the card.\",\n      \"maxLength\": 100\n    },\n    \"issuerCountryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-3 country code of the issuing institution.\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"minLength\": 3,\n      \"maxLength\": 3\n    },\n    \"cardholder\": {\n      \"$ref\": \"#/$defs/Cardholder\"\n    },\n    \"limits\": {\n      \"$ref\": \"#/$defs/CardLimits\"\n    },\n    \"applicationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of card issuance application.\",\n      \"enum\": [\n        \"PRIMARY_NEW_CLIENT\",\n        \"PRIMARY_EXISTING_CLIENT\",\n        \"SUPPLEMENTARY\",\n        \"ADD_ON\",\n        \"REPLACEMENT\",\n        \"RENEWAL\"\n      ]\n    },\n    \"corporateCode\": {\n      \"type\": \"string\",\n      \"description\": \"Unique code of the corporate entity for commercial/corporate cards.\",\n      \"pattern\": \"^[0-9]+$\",\n      \"maxLength\": 24\n \
  \   }\n  },\n  \"$defs\": {\n    \"Cardholder\": {\n      \"type\": \"object\",\n      \"description\": \"The individual to whom the card is issued.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the cardholder.\",\n          \"maxLength\": 100\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the cardholder.\",\n          \"maxLength\": 50\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the cardholder.\",\n          \"maxLength\": 50\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"description\": \"Email address of the cardholder.\",\n          \"format\": \"email\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number of the cardholder.\",\n          \"maxLength\": 20\n        },\n        \"clientType\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Classification of the cardholder.\",\n          \"enum\": [\n            \"INDIVIDUAL\",\n            \"CORPORATE\",\n            \"SMALL_BUSINESS\"\n          ]\n        },\n        \"vip\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the cardholder is classified as a VIP client.\",\n          \"default\": false\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n    },\n    \"CardLimits\": {\n      \"type\": \"object\",\n      \"description\": \"Transaction limits configured for the card.\",\n      \"properties\": {\n        \"perTransactionLimit\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum amount permitted per transaction, without decimals.\",\n          \"pattern\": \"^[0-9]+$\",\n          \"maxLength\": 12,\n          \"examples\": [\"100000\"]\n        },\n        \"dailyLimit\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Maximum total amount permitted per day, without decimals.\",\n          \"pattern\": \"^[0-9]+$\",\n          \"maxLength\": 12\n        },\n        \"totalTransactionLimit\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum cumulative transaction limit for the card.\",\n          \"pattern\": \"^[0-9]+$\",\n          \"maxLength\": 20,\n          \"examples\": [\"10000000\"]\n        },\n        \"velocity\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum number of transactions allowed within a configured duration.\",\n          \"pattern\": \"^[0-9]+$\",\n          \"maxLength\": 20\n        },\n        \"validity\": {\n          \"type\": \"string\",\n          \"description\": \"Card validity duration in ISO 8601 duration format (e.g., P3M4DT12H30M5S). Maximum validity is 3 years.\",\n          \"pattern\": \"^P(?!$)([0-9]+Y)?([0-9]+M)?([0-9]+W)?([0-9]+D)?(T(?=[0-9])([0-9]+H)?([0-9]+M)?([0-9]+S)?)?$\"\
  ,\n          \"maxLength\": 19\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A postal address.\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\",\n          \"description\": \"First line of the street address.\",\n          \"maxLength\": 50\n        },\n        \"line2\": {\n          \"type\": \"string\",\n          \"description\": \"Second line of the street address.\",\n          \"maxLength\": 50\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name.\",\n          \"maxLength\": 50\n        },\n        \"stateProvinceCode\": {\n          \"type\": \"string\",\n          \"description\": \"State or province code.\",\n          \"maxLength\": 3\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code.\",\n          \"maxLength\": 10\n        },\n        \"countryCode\": {\n      \
  \    \"type\": \"string\",\n          \"description\": \"ISO 3166-1 alpha-3 country code.\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"minLength\": 3,\n          \"maxLength\": 3\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/card.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Mastercard Card
---
