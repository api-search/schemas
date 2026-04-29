---
description: ATM detail information
layout: schema
name: Atm
properties_list:
- description: This value indicates under what conditions access fees are charged. Options are UNKNOWN, DOMESTIC, INTERNATIONAL, DOMESTIC_AND_INTERNATIONAL, NO_FEE.
  name: accessFees
  type: string
- description: Line 1 of the street address for the ATM location. Usually includes the street number and name.
  name: addressLine1
  type: string
- description: Line 2 of the street address usually an apartment number or suite number.
  name: addressLine2
  type: string
- description: The Airport Code
  name: airportCode
  type: string
- description: The ATM Terminal Id
  name: atmTerminalId
  type: string
- description: This value indicates the availability hours of the ATM. Options are UNKNOWN, ALWAYS_AVAILABLE, BUSINESS_HOURS, IRREGULAR_HOURS.
  name: availability
  type: string
- description: This value indicates whether or not a security camera is present or near ATM
  name: camera
  type: string
- description: Three digit alpha country code as defined in ISO
  name: countryCode
  type: string
- description: Name of the country.
  name: countryName
  type: string
- description: Code of the state or province for an ATM location.
  name: countrySubdivisionCode
  type: string
- description: Name of the state or province for an ATM location.
  name: countrySubdivisionName
  type: string
- description: The name of the city for an ATM location.
  name: city
  type: string
- description: This is the numerical value for the distance from the provided location to the selected ATM.
  name: distance
  type: number
- description: This is the unit of measure value for the distance from the provided location to the selected ATM. Options are KM and MILE.
  name: distanceUnit
  type: string
- description: GeocodingResult for the ATM
  name: geocodingResult
  type: string
- description: This indicates whether the ATM has the ability to read chip cards or not. Options are UNKNOWN, IS_HANDICAP_ACCESSIBLE, NOT_HANDICAP_ACCESSIBLE.
  name: handicapAccessible
  type: string
- description: This value indicates whether or not the ATM participates in the Mastercard Shared Deposit network. Options are YES or NO.
  name: hasSharedDeposit
  type: string
- description: This value indicates whether or not the ATM participates in the Mastercard Shared (only) Surcharge Free Alliance network. Options are YES or NO.
  name: isSurchargeFreeAlliance
  type: string
- description: The latitude of the ATM
  name: latitude
  type: string
- description: The name of the ATM location
  name: locationName
  type: string
- description: Type of location for the ATM. Options are OTHER, AIRPORT, HOSPITAL, FINANCIAL_INSTITUTION.
  name: locationType
  type: string
- description: The longitude of the ATM.
  name: longitude
  type: string
- description: This is the DBA name of the financial institution affiliate or independent service organization.
  name: owner
  type: string
- description: This is the ICA of the entity that owns the ATM
  name: ownerICA
  type: string
- description: The postal code of the ATM location.
  name: postalCode
  type: string
- description: The routing transaction number
  name: routeTransactionNumber
  type: string
- description: This is the legal or business name of the entity that sponsors the owner of the ATM into the Mastercard network.
  name: sponsor
  type: string
- description: This is the ICA of entity that sponsors the owner of the ATM
  name: sponsorICA
  type: string
- description: This indicates whether the ATM has the ability to read chip cards or not. Options are UNKNOWN, SUPPORTS_EMV, DOES_NOT_SUPPORT_EMV.
  name: supportsEmv
  type: string
- description: This value indicates whether or not the ATM participates in the Mastercard Shared (only) Surcharge Free Alliance network. Options are DOES_NOT_PARTICIPATE_IN_SFA, ALLPOINT_PREPAID, MONEYPASS_DEBIT, an
  name: surchargeFreeAllianceNetwork
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-atm-locations-atm-schema.json
slug: mastercard-atm-locations-atm
source_filename: mastercard-atm-locations-atm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Atm\",\n  \"type\": \"object\",\n  \"description\": \"ATM detail information\",\n  \"properties\": {\n    \"accessFees\": {\n      \"type\": \"string\",\n      \"description\": \"This value indicates under what conditions access fees are charged. Options are UNKNOWN, DOMESTIC, INTERNATIONAL, DOMESTIC_AND_INTERNATIONAL, NO_FEE.\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"Line 1 of the street address for the ATM location. Usually includes the street number and name.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"Line 2 of the street address usually an apartment number or suite number.\"\n    },\n    \"airportCode\": {\n      \"type\": \"string\",\n      \"description\": \"The Airport Code\"\n    },\n    \"atmTerminalId\": {\n      \"type\": \"string\",\n      \"description\": \"The ATM Terminal Id\"\n    },\n\
  \    \"availability\": {\n      \"type\": \"string\",\n      \"description\": \"This value indicates the availability hours of the ATM. Options are UNKNOWN, ALWAYS_AVAILABLE, BUSINESS_HOURS, IRREGULAR_HOURS.\"\n    },\n    \"camera\": {\n      \"type\": \"string\",\n      \"description\": \"This value indicates whether or not a security camera is present or near ATM\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Three digit alpha country code as defined in ISO\"\n    },\n    \"countryName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the country.\"\n    },\n    \"countrySubdivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"Code of the state or province for an ATM location.\"\n    },\n    \"countrySubdivisionName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the state or province for an ATM location.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The name of the city for an ATM location.\"\n    },\n    \"distance\": {\n      \"type\": \"number\",\n      \"description\": \"This is the numerical value for the distance from the provided location to the selected ATM.\"\n    },\n    \"distanceUnit\": {\n      \"type\": \"string\",\n      \"description\": \"This is the unit of measure value for the distance from the provided location to the selected ATM. Options are KM and MILE.\"\n    },\n    \"geocodingResult\": {\n      \"type\": \"string\",\n      \"description\": \"GeocodingResult for the ATM\"\n    },\n    \"handicapAccessible\": {\n      \"type\": \"string\",\n      \"description\": \"This indicates whether the ATM has the ability to read chip cards or not. Options are UNKNOWN, IS_HANDICAP_ACCESSIBLE, NOT_HANDICAP_ACCESSIBLE.\"\n    },\n    \"hasSharedDeposit\": {\n      \"type\": \"string\",\n      \"description\": \"This value indicates whether or not the ATM participates in the Mastercard Shared Deposit network. Options are\
  \ YES or NO.\"\n    },\n    \"isSurchargeFreeAlliance\": {\n      \"type\": \"string\",\n      \"description\": \"This value indicates whether or not the ATM participates in the Mastercard Shared (only) Surcharge Free Alliance network. Options are YES or NO.\"\n    },\n    \"latitude\": {\n      \"type\": \"string\",\n      \"description\": \"The latitude of the ATM\"\n    },\n    \"locationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the ATM location\"\n    },\n    \"locationType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of location for the ATM. Options are OTHER, AIRPORT, HOSPITAL, FINANCIAL_INSTITUTION.\"\n    },\n    \"longitude\": {\n      \"type\": \"string\",\n      \"description\": \"The longitude of the ATM.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"This is the DBA name of the financial institution affiliate or independent service organization.\"\n    },\n    \"ownerICA\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"This is the ICA of the entity that owns the ATM\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code of the ATM location.\"\n    },\n    \"routeTransactionNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The routing transaction number\"\n    },\n    \"sponsor\": {\n      \"type\": \"string\",\n      \"description\": \"This is the legal or business name of the entity that sponsors the owner of the ATM into the Mastercard network.\"\n    },\n    \"sponsorICA\": {\n      \"type\": \"string\",\n      \"description\": \"This is the ICA of entity that sponsors the owner of the ATM\"\n    },\n    \"supportsEmv\": {\n      \"type\": \"string\",\n      \"description\": \"This indicates whether the ATM has the ability to read chip cards or not. Options are UNKNOWN, SUPPORTS_EMV, DOES_NOT_SUPPORT_EMV.\"\n    },\n    \"surchargeFreeAllianceNetwork\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"This value indicates whether or not the ATM participates in the Mastercard Shared (only) Surcharge Free Alliance network. Options are DOES_NOT_PARTICIPATE_IN_SFA, ALLPOINT_PREPAID, MONEYPASS_DEBIT, and ALL_SURCHARGE_FREE.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-atm-locations-atm-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Atm
---
