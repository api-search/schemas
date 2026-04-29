---
description: Schema for a portfolio entity in the SimCorp Integration Model (SIM). Portfolios represent investment portfolios managed within SimCorp Dimension, supporting multi-asset class holdings across the Investment Book of Record (IBOR). Based on the SimCorp Dimension data model documented at thesim.dev and simcorp.com.
layout: schema
name: SimCorp Dimension Portfolio
properties_list:
- description: Unique internal identifier for the portfolio within SimCorp Dimension
  name: portfolioId
  type: integer
- description: Short alphanumeric code uniquely identifying the portfolio
  name: portfolioCode
  type: string
- description: Full descriptive name of the portfolio
  name: portfolioName
  type: string
- description: Classification of the portfolio by its operational role
  name: portfolioType
  type: string
- description: Current lifecycle status of the portfolio
  name: portfolioStatus
  type: string
- description: ISO 4217 currency code for the portfolio base currency used for valuation and reporting
  name: baseCurrency
  type: string
- description: Date the portfolio was established and began tracking positions
  name: inceptionDate
  type: string
- description: Date the portfolio was closed or terminated, null if still active
  name: terminationDate
  type:
  - string
  - 'null'
- description: The legal entity or organization that owns the portfolio
  name: legalEntity
  type: string
- description: Name or identifier of the portfolio manager or management team responsible
  name: investmentManager
  type: string
- description: The custodian bank or institution holding the portfolio assets
  name: custodian
  type: string
- description: The benchmark portfolio or index used for performance comparison
  name: benchmark
  type: object
- description: Description of the investment strategy or mandate governing the portfolio
  name: investmentStrategy
  type: string
- description: Asset classes that the portfolio is authorized to hold
  name: assetClasses
  type: array
- description: Hierarchical structure placing this portfolio within a portfolio tree or organizational grouping
  name: portfolioHierarchy
  type: object
- description: Current holdings or positions within the portfolio from the Investment Book of Record (IBOR)
  name: positions
  type: array
- description: Investment compliance rules and constraints applied to the portfolio
  name: complianceRules
  type: array
- description: Summary valuation data for the portfolio as of the last valuation date
  name: valuationSummary
  type: object
- description: The accounting method used for the portfolio in the Accounting Book of Record (ABOR)
  name: accountingMethod
  type: string
- description: Currency used for client reporting if different from base currency
  name: reportingCurrency
  type: string
- description: User-defined and system classification attributes for the portfolio
  name: classifications
  type: object
- description: User-defined custom fields extending the standard portfolio attributes
  name: customProperties
  type: object
- description: Timestamp when the portfolio record was created in SimCorp Dimension
  name: createdDate
  type: string
- description: Timestamp when the portfolio record was last modified
  name: modifiedDate
  type: string
provider_name: SimCorp Dimension
provider_slug: simcorp-dimension
schema_file: json-schema/simcorp-dimension-portfolio-schema.json
slug: simcorp-dimension-portfolio
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://thesim.dev/schemas/simcorp-dimension/portfolio.json\",\n  \"title\": \"SimCorp Dimension Portfolio\",\n  \"description\": \"Schema for a portfolio entity in the SimCorp Integration Model (SIM). Portfolios represent investment portfolios managed within SimCorp Dimension, supporting multi-asset class holdings across the Investment Book of Record (IBOR). Based on the SimCorp Dimension data model documented at thesim.dev and simcorp.com.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"portfolioCode\",\n    \"portfolioName\"\n  ],\n  \"properties\": {\n    \"portfolioId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique internal identifier for the portfolio within SimCorp Dimension\"\n    },\n    \"portfolioCode\": {\n      \"type\": \"string\",\n      \"description\": \"Short alphanumeric code uniquely identifying the portfolio\",\n      \"maxLength\": 20\n    },\n \
  \   \"portfolioName\": {\n      \"type\": \"string\",\n      \"description\": \"Full descriptive name of the portfolio\",\n      \"maxLength\": 255\n    },\n    \"portfolioType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the portfolio by its operational role\",\n      \"enum\": [\n        \"REAL\",\n        \"MODEL\",\n        \"BENCHMARK\",\n        \"COMPOSITE\",\n        \"SLEEVE\",\n        \"MASTER\",\n        \"FUND\",\n        \"MANDATE\",\n        \"INTERNAL\"\n      ]\n    },\n    \"portfolioStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the portfolio\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"CLOSED\",\n        \"PENDING\",\n        \"SUSPENDED\",\n        \"TERMINATED\"\n      ]\n    },\n    \"baseCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the portfolio base currency used for valuation and reporting\",\n      \"pattern\": \"^[A-Z]{3}$\"\
  ,\n      \"examples\": [\"USD\", \"EUR\", \"GBP\", \"DKK\"]\n    },\n    \"inceptionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the portfolio was established and began tracking positions\"\n    },\n    \"terminationDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date the portfolio was closed or terminated, null if still active\"\n    },\n    \"legalEntity\": {\n      \"type\": \"string\",\n      \"description\": \"The legal entity or organization that owns the portfolio\",\n      \"maxLength\": 255\n    },\n    \"investmentManager\": {\n      \"type\": \"string\",\n      \"description\": \"Name or identifier of the portfolio manager or management team responsible\",\n      \"maxLength\": 255\n    },\n    \"custodian\": {\n      \"type\": \"string\",\n      \"description\": \"The custodian bank or institution holding the portfolio assets\",\n      \"maxLength\": 255\n    },\n\
  \    \"benchmark\": {\n      \"type\": \"object\",\n      \"description\": \"The benchmark portfolio or index used for performance comparison\",\n      \"properties\": {\n        \"benchmarkCode\": {\n          \"type\": \"string\",\n          \"description\": \"Code identifying the benchmark portfolio or index\"\n        },\n        \"benchmarkName\": {\n          \"type\": \"string\",\n          \"description\": \"Descriptive name of the benchmark\"\n        },\n        \"benchmarkType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of benchmark used\",\n          \"enum\": [\n            \"INDEX\",\n            \"PORTFOLIO\",\n            \"COMPOSITE\",\n            \"CUSTOM\",\n            \"BLENDED\"\n          ]\n        }\n      }\n    },\n    \"investmentStrategy\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the investment strategy or mandate governing the portfolio\",\n      \"maxLength\": 1000\n    },\n    \"assetClasses\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Asset classes that the portfolio is authorized to hold\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"EQUITY\",\n          \"FIXED_INCOME\",\n          \"MONEY_MARKET\",\n          \"DERIVATIVES\",\n          \"ALTERNATIVES\",\n          \"PRIVATE_EQUITY\",\n          \"REAL_ESTATE\",\n          \"COMMODITIES\",\n          \"FX\",\n          \"STRUCTURED_PRODUCTS\",\n          \"FUND\"\n        ]\n      }\n    },\n    \"portfolioHierarchy\": {\n      \"type\": \"object\",\n      \"description\": \"Hierarchical structure placing this portfolio within a portfolio tree or organizational grouping\",\n      \"properties\": {\n        \"parentPortfolioCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Code of the parent portfolio in a master-sleeve or composite structure\"\n        },\n        \"level\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Depth level within the portfolio hierarchy, where 0 is the top-level\",\n          \"minimum\": 0\n        },\n        \"groupCode\": {\n          \"type\": \"string\",\n          \"description\": \"Code identifying the portfolio group or organizational unit\"\n        },\n        \"groupName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the portfolio group\"\n        }\n      }\n    },\n    \"positions\": {\n      \"type\": \"array\",\n      \"description\": \"Current holdings or positions within the portfolio from the Investment Book of Record (IBOR)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Position\"\n      }\n    },\n    \"complianceRules\": {\n      \"type\": \"array\",\n      \"description\": \"Investment compliance rules and constraints applied to the portfolio\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ruleId\": {\n            \"type\": \"string\",\n            \"description\": \"Identifier\
  \ of the compliance rule\"\n          },\n          \"ruleName\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the compliance rule\"\n          },\n          \"ruleType\": {\n            \"type\": \"string\",\n            \"description\": \"Category of the compliance rule\",\n            \"enum\": [\n              \"PRE_TRADE\",\n              \"POST_TRADE\",\n              \"REGULATORY\",\n              \"INTERNAL\",\n              \"MANDATE\"\n            ]\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"Current compliance status\",\n            \"enum\": [\n              \"COMPLIANT\",\n              \"BREACH\",\n              \"WARNING\",\n              \"NOT_CHECKED\"\n            ]\n          }\n        }\n      }\n    },\n    \"valuationSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary valuation data for the portfolio as of the last valuation date\",\n      \"properties\"\
  : {\n        \"valuationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date of the most recent portfolio valuation\"\n        },\n        \"totalMarketValue\": {\n          \"type\": \"number\",\n          \"description\": \"Total market value of the portfolio in base currency\"\n        },\n        \"totalCostValue\": {\n          \"type\": \"number\",\n          \"description\": \"Total cost basis of the portfolio in base currency\"\n        },\n        \"cashBalance\": {\n          \"type\": \"number\",\n          \"description\": \"Total cash balance across all cash accounts in base currency\"\n        },\n        \"unrealizedGainLoss\": {\n          \"type\": \"number\",\n          \"description\": \"Total unrealized gain or loss in base currency\"\n        },\n        \"netAssetValue\": {\n          \"type\": \"number\",\n          \"description\": \"Net asset value (NAV) of the portfolio in base currency\"\n        }\n \
  \     }\n    },\n    \"accountingMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The accounting method used for the portfolio in the Accounting Book of Record (ABOR)\",\n      \"enum\": [\n        \"AVERAGE_COST\",\n        \"FIFO\",\n        \"LIFO\",\n        \"SPECIFIC_LOT\",\n        \"HIGHEST_COST\",\n        \"LOWEST_COST\"\n      ]\n    },\n    \"reportingCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency used for client reporting if different from base currency\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"classifications\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined and system classification attributes for the portfolio\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"customProperties\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined custom fields extending the standard portfolio attributes\",\n      \"additionalProperties\": true\n\
  \    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the portfolio record was created in SimCorp Dimension\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the portfolio record was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"Position\": {\n      \"$id\": \"#Position\",\n      \"title\": \"Portfolio Position\",\n      \"description\": \"A holding or position within a SimCorp Dimension portfolio, representing a quantity of an instrument held at a given status level within the IBOR.\",\n      \"type\": \"object\",\n      \"required\": [\n        \"instrumentCode\",\n        \"quantity\"\n      ],\n      \"properties\": {\n        \"positionId\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier for the position record\"\n        },\n        \"instrumentCode\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Code identifying the instrument held in this position\"\n        },\n        \"instrumentName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the instrument held\"\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"description\": \"Number of units, shares, or nominal amount held\"\n        },\n        \"settlementQuantity\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity at the settled position level\"\n        },\n        \"marketValue\": {\n          \"type\": \"number\",\n          \"description\": \"Current market value of the position in portfolio base currency\"\n        },\n        \"costValue\": {\n          \"type\": \"number\",\n          \"description\": \"Cost basis of the position in portfolio base currency\"\n        },\n        \"accruedInterest\": {\n          \"type\": \"number\",\n          \"description\": \"Accrued interest for fixed income\
  \ positions\"\n        },\n        \"unrealizedGainLoss\": {\n          \"type\": \"number\",\n          \"description\": \"Unrealized profit or loss on the position\"\n        },\n        \"weight\": {\n          \"type\": \"number\",\n          \"description\": \"Position weight as a percentage of total portfolio market value\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"positionDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date for which the position is reported\"\n        },\n        \"statusLevel\": {\n          \"type\": \"string\",\n          \"description\": \"Transaction status level defining the position view, reflecting the front-to-back lifecycle stage\",\n          \"enum\": [\n            \"ENTRY\",\n            \"TEMPORARILY_BOOKED\",\n            \"FINALLY_BOOKED\",\n            \"SETTLED\",\n            \"CONFIRMED\"\n          ]\n        },\n        \"positionCurrency\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code of the position\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"exchangeRate\": {\n          \"type\": \"number\",\n          \"description\": \"Exchange rate applied to convert from position currency to portfolio base currency\"\n        }\n      }\n    },\n\n    \"TransactionStatusLevel\": {\n      \"$id\": \"#TransactionStatusLevel\",\n      \"title\": \"Transaction Status Level\",\n      \"description\": \"Defines the status levels through which a transaction progresses in SimCorp Dimension, from entry through to final settlement. These status levels serve as position drivers.\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENTRY\",\n        \"TEMPORARILY_BOOKED\",\n        \"FINALLY_BOOKED\",\n        \"SETTLED\",\n        \"CONFIRMED\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/simcorp-dimension/refs/heads/main/json-schema/simcorp-dimension-portfolio-schema.json
tags:
- Accounting
- Asset Management
- Compliance
- Data Distribution
- Enterprise Software
- Financial Data
- Financial Technology
- Investment Management
- Portfolio Management
- Risk Management
- SimCorp One
- Streaming
- Trading
title: SimCorp Dimension Portfolio
---
