---
description: AdditionalDataTemporaryServices schema from Adyen API
layout: schema
name: AdditionalDataTemporaryServices
properties_list:
- description: 'The customer code, if supplied by a customer. * Encoding: ASCII * maxLength: 25'
  name: enhancedSchemeData.customerReference
  type: string
- description: 'The name or ID of the person working in a temporary capacity. * maxLength: 40. * Must not be all spaces. *Must not be all zeros.'
  name: enhancedSchemeData.employeeName
  type: string
- description: 'The job description of the person working in a temporary capacity. * maxLength: 40 * Must not be all spaces. *Must not be all zeros.'
  name: enhancedSchemeData.jobDescription
  type: string
- description: 'The amount paid for regular hours worked, [minor units](https://docs.adyen.com/development-resources/currency-codes). * maxLength: 7 * Must not be empty * Can be all zeros'
  name: enhancedSchemeData.regularHoursRate
  type: string
- description: 'The hours worked. * maxLength: 7 * Must not be empty * Can be all zeros'
  name: enhancedSchemeData.regularHoursWorked
  type: string
- description: 'The name of the person requesting temporary services. * maxLength: 40 * Must not be all zeros * Must not be all spaces'
  name: enhancedSchemeData.requestName
  type: string
- description: 'The billing period start date. * Format: ddMMyy * maxLength: 6'
  name: enhancedSchemeData.tempStartDate
  type: string
- description: 'The billing period end date. * Format: ddMMyy * maxLength: 6'
  name: enhancedSchemeData.tempWeekEnding
  type: string
- description: 'The total tax amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). For example, 2000 means USD 20.00 * maxLength: 12'
  name: enhancedSchemeData.totalTaxAmount
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-additional-data-temporary-services-schema.json
slug: checkout-additional-data-temporary-services
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-temporary-services-schema.json\",\n  \"title\": \"AdditionalDataTemporaryServices\",\n  \"description\": \"AdditionalDataTemporaryServices schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enhancedSchemeData.customerReference\": {\n      \"description\": \"The customer code, if supplied by a customer.\\n* Encoding: ASCII\\n* maxLength: 25\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.employeeName\": {\n      \"description\": \"The name or ID of the person working in a temporary capacity.\\n* maxLength: 40.  \\n* Must not be all spaces. \\n*Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.jobDescription\": {\n      \"description\": \"The job description of the person working in a temporary capacity.\\n*\
  \ maxLength: 40 \\n* Must not be all spaces. \\n*Must not be all zeros.\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.regularHoursRate\": {\n      \"description\": \"The amount paid for regular hours worked, [minor units](https://docs.adyen.com/development-resources/currency-codes).\\n* maxLength: 7\\n* Must not be empty\\n* Can be all zeros\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.regularHoursWorked\": {\n      \"description\": \"The hours worked.\\n* maxLength: 7\\n* Must not be empty\\n* Can be all zeros\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.requestName\": {\n      \"description\": \"The name of the person requesting temporary services.\\n* maxLength: 40\\n* Must not be all zeros\\n* Must not be all spaces\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.tempStartDate\": {\n      \"description\": \"The billing period start date.\\n* Format: ddMMyy\\n* maxLength: 6\",\n      \"type\": \"string\"\n \
  \   },\n    \"enhancedSchemeData.tempWeekEnding\": {\n      \"description\": \"The billing period end date.\\n* Format: ddMMyy\\n* maxLength: 6\",\n      \"type\": \"string\"\n    },\n    \"enhancedSchemeData.totalTaxAmount\": {\n      \"description\": \"The total tax amount, in [minor units](https://docs.adyen.com/development-resources/currency-codes). For example, 2000 means USD 20.00\\n* maxLength: 12\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-additional-data-temporary-services-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AdditionalDataTemporaryServices
---
