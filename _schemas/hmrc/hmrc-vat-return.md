---
description: JSON Schema for an HMRC Making Tax Digital VAT return submission. Contains the nine VAT return boxes as defined by HMRC for quarterly/monthly VAT accounting periods.
layout: schema
name: HMRC VAT Return
properties_list:
- description: The period key identifying the VAT obligation (e.g., '23AA' for a specific quarter)
  name: periodKey
  type: string
- description: Box 1 – VAT due on sales and other outputs. Must be >= 0.
  name: vatDueSales
  type: number
- description: Box 2 – VAT due on acquisitions of goods and services from EC member states. Must be >= 0.
  name: vatDueAcquisitions
  type: number
- description: Box 3 – Total VAT due (sum of Box 1 and Box 2). Must equal vatDueSales + vatDueAcquisitions.
  name: totalVatDue
  type: number
- description: Box 4 – VAT reclaimed in the period on purchases and other inputs (including EC acquisitions). Must be >= 0.
  name: vatReclaimedCurrPeriod
  type: number
- description: Box 5 – Net VAT to be paid to HMRC or reclaimed (absolute difference between Box 3 and Box 4). Must be >= 0.
  name: netVatDue
  type: number
- description: Box 6 – Total value of sales and all other outputs excluding VAT. Round to nearest pound.
  name: totalValueSalesExVAT
  type: number
- description: Box 7 – Total value of purchases and all other inputs excluding VAT. Round to nearest pound.
  name: totalValuePurchasesExVAT
  type: number
- description: Box 8 – Total value of all supplies of goods and related costs, excluding VAT, to EC member states.
  name: totalValueGoodsSuppliedExVAT
  type: number
- description: Box 9 – Total value of all acquisitions of goods and related costs, excluding VAT, from EC member states.
  name: totalAcquisitionsExVAT
  type: number
- description: Declaration that this is the final VAT return for the period. Must be true for accepted submissions.
  name: finalised
  type: boolean
provider_name: HMRC UK Tax Authority
provider_slug: hmrc
schema_file: json-schema/hmrc-vat-return-schema.json
slug: hmrc-vat-return
source_filename: hmrc-vat-return-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/hmrc/json-schema/hmrc-vat-return-schema.json\",\n  \"title\": \"HMRC VAT Return\",\n  \"description\": \"JSON Schema for an HMRC Making Tax Digital VAT return submission. Contains the nine VAT return boxes as defined by HMRC for quarterly/monthly VAT accounting periods.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"periodKey\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{2}[A-Z]{2}$\",\n      \"description\": \"The period key identifying the VAT obligation (e.g., '23AA' for a specific quarter)\"\n    },\n    \"vatDueSales\": {\n      \"type\": \"number\",\n      \"description\": \"Box 1 – VAT due on sales and other outputs. Must be >= 0.\",\n      \"minimum\": 0\n    },\n    \"vatDueAcquisitions\": {\n      \"type\": \"number\",\n      \"description\": \"Box 2 – VAT due on acquisitions of goods and services from EC member states. Must\
  \ be >= 0.\",\n      \"minimum\": 0\n    },\n    \"totalVatDue\": {\n      \"type\": \"number\",\n      \"description\": \"Box 3 – Total VAT due (sum of Box 1 and Box 2). Must equal vatDueSales + vatDueAcquisitions.\",\n      \"minimum\": 0\n    },\n    \"vatReclaimedCurrPeriod\": {\n      \"type\": \"number\",\n      \"description\": \"Box 4 – VAT reclaimed in the period on purchases and other inputs (including EC acquisitions). Must be >= 0.\",\n      \"minimum\": 0\n    },\n    \"netVatDue\": {\n      \"type\": \"number\",\n      \"description\": \"Box 5 – Net VAT to be paid to HMRC or reclaimed (absolute difference between Box 3 and Box 4). Must be >= 0.\",\n      \"minimum\": 0\n    },\n    \"totalValueSalesExVAT\": {\n      \"type\": \"number\",\n      \"description\": \"Box 6 – Total value of sales and all other outputs excluding VAT. Round to nearest pound.\",\n      \"minimum\": 0\n    },\n    \"totalValuePurchasesExVAT\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Box 7 – Total value of purchases and all other inputs excluding VAT. Round to nearest pound.\",\n      \"minimum\": 0\n    },\n    \"totalValueGoodsSuppliedExVAT\": {\n      \"type\": \"number\",\n      \"description\": \"Box 8 – Total value of all supplies of goods and related costs, excluding VAT, to EC member states.\",\n      \"minimum\": 0\n    },\n    \"totalAcquisitionsExVAT\": {\n      \"type\": \"number\",\n      \"description\": \"Box 9 – Total value of all acquisitions of goods and related costs, excluding VAT, from EC member states.\",\n      \"minimum\": 0\n    },\n    \"finalised\": {\n      \"type\": \"boolean\",\n      \"description\": \"Declaration that this is the final VAT return for the period. Must be true for accepted submissions.\",\n      \"const\": true\n    }\n  },\n  \"required\": [\n    \"periodKey\",\n    \"vatDueSales\",\n    \"vatDueAcquisitions\",\n    \"totalVatDue\",\n    \"vatReclaimedCurrPeriod\",\n    \"netVatDue\",\n    \"totalValueSalesExVAT\"\
  ,\n    \"totalValuePurchasesExVAT\",\n    \"totalValueGoodsSuppliedExVAT\",\n    \"totalAcquisitionsExVAT\",\n    \"finalised\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hmrc/refs/heads/main/json-schema/hmrc-vat-return-schema.json
tags:
- Government
- Making Tax Digital
- Regulatory
- Tax
- UK
title: HMRC VAT Return
---
