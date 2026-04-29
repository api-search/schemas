---
description: ''
layout: schema
name: Gift
properties_list:
- description: ''
  name: amount
  type: number
- description: ''
  name: currencyIsoCode
  type: string
- description: ''
  name: receivedDate
  type: string
- description: ''
  name: donorCoverAmount
  type: number
- description: ''
  name: transactionStatus
  type: string
- description: ''
  name: commitmentId
  type: string
- description: ''
  name: paymentIdentifier
  type: string
- description: ''
  name: gatewayTransactionFee
  type: number
- description: ''
  name: processorTransactionFee
  type: number
- description: ''
  name: processorReference
  type: string
- description: ''
  name: gatewayReference
  type: string
- description: ''
  name: lastGatewayResponseCode
  type: string
- description: ''
  name: lastGatewayErrorMessage
  type: string
- description: ''
  name: lastGatewayProcessedDateTime
  type: string
- description: ''
  name: campaign
  type: object
- description: ''
  name: outreachSourceCode
  type: object
- description: ''
  name: donor
  type: object
- description: ''
  name: paymentInstrument
  type: object
- description: ''
  name: designations
  type: array
- description: ''
  name: giftTransactionCustomFields
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-gift-schema.json
slug: salesforce-gift
source_filename: salesforce-gift-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"currencyIsoCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"receivedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"donorCoverAmount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"transactionStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"commitmentId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"paymentIdentifier\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"gatewayTransactionFee\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"processorTransactionFee\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"processorReference\": {\n      \"type\": \"string\",\n      \"\
  example\": \"example_value\"\n    },\n    \"gatewayReference\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayResponseCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayErrorMessage\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayProcessedDateTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"campaign\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"outreachSourceCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"sourceCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\
  \n        }\n      },\n      \"required\": [\n        \"id\",\n        \"sourceCode\"\n      ]\n    },\n    \"donor\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"donorType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"organizationName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"example\": \"user@example.com\"\n        },\n        \"address\": {\n          \"type\": \"\
  array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"addressType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"street\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"city\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"state\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"postalCode\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"country\": {\n                \"type\": \"string\",\n                \"example\": 42\n              }\n            },\n            \"required\": [\n\
  \              \"addressType\",\n              \"street\",\n              \"city\",\n              \"state\",\n              \"postalCode\",\n              \"country\"\n            ]\n          }\n        },\n        \"accountCustomFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": 42,\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"fieldName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"fieldValue\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"fieldName\",\n              \"fieldValue\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"donorType\",\n        \"id\",\n        \"organizationName\",\n        \"firstName\",\n        \"lastName\",\n\
  \        \"phone\",\n        \"email\",\n        \"address\",\n        \"accountCustomFields\"\n      ]\n    },\n    \"paymentInstrument\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"accountHolderName\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"expiryMonth\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"expiryYear\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"last4\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"cardBrand\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"bankName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"digitalWalletProvider\"\
  : {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"bankAccountHolderType\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankAccountType\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankAccountNumber\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"gatewayName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"processorName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"processorPaymentReference\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"gatewayReference\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n      \
  \  }\n      },\n      \"required\": [\n        \"type\",\n        \"accountHolderName\",\n        \"expiryMonth\",\n        \"expiryYear\",\n        \"last4\",\n        \"cardBrand\",\n        \"bankName\",\n        \"digitalWalletProvider\",\n        \"bankAccountHolderType\",\n        \"bankAccountType\",\n        \"bankAccountNumber\",\n        \"bankCode\",\n        \"gatewayName\",\n        \"processorName\",\n        \"processorPaymentReference\",\n        \"gatewayReference\"\n      ]\n    },\n    \"designations\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"designationId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"percent\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"amount\": {\n            \"type\": \"number\",\n            \"example\": 42.5\n\
  \          }\n        },\n        \"required\": [\n          \"designationId\",\n          \"percent\",\n          \"amount\"\n        ]\n      }\n    },\n    \"giftTransactionCustomFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fieldValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"fieldName\",\n          \"fieldValue\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"currencyIsoCode\",\n    \"receivedDate\",\n    \"donorCoverAmount\",\n    \"transactionStatus\",\n    \"commitmentId\",\n    \"paymentIdentifier\",\n    \"gatewayTransactionFee\",\n    \"processorTransactionFee\",\n    \"processorReference\"\
  ,\n    \"gatewayReference\",\n    \"lastGatewayResponseCode\",\n    \"lastGatewayErrorMessage\",\n    \"lastGatewayProcessedDateTime\",\n    \"campaign\",\n    \"outreachSourceCode\",\n    \"donor\",\n    \"paymentInstrument\",\n    \"designations\",\n    \"giftTransactionCustomFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Gift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-gift-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Gift
---
