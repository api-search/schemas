---
description: ''
layout: schema
name: costsFees
properties_list:
- description: FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.
  name: fsymId
  type: string
- description: The management fee, or maintenance fee, is charged by the fund manager. This cost is usually between 0.5% and 2% of assets on average and is a periodic fee.
  name: managementExpenses
  type: number
- description: The Expense Date expressed in YYYY-MM-DD.
  name: date
  type: string
- description: ISO3 Currency
  name: currency
  type: string
- description: The transaction entry fee or purchase fee collected from investors when they join or leave a scheme. The fee is paid to the fund
  name: entryExpenses
  type: number
- description: The transaction exit fee is charged to investors when they redeem shares from a fund.
  name: exitExpenses
  type: number
- description: The Maximum sales load or initial Sales Fee is a reduction made from each investment in the fund, the maximum paid is dependent on the size of the purchase, it decreases as the investment increases. O
  name: frontExpensesMax
  type: number
- description: The Back Expense Maximum
  name: backExpensesMax
  type: number
- description: The Expense Ratio
  name: expenseRatio
  type: number
- description: The Expense Ratio Prospectus
  name: expenseRatioProspectus
  type: number
- description: The Initial Investment Minimum
  name: initInvestmentMin
  type: number
- description: The Initial Investment Individual Retirement Accounts
  name: initInvestmentIra
  type: number
- description: Swing Price. Swing pricing occurs when a fund provider adjusts the net asset value (NAV) of a fund in order to pass on trading costs to purchasing or redeeming shareholders. This anti-dilution techniq
  name: swingPrice
  type: number
- description: Swing Price Date. Swing pricing occurs when a fund provider adjusts the net asset value (NAV) of a fund in order to pass on trading costs to purchasing or redeeming shareholders. This anti-dilution te
  name: swingPriceDate
  type: string
- description: The SRI (Summary Risk Indicator) illustrates PRIIPs' risk and reward profile by measuring the market and credit risk level. Returns 1 for low risk up to 7 for higher risk.
  name: sriPriips
  type: integer
- description: Synthetic Risk and Reward Indicator illustrates a UCITS or NURS (Non-UCITS Retail Scheme) fund's risk and reward profile by measuring the market risk level. Returns 1 for low risk up to 7 for high ris
  name: srriUcits
  type: integer
- description: Represents fees made to an investment manager as a percentage of investment profits for generating positive returns.
  name: performanceFee
  type: number
- description: Represents the amount of trading commissions incurred to manage the portfolio as a percentage of the total assets of the fund.
  name: tradingExpenseRatio
  type: number
- description: The requested Id sent as input.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-costs-fees-schema.json
slug: factset-funds-costs-fees
source_filename: factset-funds-costs-fees-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"costsFees\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Security Identifier. Six alpha-numeric characters, excluding vowels, with a -S suffix (XXXXXX-S), resolved from the requestId of the Fund requested.\"\n    },\n    \"managementExpenses\": {\n      \"type\": \"number\",\n      \"description\": \"The management fee, or maintenance fee, is charged by the fund manager. This cost is usually between 0.5% and 2% of assets on average and is a periodic fee.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"The Expense Date expressed in YYYY-MM-DD.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO3 Currency\"\n    },\n    \"entryExpenses\": {\n      \"type\": \"number\",\n      \"description\": \"The transaction entry fee or purchase fee collected\
  \ from investors when they join or leave a scheme. The fee is paid to the fund\"\n    },\n    \"exitExpenses\": {\n      \"type\": \"number\",\n      \"description\": \"The transaction exit fee is charged to investors when they redeem shares from a fund.\"\n    },\n    \"frontExpensesMax\": {\n      \"type\": \"number\",\n      \"description\": \"The Maximum sales load or initial Sales Fee is a reduction made from each investment in the fund, the maximum paid is dependent on the size of the purchase, it decreases as the investment increases. Often associated with class 'A' shares of a mutual fund it is also known as Sales Charge, this is a fee paid when shares are purchased. Also known as a \\\"front-end load\\\", this fee typically goes to the brokers that sell the fund's shares.  (Under the Investment Company Act of 1940 is 9%. The maximum sales load under NASD Rules is 8 1/2%).\\\"\\n\"\n    },\n    \"backExpensesMax\": {\n      \"type\": \"number\",\n      \"description\": \"The Back\
  \ Expense Maximum\"\n    },\n    \"expenseRatio\": {\n      \"type\": \"number\",\n      \"description\": \"The Expense Ratio\"\n    },\n    \"expenseRatioProspectus\": {\n      \"type\": \"number\",\n      \"description\": \"The Expense Ratio Prospectus\"\n    },\n    \"initInvestmentMin\": {\n      \"type\": \"number\",\n      \"description\": \"The Initial Investment Minimum\"\n    },\n    \"initInvestmentIra\": {\n      \"type\": \"number\",\n      \"description\": \"The Initial Investment Individual Retirement Accounts\"\n    },\n    \"swingPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Swing Price. Swing pricing occurs when a fund provider adjusts the net asset value (NAV) of a fund in order to pass on trading costs to purchasing or redeeming shareholders. This anti-dilution technique is used to protect long-term shareholder's interests.\"\n    },\n    \"swingPriceDate\": {\n      \"type\": \"string\",\n      \"description\": \"Swing Price Date. Swing pricing occurs\
  \ when a fund provider adjusts the net asset value (NAV) of a fund in order to pass on trading costs to purchasing or redeeming shareholders. This anti-dilution technique is used to protect long-term shareholder's interests.\"\n    },\n    \"sriPriips\": {\n      \"type\": \"integer\",\n      \"description\": \"The SRI (Summary Risk Indicator) illustrates PRIIPs' risk and reward profile by measuring the market and credit risk level. Returns 1 for low risk up to 7 for higher risk.\"\n    },\n    \"srriUcits\": {\n      \"type\": \"integer\",\n      \"description\": \"Synthetic Risk and Reward Indicator illustrates a UCITS or NURS (Non-UCITS Retail Scheme) fund's risk and reward profile by measuring the market risk level. Returns 1 for low risk up to 7 for high risk.\"\n    },\n    \"performanceFee\": {\n      \"type\": \"number\",\n      \"description\": \"Represents fees made to an investment manager as a percentage of investment profits for generating positive returns.\"\n    },\n   \
  \ \"tradingExpenseRatio\": {\n      \"type\": \"number\",\n      \"description\": \"Represents the amount of trading commissions incurred to manage the portfolio as a percentage of the total assets of the fund.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Id sent as input.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-costs-fees-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: costsFees
---
