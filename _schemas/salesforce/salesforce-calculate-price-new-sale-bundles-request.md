---
description: ''
layout: schema
name: CalculatePriceNewSaleBundlesRequest
properties_list:
- description: ''
  name: listPricebookId
  type: string
- description: ''
  name: candidatePricebookIds
  type: array
- description: ''
  name: pricingFlow
  type: string
- description: ''
  name: graph
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-calculate-price-new-sale-bundles-request-schema.json
slug: salesforce-calculate-price-new-sale-bundles-request
source_filename: salesforce-calculate-price-new-sale-bundles-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"listPricebookId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"candidatePricebookIds\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pricingFlow\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"graph\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"graphId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"records\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"referenceId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"record\": {\n               \
  \ \"type\": \"object\",\n                \"properties\": {\n                  \"attributes\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"type\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"type\"\n                    ]\n                  },\n                  \"CurrencyIsoCode\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"SalesTransactionShapeId\": {\n                    \"type\": \"string\",\n                    \"example\": \"500123\"\n                  },\n                  \"StartDate\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"ProductId\": {\n                    \"type\": \"string\",\n                    \"example\"\
  : \"500123\"\n                  },\n                  \"ProductSellingModelId\": {\n                    \"type\": \"string\",\n                    \"example\": \"500123\"\n                  },\n                  \"Quantity\": {\n                    \"type\": \"number\",\n                    \"example\": 42.5\n                  },\n                  \"PricingTransactionType\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"MainSalesTrxnItemShapeId\": {\n                    \"type\": \"string\",\n                    \"example\": \"500123\"\n                  },\n                  \"AssocSalesTrxnItemShapeId\": {\n                    \"type\": \"string\",\n                    \"example\": \"500123\"\n                  },\n                  \"MainSalesTrxnItemShapeRole\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n       \
  \           \"AssocSalesTrxnItemShapeRole\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"AssociatedItemShapePricing\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"attributes\"\n                ]\n              }\n            },\n            \"required\": [\n              \"referenceId\",\n              \"record\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"graphId\",\n        \"records\"\n      ]\n    }\n  },\n  \"required\": [\n    \"listPricebookId\",\n    \"candidatePricebookIds\",\n    \"pricingFlow\",\n    \"graph\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CalculatePriceNewSaleBundlesRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-calculate-price-new-sale-bundles-request-schema.json
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
title: CalculatePriceNewSaleBundlesRequest
---
