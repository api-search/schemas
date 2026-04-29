---
description: AdditionalDataLodging schema from Adyen API
layout: schema
name: AdditionalDataLodging
properties_list:
- description: 'The arrival date. * Date format: **yyyyMmDd**. For example, for 2023 April 22, **20230422**.'
  name: lodging.checkInDate
  type: string
- description: 'The departure date. * Date format: **yyyyMmDd**. For example, for 2023 April 22, **20230422**.'
  name: lodging.checkOutDate
  type: string
- description: 'The toll-free phone number for the lodging. * Format: numeric * Max length: 17 characters. * For US and CA numbers must be 10 characters in length * Must not start with a space * Must not contain any '
  name: lodging.customerServiceTollFreeNumber
  type: string
- description: 'Identifies that the facility complies with the Hotel and Motel Fire Safety Act of 1990. Must be ''Y'' or ''N''. * Format: alphabetic * Max length: 1 character'
  name: lodging.fireSafetyActIndicator
  type: string
- description: 'The folio cash advances, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * Format: numeric * Max length: 12 characters'
  name: lodging.folioCashAdvances
  type: string
- description: 'The card acceptor’s internal invoice or billing ID reference number. * Max length: 25 characters. * Must not start with a space *Must not be all zeros.'
  name: lodging.folioNumber
  type: string
- description: 'Any charges for food and beverages associated with the booking, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * Format: numeric * Max length: 12 characters'
  name: lodging.foodBeverageCharges
  type: string
- description: 'Indicates if the customer didn''t check in for their booking. Possible values: * **Y**: the customer didn''t check in * **N**: the customer checked in'
  name: lodging.noShowIndicator
  type: string
- description: 'The prepaid expenses for the booking. * Format: numeric * Max length: 12 characters'
  name: lodging.prepaidExpenses
  type: string
- description: 'The lodging property location''s phone number. * Format: numeric. * Min length: 10 characters * Max length: 17 characters * For US and CA numbers must be 10 characters in length * Must not start with a'
  name: lodging.propertyPhoneNumber
  type: string
- description: 'The total number of nights the room is booked for. * Format: numeric * Must be a number between 0 and 99 * Max length: 4 characters'
  name: lodging.room1.numberOfNights
  type: string
- description: 'The rate for the room, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * Format: numeric * Max length: 12 characters * Must not be a negative number'
  name: lodging.room1.rate
  type: string
- description: 'The total room tax amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * Format: numeric * Max length: 12 characters * Must not be a negative number'
  name: lodging.totalRoomTax
  type: string
- description: 'The total tax amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). * Format: numeric * Max length: 12 characters * Must not be a negative number'
  name: lodging.totalTax
  type: string
- description: 'The number of nights. This should be included in the auth message. * Format: numeric * Max length: 4 characters'
  name: travelEntertainmentAuthData.duration
  type: string
- description: 'Indicates what market-specific dataset will be submitted. Must be ''H'' for Hotel. This should be included in the auth message. * Format: alphanumeric * Max length: 1 character'
  name: travelEntertainmentAuthData.market
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-additional-data-lodging-schema.json
slug: checkout-additional-data-lodging
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-lodging-schema.json\",\n  \"title\": \"AdditionalDataLodging\",\n  \"description\": \"AdditionalDataLodging schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lodging.checkInDate\": {\n      \"description\": \"The arrival date.\\n* Date format: **yyyyMmDd**. For example, for 2023 April 22, **20230422**.\",\n      \"type\": \"string\"\n    },\n    \"lodging.checkOutDate\": {\n      \"description\": \"The departure date.\\n* Date format: **yyyyMmDd**. For example, for 2023 April 22, **20230422**.\",\n      \"type\": \"string\"\n    },\n    \"lodging.customerServiceTollFreeNumber\": {\n      \"description\": \"The toll-free phone number for the lodging.\\n* Format: numeric\\n* Max length: 17 characters.\\n* For US and CA numbers must be 10 characters in length\\n*\
  \ Must not start with a space\\n* Must not contain any special characters such as + or -\\n*Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"lodging.fireSafetyActIndicator\": {\n      \"description\": \"Identifies that the facility complies with the Hotel and Motel Fire Safety Act of 1990. Must be 'Y' or 'N'.\\n* Format: alphabetic\\n* Max length: 1 character\",\n      \"type\": \"string\"\n    },\n    \"lodging.folioCashAdvances\": {\n      \"description\": \"The folio cash advances, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* Format: numeric\\n* Max length: 12 characters\",\n      \"type\": \"string\"\n    },\n    \"lodging.folioNumber\": {\n      \"description\": \"The card acceptor\\u2019s internal invoice or billing ID reference number.\\n* Max length: 25 characters.\\n* Must not start with a space\\n*Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"lodging.foodBeverageCharges\": {\n      \"description\"\
  : \"Any charges for food and beverages associated with the booking, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* Format: numeric\\n* Max length: 12 characters\",\n      \"type\": \"string\"\n    },\n    \"lodging.noShowIndicator\": {\n      \"description\": \"Indicates if the customer didn't check in for their booking.\\n Possible values: \\n* **Y**: the customer didn't check in \\n* **N**: the customer checked in\",\n      \"type\": \"string\"\n    },\n    \"lodging.prepaidExpenses\": {\n      \"description\": \"The prepaid expenses for the booking.\\n* Format: numeric\\n* Max length: 12 characters\",\n      \"type\": \"string\"\n    },\n    \"lodging.propertyPhoneNumber\": {\n      \"description\": \"The lodging property location's phone number.\\n* Format: numeric.\\n* Min length: 10 characters\\n* Max length: 17 characters\\n* For US and CA numbers must be 10 characters in length\\n* Must not start with a space\\n* Must not contain any special\
  \ characters such as + or -\\n*Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"lodging.room1.numberOfNights\": {\n      \"description\": \"The total number of nights the room is booked for.\\n* Format: numeric\\n* Must be a number between 0 and 99\\n* Max length: 4 characters\",\n      \"type\": \"string\"\n    },\n    \"lodging.room1.rate\": {\n      \"description\": \"The rate for the room, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* Format: numeric\\n* Max length: 12 characters\\n* Must not be a negative number\",\n      \"type\": \"string\"\n    },\n    \"lodging.totalRoomTax\": {\n      \"description\": \"The total room tax amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* Format: numeric\\n* Max length: 12 characters\\n* Must not be a negative number\",\n      \"type\": \"string\"\n    },\n    \"lodging.totalTax\": {\n      \"description\": \"The total tax amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes).\\\
  n* Format: numeric\\n* Max length: 12 characters\\n* Must not be a negative number\",\n      \"type\": \"string\"\n    },\n    \"travelEntertainmentAuthData.duration\": {\n      \"description\": \"The number of nights. This should be included in the auth message.\\n* Format: numeric\\n* Max length: 4 characters\",\n      \"type\": \"string\"\n    },\n    \"travelEntertainmentAuthData.market\": {\n      \"description\": \"Indicates what market-specific dataset will be submitted. Must be 'H' for Hotel. This should be included in the auth message.\\n\\n* Format: alphanumeric\\n* Max length: 1 character\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-lodging-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataLodging
---
