---
description: ''
layout: schema
name: Commitment
properties_list:
- description: ''
  name: amount
  type: number
- description: ''
  name: currencyIsoCode
  type: string
- description: ''
  name: transactionPeriod
  type: string
- description: ''
  name: transactionInterval
  type: integer
- description: ''
  name: transactionDay
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
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
  name: firstTransaction
  type: object
- description: ''
  name: giftCommitmentCustomFields
  type: array
- description: ''
  name: giftCommitmentScheduleCustomFields
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-commitment-schema.json
slug: salesforce-commitment
source_filename: salesforce-commitment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"currencyIsoCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"transactionPeriod\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"transactionInterval\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"transactionDay\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"campaign\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"outreachSourceCode\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"sourceCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"sourceCode\"\n      ]\n    },\n    \"donor\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"donorType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"email\": {\n\
  \          \"type\": \"string\",\n          \"example\": \"user@example.com\"\n        },\n        \"address\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"addressType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"street\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"city\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"state\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"postalCode\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"country\"\
  : {\n                \"type\": \"string\",\n                \"example\": 42\n              }\n            },\n            \"required\": [\n              \"addressType\",\n              \"street\",\n              \"city\",\n              \"state\",\n              \"postalCode\",\n              \"country\"\n            ]\n          }\n        },\n        \"accountCustomFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": 42,\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"fieldName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"fieldValue\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"fieldName\",\n              \"fieldValue\"\n            ]\n          }\n        }\n      },\n    \
  \  \"required\": [\n        \"donorType\",\n        \"id\",\n        \"firstName\",\n        \"lastName\",\n        \"phone\",\n        \"email\",\n        \"address\",\n        \"accountCustomFields\"\n      ]\n    },\n    \"paymentInstrument\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"accountHolderName\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"expiryMonth\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"expiryYear\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"last4\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"cardBrand\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"bankName\": {\n     \
  \     \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"digitalWalletProvider\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"bankAccountHolderType\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankAccountType\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankAccountNumber\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"gatewayName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"processorName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"processorPaymentReference\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n\
  \        \"gatewayReference\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"accountHolderName\",\n        \"expiryMonth\",\n        \"expiryYear\",\n        \"last4\",\n        \"cardBrand\",\n        \"bankName\",\n        \"digitalWalletProvider\",\n        \"bankAccountHolderType\",\n        \"bankAccountType\",\n        \"bankAccountNumber\",\n        \"bankCode\",\n        \"gatewayName\",\n        \"processorName\",\n        \"processorPaymentReference\",\n        \"gatewayReference\"\n      ]\n    },\n    \"designations\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"designationId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"percent\": {\n            \"type\": \"integer\",\n            \"\
  example\": 10\n          }\n        },\n        \"required\": [\n          \"designationId\",\n          \"percent\"\n        ]\n      }\n    },\n    \"firstTransaction\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"number\",\n          \"example\": 42.5\n        },\n        \"receivedDate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"donorCoverAmount\": {\n          \"type\": \"number\",\n          \"example\": 42.5\n        },\n        \"transactionStatus\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"gatewayTransactionFee\": {\n          \"type\": \"number\",\n          \"example\": 42.5\n        },\n        \"processorTransactionFee\": {\n          \"type\": \"number\",\n          \"example\": 42.5\n        },\n        \"processorReference\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\
  \n        },\n        \"gatewayReference\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastGatewayResponseCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastGatewayErrorMessage\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastGatewayProcessedDateTime\": {\n          \"type\": \"string\",\n          \"example\": \"2026-01-15T10:30:00Z\"\n        }\n      },\n      \"required\": [\n        \"amount\",\n        \"receivedDate\",\n        \"donorCoverAmount\",\n        \"transactionStatus\",\n        \"gatewayTransactionFee\",\n        \"processorTransactionFee\",\n        \"processorReference\",\n        \"gatewayReference\",\n        \"lastGatewayResponseCode\",\n        \"lastGatewayErrorMessage\",\n        \"lastGatewayProcessedDateTime\"\n      ]\n    },\n    \"giftCommitmentCustomFields\": {\n      \"type\": \"\
  array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fieldValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"fieldName\",\n          \"fieldValue\"\n        ]\n      }\n    },\n    \"giftCommitmentScheduleCustomFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fieldValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"\
  fieldName\",\n          \"fieldValue\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"currencyIsoCode\",\n    \"transactionPeriod\",\n    \"transactionInterval\",\n    \"transactionDay\",\n    \"startDate\",\n    \"endDate\",\n    \"campaign\",\n    \"outreachSourceCode\",\n    \"donor\",\n    \"paymentInstrument\",\n    \"designations\",\n    \"firstTransaction\",\n    \"giftCommitmentCustomFields\",\n    \"giftCommitmentScheduleCustomFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Commitment\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-commitment-schema.json
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
title: Commitment
---
