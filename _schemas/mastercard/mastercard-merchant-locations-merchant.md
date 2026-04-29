---
description: Merchant detail information
layout: schema
name: Merchant
properties_list:
- description: Line 1 of the street address for the merchant location. Usually includes the street number and name.
  name: addressLine1
  type: string
- description: Line 2 of the street address usually an apartment number or suite number.
  name: addressLine2
  type: string
- description: Maximum cashback amount permitted at the location.
  name: cashbackMaximumAmount
  type: string
- description: The Merchant Category
  name: category
  type: string
- description: Two digit alpha country code as defined in ISO
  name: countryCode
  type: string
- description: Name of the country.
  name: countryName
  type: string
- description: Code of the state or province for a merchant location.
  name: countrySubdivisionCode
  type: string
- description: Name of the state or province for a merchant location.
  name: countrySubdivisionName
  type: string
- description: The name of the city for a merchant location.
  name: city
  type: string
- description: This is the numerical value for the distance from the provided location to the selected merchant.
  name: distance
  type: number
- description: This is the unit of measure value for the distance from the provided location to the selected merchant. Options are KM and MILE.
  name: distanceUnit
  type: string
- description: Merchant's Easy Savings Offer Id
  name: easySavingsMerchantOfferId
  type: string
- description: GeocodingResult for the merchant
  name: geocodingResult
  type: string
- description: Numerical merchant identifier.
  name: id
  type: integer
- description: Boolean value which indicates if the concession area is equipped with a PayPass card reader.
  name: isPayPassConcession
  type: boolean
- description: Boolean value which indicates if the pharmacy is equipped with a PayPass card reader.
  name: isPayPassPharmacy
  type: boolean
- description: Boolean value which indicates if the fuel pump is equipped with a PayPass card reader.
  name: isPayPassFuelPump
  type: boolean
- description: Boolean value which indicates if the toll booth is equipped with a PayPass card reader.
  name: isPayPassTollBooth
  type: boolean
- description: Boolean value which indicates if the drive thru is equipped with a PayPass card reader.
  name: isPayPassDriveThrough
  type: boolean
- description: Boolean value which indicates if the register is equipped with a PayPass card reader.
  name: isPayPassRegister
  type: boolean
- description: Boolean value which indicates if the ticketing area is equipped with a PayPass card reader.
  name: isPayPassTicketing
  type: boolean
- description: Boolean value which indicates if the vending machine is equipped with a PayPass card reader.
  name: isPayPassVendingMachine
  type: boolean
- description: Boolean value which indicates if the repower card load type at this merchant supports Card Swipe.
  name: isRepowerByCardSwipeSupported
  type: boolean
- description: Boolean value which indicates if the repower card load type at this merchant supports MoneyPak.
  name: isRepowerByMoneyPakSupported
  type: boolean
- description: The latitude of the merchant
  name: latitude
  type: string
- description: The name of the merchant
  name: locationName
  type: string
- description: The longitude of the merchant.
  name: longitude
  type: string
- description: Merchant's phone number
  name: phoneNumber
  type: string
- description: The postal code of the Merchant location.
  name: postalCode
  type: string
- description: Merchant's website URL address
  name: websiteUrl
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-merchant-locations-merchant-schema.json
slug: mastercard-merchant-locations-merchant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Merchant\",\n  \"type\": \"object\",\n  \"description\": \"Merchant detail information\",\n  \"properties\": {\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"Line 1 of the street address for the merchant location. Usually includes the street number and name.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Line 2 of the street address usually an apartment number or suite number.\"\n    },\n    \"cashbackMaximumAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum cashback amount permitted at the location.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The Merchant Category\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Two digit alpha country code as defined in ISO\"\n    },\n    \"countryName\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Name of the country.\"\n    },\n    \"countrySubdivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Code of the state or province for a merchant location.\"\n    },\n    \"countrySubdivisionName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the state or province for a merchant location.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the city for a merchant location.\"\n    },\n    \"distance\": {\n      \"type\": \"number\",\n      \"description\": \"This is the numerical value for the distance from the provided location to the selected merchant.\"\n    },\n    \"distanceUnit\": {\n      \"type\": \"string\",\n      \"description\": \"This is the unit of measure value for the distance from the provided location to the selected merchant. Options are KM and MILE.\"\n    },\n    \"easySavingsMerchantOfferId\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"Merchant's Easy Savings Offer Id\"\n    },\n    \"geocodingResult\": {\n      \"type\": \"string\",\n      \"description\": \"GeocodingResult for the merchant\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numerical merchant identifier.\"\n    },\n    \"isPayPassConcession\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the concession area is equipped with a PayPass card reader.\"\n    },\n    \"isPayPassPharmacy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the pharmacy is equipped with a PayPass card reader.\"\n    },\n    \"isPayPassFuelPump\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the fuel pump is equipped with a PayPass card reader.\"\n    },\n    \"isPayPassTollBooth\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the toll booth is equipped with a PayPass\
  \ card reader.\"\n    },\n    \"isPayPassDriveThrough\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the drive thru is equipped with a PayPass card reader.\"\n    },\n    \"isPayPassRegister\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the register is equipped with a PayPass card reader.\"\n    },\n    \"isPayPassTicketing\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the ticketing area is equipped with a PayPass card reader.\"\n    },\n    \"isPayPassVendingMachine\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the vending machine is equipped with a PayPass card reader.\"\n    },\n    \"isRepowerByCardSwipeSupported\": {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the repower card load type at this merchant supports Card Swipe.\"\n    },\n    \"isRepowerByMoneyPakSupported\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Boolean value which indicates if the repower card load type at this merchant supports MoneyPak.\"\n    },\n    \"latitude\": {\n      \"type\": \"string\",\n      \"description\": \"The latitude of the merchant\"\n    },\n    \"locationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the merchant\"\n    },\n    \"longitude\": {\n      \"type\": \"string\",\n      \"description\": \"The longitude of the merchant.\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant's phone number\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code of the Merchant location.\"\n    },\n    \"websiteUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant's website URL address\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-merchant-locations-merchant-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Merchant
---
