---
description: ''
layout: schema
name: PromotionsCreationRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: startDateTime
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: priorityNumber
  type: integer
- description: ''
  name: description
  type: string
- description: ''
  name: endDateTime
  type: string
- description: ''
  name: objective
  type: string
- description: ''
  name: loyaltyProgram
  type: object
- description: ''
  name: additionalFieldValues
  type: object
- description: ''
  name: promotionLimits
  type: object
- description: ''
  name: promotionEligibility
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-promotions-creation-request-schema.json
slug: salesforce-promotions-creation-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"priorityNumber\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A sample description.\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"objective\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"loyaltyProgram\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Example Title\"\n        }\n      },\n      \"required\": [\n        \"name\"\n  \
  \    ]\n    },\n    \"additionalFieldValues\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"promotionLocation__c\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"promotionLocation__c\"\n          ]\n        }\n      },\n      \"required\": [\n        \"attributes\"\n      ]\n    },\n    \"promotionLimits\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"perLineItemLimit\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"vouchersLimit\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"vouchersPerCustomerLimit\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"perCartLimit\": {\n          \"type\": \"integer\",\n          \"example\":\
  \ 10\n        },\n        \"usePerCustomerLimit\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"liabilityLimit\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"loyaltyProgramCurrency\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"id\"\n          ]\n        },\n        \"pointsPerCustomerLimit\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"perLineItemLimit\",\n        \"vouchersLimit\",\n        \"vouchersPerCustomerLimit\",\n        \"perCartLimit\",\n        \"usePerCustomerLimit\",\n        \"liabilityLimit\",\n        \"loyaltyProgramCurrency\",\n        \"pointsPerCustomerLimit\"\n      ]\n    },\n    \"promotionEligibility\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"eligibleProductCategories\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              }\n            },\n            \"required\": [\n              \"id\"\n            ]\n          }\n        },\n        \"eligibleProducts\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Example Title\"\n              }\n            },\n            \"required\": [\n              \"name\"\n            ]\n          }\n        },\n        \"eligibleChannels\": {\n          \"type\"\
  : \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"channelType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"store\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\": \"Example Title\"\n                  }\n                },\n                \"required\": [\n                  \"name\"\n                ]\n              },\n              \"retailLocationGroup\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\": \"Example Title\"\n                  }\n                },\n                \"required\": [\n           \
  \       \"name\"\n                ]\n              }\n            },\n            \"required\": [\n              \"channelType\",\n              \"store\",\n              \"retailLocationGroup\"\n            ]\n          }\n        },\n        \"eligibleCustomerEvents\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"event\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"eventPeriodUnit\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"event\",\n            \"eventPeriodUnit\"\n          ]\n        },\n        \"eligibleEnrollmentPeriod\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isEnrollmentRequired\": {\n              \"type\": \"boolean\",\n              \"example\": true\n            },\n            \"enrollmentStartDate\": {\n         \
  \     \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"enrollmentEndDate\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"isEnrollmentRequired\",\n            \"enrollmentStartDate\",\n            \"enrollmentEndDate\"\n          ]\n        },\n        \"eligibleLoyaltyTiers\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"tierGroup\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\": \"Example Title\"\n                  },\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"example\": \"abc123\"\n  \
  \                }\n                },\n                \"required\": [\n                  \"name\",\n                  \"id\"\n                ]\n              },\n              \"tier\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\": \"Example Title\"\n                  },\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"example\": \"abc123\"\n                  }\n                },\n                \"required\": [\n                  \"name\",\n                  \"id\"\n                ]\n              }\n            },\n            \"required\": [\n              \"tierGroup\",\n              \"tier\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"eligibleProductCategories\",\n        \"eligibleProducts\",\n        \"eligibleChannels\",\n        \"eligibleCustomerEvents\"\
  ,\n        \"eligibleEnrollmentPeriod\",\n        \"eligibleLoyaltyTiers\"\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"startDateTime\",\n    \"displayName\",\n    \"priorityNumber\",\n    \"description\",\n    \"endDateTime\",\n    \"objective\",\n    \"loyaltyProgram\",\n    \"additionalFieldValues\",\n    \"promotionLimits\",\n    \"promotionEligibility\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PromotionsCreationRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-promotions-creation-request-schema.json
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
title: PromotionsCreationRequest
---
