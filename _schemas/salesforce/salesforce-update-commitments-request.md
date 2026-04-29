---
description: ''
layout: schema
name: UpdateCommitmentsRequest
properties_list:
- description: ''
  name: amount
  type: number
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
  name: giftCommitmentCustomFields
  type: array
- description: ''
  name: giftCommitmentScheduleCustomFields
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-update-commitments-request-schema.json
slug: salesforce-update-commitments-request
source_filename: salesforce-update-commitments-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"transactionPeriod\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"transactionInterval\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"transactionDay\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"campaign\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"example\": \"abc123\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"outreachSourceCode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"\
  string\",\n          \"example\": \"abc123\"\n        },\n        \"sourceCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"id\",\n        \"sourceCode\"\n      ]\n    },\n    \"donor\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"donorType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"organizationName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"example\": \"user@example.com\"\n\
  \        },\n        \"address\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"addressType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"street\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"city\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"state\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"postalCode\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"country\": {\n                \"type\": \"string\",\n                \"example\": 42\n\
  \              }\n            },\n            \"required\": [\n              \"addressType\",\n              \"street\",\n              \"city\",\n              \"state\",\n              \"postalCode\",\n              \"country\"\n            ]\n          }\n        },\n        \"accountCustomFields\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": 42,\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"fieldName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"fieldValue\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"fieldName\",\n              \"fieldValue\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"donorType\",\n        \"organizationName\",\n  \
  \      \"firstName\",\n        \"lastName\",\n        \"phone\",\n        \"email\",\n        \"address\",\n        \"accountCustomFields\"\n      ]\n    },\n    \"paymentInstrument\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"accountHolderName\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"expiryMonth\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"expiryYear\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"last4\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"cardBrand\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"bankName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\
  \n        },\n        \"digitalWalletProvider\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"bankAccountHolderType\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankAccountType\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankAccountNumber\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"gatewayName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"processorName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"processorPaymentReference\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"gatewayReference\": {\n          \"type\": \"string\",\n \
  \         \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"accountHolderName\",\n        \"expiryMonth\",\n        \"expiryYear\",\n        \"last4\",\n        \"cardBrand\",\n        \"bankName\",\n        \"digitalWalletProvider\",\n        \"bankAccountHolderType\",\n        \"bankAccountType\",\n        \"bankAccountNumber\",\n        \"bankCode\",\n        \"gatewayName\",\n        \"processorName\",\n        \"processorPaymentReference\",\n        \"gatewayReference\"\n      ]\n    },\n    \"giftCommitmentCustomFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fieldValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n     \
  \   },\n        \"required\": [\n          \"fieldName\",\n          \"fieldValue\"\n        ]\n      }\n    },\n    \"giftCommitmentScheduleCustomFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fieldName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"fieldValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"fieldName\",\n          \"fieldValue\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"transactionPeriod\",\n    \"transactionInterval\",\n    \"transactionDay\",\n    \"startDate\",\n    \"endDate\",\n    \"campaign\",\n    \"outreachSourceCode\",\n    \"donor\",\n    \"paymentInstrument\",\n    \"giftCommitmentCustomFields\",\n    \"giftCommitmentScheduleCustomFields\"\
  \n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateCommitmentsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-update-commitments-request-schema.json
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
title: UpdateCommitmentsRequest
---
