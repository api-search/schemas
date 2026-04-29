---
description: A financial security as represented in the Bloomberg BLPAPI data universe. Bloomberg tracks over 35 million instruments across equities, fixed income, derivatives, commodities, currencies, and alternative assets through services including //blp/refdata, //blp/mktdata, and //blp/mktbar. Securities are identified using Bloomberg tickers, FIGI, ISIN, CUSIP, SEDOL, and Bloomberg Unique Identifiers (BBUID). Based on bloomberg.github.io/blpapi-docs.
layout: schema
name: Bloomberg Security
properties_list:
- description: Bloomberg Unique Identifier (BBUID) - the primary internal Bloomberg security identifier.
  name: bbuid
  type: string
- description: Financial Instrument Global Identifier (FIGI) assigned by Bloomberg as the open, standard global identifier.
  name: figi
  type: string
- description: Bloomberg ticker symbol including asset class suffix used in BLPAPI requests (e.g., AAPL US Equity, CL1 Comdty, SPX Index, JPY Curncy).
  name: ticker
  type: string
- description: International Securities Identification Number (ISIN) for cross-border security identification.
  name: isin
  type: string
- description: Committee on Uniform Securities Identification Procedures (CUSIP) identifier, used primarily for US and Canadian securities.
  name: cusip
  type: string
- description: Stock Exchange Daily Official List (SEDOL) identifier. BLPAPI supports symbology lookup via /sedol1/ prefix (e.g., /sedol1/2840215).
  name: sedol
  type: string
- description: 'Full legal name of the security or issuer (BLPAPI field: Security_Name or NAME).'
  name: name
  type: string
- description: 'Abbreviated name of the security as displayed on Bloomberg Terminal (BLPAPI field: SHORT_NAME).'
  name: shortName
  type: string
- description: 'Extended company or instrument description (BLPAPI field: LONG_COMP_NAME).'
  name: longCompanyName
  type: string
- description: 'Bloomberg security description providing concise instrument details (BLPAPI field: SECURITY_DES).'
  name: securityDescription
  type: string
- description: Bloomberg security type classification determining which market data fields and services are available.
  name: securityType
  type: string
- description: 'Primary exchange where the security is listed, using Bloomberg exchange codes (BLPAPI field: EXCH_CODE).'
  name: exchange
  type: string
- description: 'ISO 4217 three-letter currency code for the security''s primary trading currency (BLPAPI field: CRNCY).'
  name: currency
  type: string
- description: 'ISO 3166-1 alpha-2 country code of the security''s country of domicile (BLPAPI field: COUNTRY_ISO).'
  name: country
  type: string
- description: 'GICS sector classification for the security (BLPAPI field: GICS_SECTOR_NAME).'
  name: sector
  type: string
- description: 'GICS industry group classification (BLPAPI field: GICS_INDUSTRY_GROUP_NAME).'
  name: industryGroup
  type: string
- description: 'Bloomberg Industry Classification Standard (BICS) industry code (BLPAPI field: INDUSTRY_GROUP).'
  name: industry
  type: string
- description: 'GICS sub-industry classification (BLPAPI field: GICS_SUB_INDUSTRY_NAME).'
  name: subIndustry
  type: string
- description: 'Market capitalization in the security''s primary trading currency (BLPAPI field: MARKET_CAP or CUR_MKT_CAP).'
  name: marketCap
  type: number
- description: 'Total number of shares currently outstanding (BLPAPI field: EQY_SH_OUT).'
  name: sharesOutstanding
  type: number
- description: ''
  name: pricing
  type: object
- description: ''
  name: fundamentals
  type: object
- description: ''
  name: referenceData
  type: object
- description: ''
  name: esgScores
  type: object
- description: 'Credit ratings from major rating agencies as reported via Bloomberg (BLPAPI fields: RTG_MOODY, RTG_SP, RTG_FITCH).'
  name: creditRatings
  type: array
- description: ''
  name: dividends
  type: object
- description: Whether the security is currently active and trading on its primary exchange.
  name: active
  type: boolean
provider_name: Bloomberg
provider_slug: bloomberg
schema_file: json-schema/bloomberg-security-schema.json
slug: bloomberg-security
source_filename: bloomberg-security-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bloomberg/refs/heads/main/json-schema/bloomberg-security-schema.json\",\n  \"title\": \"Bloomberg Security\",\n  \"description\": \"A financial security as represented in the Bloomberg BLPAPI data universe. Bloomberg tracks over 35 million instruments across equities, fixed income, derivatives, commodities, currencies, and alternative assets through services including //blp/refdata, //blp/mktdata, and //blp/mktbar. Securities are identified using Bloomberg tickers, FIGI, ISIN, CUSIP, SEDOL, and Bloomberg Unique Identifiers (BBUID). Based on bloomberg.github.io/blpapi-docs.\",\n  \"type\": \"object\",\n  \"required\": [\"ticker\", \"securityType\"],\n  \"properties\": {\n    \"bbuid\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg Unique Identifier (BBUID) - the primary internal Bloomberg security identifier.\"\n    },\n    \"\
  figi\": {\n      \"type\": \"string\",\n      \"description\": \"Financial Instrument Global Identifier (FIGI) assigned by Bloomberg as the open, standard global identifier.\",\n      \"pattern\": \"^[A-Z]{2}[0-9A-Z]{10}$\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg ticker symbol including asset class suffix used in BLPAPI requests (e.g., AAPL US Equity, CL1 Comdty, SPX Index, JPY Curncy).\"\n    },\n    \"isin\": {\n      \"type\": \"string\",\n      \"description\": \"International Securities Identification Number (ISIN) for cross-border security identification.\",\n      \"pattern\": \"^[A-Z]{2}[0-9A-Z]{10}$\"\n    },\n    \"cusip\": {\n      \"type\": \"string\",\n      \"description\": \"Committee on Uniform Securities Identification Procedures (CUSIP) identifier, used primarily for US and Canadian securities.\",\n      \"pattern\": \"^[0-9A-Z]{9}$\"\n    },\n    \"sedol\": {\n      \"type\": \"string\",\n      \"description\": \"Stock\
  \ Exchange Daily Official List (SEDOL) identifier. BLPAPI supports symbology lookup via /sedol1/ prefix (e.g., /sedol1/2840215).\",\n      \"pattern\": \"^[0-9B-DF-HJ-NP-TV-Z]{7}$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full legal name of the security or issuer (BLPAPI field: Security_Name or NAME).\"\n    },\n    \"shortName\": {\n      \"type\": \"string\",\n      \"description\": \"Abbreviated name of the security as displayed on Bloomberg Terminal (BLPAPI field: SHORT_NAME).\"\n    },\n    \"longCompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"Extended company or instrument description (BLPAPI field: LONG_COMP_NAME).\"\n    },\n    \"securityDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg security description providing concise instrument details (BLPAPI field: SECURITY_DES).\"\n    },\n    \"securityType\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg security type\
  \ classification determining which market data fields and services are available.\",\n      \"enum\": [\n        \"Equity\",\n        \"Corp\",\n        \"Govt\",\n        \"Mtge\",\n        \"M-Mkt\",\n        \"Muni\",\n        \"Pfd\",\n        \"Comdty\",\n        \"Index\",\n        \"Curncy\",\n        \"Equity Option\",\n        \"Fut\",\n        \"FX Option\"\n      ]\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Primary exchange where the security is listed, using Bloomberg exchange codes (BLPAPI field: EXCH_CODE).\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code for the security's primary trading currency (BLPAPI field: CRNCY).\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code of the security's country of domicile (BLPAPI field: COUNTRY_ISO).\",\n      \"pattern\":\
  \ \"^[A-Z]{2}$\"\n    },\n    \"sector\": {\n      \"type\": \"string\",\n      \"description\": \"GICS sector classification for the security (BLPAPI field: GICS_SECTOR_NAME).\"\n    },\n    \"industryGroup\": {\n      \"type\": \"string\",\n      \"description\": \"GICS industry group classification (BLPAPI field: GICS_INDUSTRY_GROUP_NAME).\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg Industry Classification Standard (BICS) industry code (BLPAPI field: INDUSTRY_GROUP).\"\n    },\n    \"subIndustry\": {\n      \"type\": \"string\",\n      \"description\": \"GICS sub-industry classification (BLPAPI field: GICS_SUB_INDUSTRY_NAME).\"\n    },\n    \"marketCap\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"minimum\": 0,\n      \"description\": \"Market capitalization in the security's primary trading currency (BLPAPI field: MARKET_CAP or CUR_MKT_CAP).\"\n    },\n    \"sharesOutstanding\": {\n      \"type\": \"number\"\
  ,\n      \"format\": \"double\",\n      \"minimum\": 0,\n      \"description\": \"Total number of shares currently outstanding (BLPAPI field: EQY_SH_OUT).\"\n    },\n    \"pricing\": {\n      \"$ref\": \"#/$defs/PricingSnapshot\"\n    },\n    \"fundamentals\": {\n      \"$ref\": \"#/$defs/Fundamentals\"\n    },\n    \"referenceData\": {\n      \"$ref\": \"#/$defs/ReferenceData\"\n    },\n    \"esgScores\": {\n      \"$ref\": \"#/$defs/EsgScores\"\n    },\n    \"creditRatings\": {\n      \"type\": \"array\",\n      \"description\": \"Credit ratings from major rating agencies as reported via Bloomberg (BLPAPI fields: RTG_MOODY, RTG_SP, RTG_FITCH).\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CreditRating\"\n      }\n    },\n    \"dividends\": {\n      \"$ref\": \"#/$defs/DividendData\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the security is currently active and trading on its primary exchange.\"\n    }\n  },\n  \"$defs\": {\n    \"\
  PricingSnapshot\": {\n      \"type\": \"object\",\n      \"description\": \"Current and recent pricing data for a Bloomberg security, corresponding to fields available via the //blp/mktdata subscription service and //blp/refdata ReferenceDataRequest.\",\n      \"properties\": {\n        \"lastPrice\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Most recent trade price (BLPAPI field: PX_LAST or LAST_PRICE for subscriptions).\"\n        },\n        \"bidPrice\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Current best bid price (BLPAPI field: PX_BID for requests, BID for subscriptions).\"\n        },\n        \"askPrice\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Current best ask price (BLPAPI field: PX_ASK for requests, ASK for subscriptions).\"\n        },\n        \"midPrice\": {\n          \"type\": \"number\",\n  \
  \        \"format\": \"double\",\n          \"description\": \"Mid-point of the last bid and last offer (BLPAPI field: PX_MID).\"\n        },\n        \"openPrice\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Opening price for the current trading session (BLPAPI field: PX_OPEN or OPEN for subscriptions).\"\n        },\n        \"highPrice\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Intraday high price for the current session (BLPAPI field: PX_HIGH or HIGH for subscriptions).\"\n        },\n        \"lowPrice\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Intraday low price for the current session (BLPAPI field: PX_LOW or LOW for subscriptions).\"\n        },\n        \"volume\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"minimum\": 0,\n          \"description\": \"Total trading\
  \ volume for the current session (BLPAPI field: VOLUME).\"\n        },\n        \"vwap\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Volume-weighted average price for the current session (BLPAPI field: EQY_WEIGHTED_AVG_PX, available via //blp/mktvwap).\"\n        },\n        \"previousClose\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Previous trading session close price (BLPAPI field: PX_LAST for prior session).\"\n        },\n        \"priceChange\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Absolute price change from previous close (BLPAPI field: NET_CHG).\"\n        },\n        \"priceChangePct\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Percentage price change from previous close (BLPAPI field: CHG_PCT_1D).\"\n        },\n        \"fiftyTwoWeekHigh\": {\n\
  \          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Highest price over the trailing 52-week period (BLPAPI field: HIGH_52WEEK).\"\n        },\n        \"fiftyTwoWeekLow\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Lowest price over the trailing 52-week period (BLPAPI field: LOW_52WEEK).\"\n        },\n        \"asOf\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when pricing data was last updated.\"\n        }\n      }\n    },\n    \"Fundamentals\": {\n      \"type\": \"object\",\n      \"description\": \"Key fundamental financial data available via BLPAPI ReferenceDataRequest.\",\n      \"properties\": {\n        \"earningsPerShare\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Annualized earnings per share (BLPAPI field: EPS_ANNUALIZED or IS_EPS).\"\n\
  \        },\n        \"priceToEarnings\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Price-to-earnings ratio (BLPAPI field: PE_RATIO).\"\n        },\n        \"priceToBook\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Price-to-book value ratio (BLPAPI field: PX_TO_BOOK_RATIO).\"\n        },\n        \"returnOnEquity\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Return on equity as a percentage (BLPAPI field: RETURN_COM_EQY).\"\n        },\n        \"debtToEquity\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Total debt to common equity ratio (BLPAPI field: TOT_DEBT_TO_COM_EQY).\"\n        },\n        \"revenuePerShare\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Revenue per share (BLPAPI field: SALES_REV_TURN).\"\
  \n        },\n        \"dividendYield\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Indicated dividend yield as a percentage (BLPAPI field: EQY_DVD_YLD_IND).\"\n        },\n        \"beta\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Beta relative to the benchmark index (BLPAPI field: BETA_RAW_OVERRIDABLE).\"\n        },\n        \"fiscalYearEnd\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Most recent fiscal year end date.\"\n        }\n      }\n    },\n    \"ReferenceData\": {\n      \"type\": \"object\",\n      \"description\": \"Descriptive and reference data for a Bloomberg security, retrieved via //blp/refdata ReferenceDataRequest.\",\n      \"properties\": {\n        \"businessDescription\": {\n          \"type\": \"string\",\n          \"description\": \"Business description of the issuing company (BLPAPI field:\
  \ CIE_DES_BULK or BUSINESS_DESCRIPTION).\"\n        },\n        \"numberOfEmployees\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total number of employees reported by the company (BLPAPI field: NUM_OF_EMPLOYEES).\"\n        },\n        \"yearFounded\": {\n          \"type\": \"integer\",\n          \"minimum\": 1000,\n          \"maximum\": 9999,\n          \"description\": \"Year the company was founded (BLPAPI field: YEAR_FOUNDED).\"\n        },\n        \"headquarters\": {\n          \"type\": \"string\",\n          \"description\": \"City and country where the company is headquartered.\"\n        },\n        \"website\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Company website URL (BLPAPI field: COMPANY_WEB_ADDRESS).\"\n        },\n        \"ceo\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the Chief Executive Officer.\"\n        },\n        \"bloombergIndustryGroup\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg Industry Classification Standard (BICS) industry group.\"\n        },\n        \"bloombergSubIndustry\": {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg Industry Classification Standard (BICS) sub-industry.\"\n        },\n        \"companyAddress\": {\n          \"type\": \"array\",\n          \"description\": \"Company address lines returned as a bulk field (BLPAPI bulk field: COMPANY_ADDRESS).\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"lei\": {\n          \"type\": \"string\",\n          \"description\": \"Legal Entity Identifier (LEI) of the issuing entity.\",\n          \"pattern\": \"^[A-Z0-9]{18}[0-9]{2}$\"\n        }\n      }\n    },\n    \"EsgScores\": {\n      \"type\": \"object\",\n      \"description\": \"Bloomberg ESG scores for the security's issuer, available through Bloomberg Data License and BLPAPI reference data.\"\
  ,\n      \"properties\": {\n        \"overallScore\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"Overall Bloomberg ESG score on a 0-100 scale.\"\n        },\n        \"environmentalScore\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"Environmental pillar score on a 0-100 scale.\"\n        },\n        \"socialScore\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"Social pillar score on a 0-100 scale.\"\n        },\n        \"governanceScore\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"Governance pillar score on a 0-100 scale.\"\n        },\n    \
  \    \"disclosureScore\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"ESG disclosure quality score reflecting completeness of reported data.\"\n        },\n        \"asOfDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date for which the ESG scores are reported.\"\n        }\n      }\n    },\n    \"CreditRating\": {\n      \"type\": \"object\",\n      \"description\": \"A credit rating issued by a major rating agency for the security, as reported via BLPAPI reference data fields.\",\n      \"required\": [\"agency\", \"rating\"],\n      \"properties\": {\n        \"agency\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the credit rating agency.\",\n          \"enum\": [\"Moody's\", \"S&P\", \"Fitch\", \"DBRS\", \"Kroll\", \"AM Best\"]\n        },\n        \"rating\": {\n          \"type\": \"\
  string\",\n          \"description\": \"Credit rating symbol (e.g., AAA, Aaa, BB+). BLPAPI fields: RTG_MOODY, RTG_SP, RTG_FITCH.\"\n        },\n        \"outlook\": {\n          \"type\": \"string\",\n          \"description\": \"Rating outlook indicating potential direction of future rating changes.\",\n          \"enum\": [\"Positive\", \"Stable\", \"Negative\", \"Watch Positive\", \"Watch Negative\", \"Review\"]\n        },\n        \"ratedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date the credit rating was assigned or most recently affirmed.\"\n        },\n        \"ratingType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of rating scope.\",\n          \"enum\": [\"long-term\", \"short-term\"]\n        }\n      }\n    },\n    \"DividendData\": {\n      \"type\": \"object\",\n      \"description\": \"Dividend information for the security, available via BLPAPI reference data.\",\n      \"properties\"\
  : {\n        \"indicatedAnnualDividend\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": 0,\n          \"description\": \"Indicated annual dividend amount per share (BLPAPI field: EQY_DVD_YLD_IND).\"\n        },\n        \"dividendFrequency\": {\n          \"type\": \"string\",\n          \"description\": \"Frequency of dividend payments (BLPAPI field: DVD_FREQ).\",\n          \"enum\": [\"Annual\", \"Semi-Annual\", \"Quarterly\", \"Monthly\", \"Irregular\", \"None\"]\n        },\n        \"exDividendDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Next or most recent ex-dividend date (BLPAPI field: DVD_EX_DT).\"\n        },\n        \"dividendPayDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Next or most recent dividend payment date (BLPAPI field: DVD_PAY_DT).\"\n        },\n        \"dividendAmount\": {\n          \"type\"\
  : \"number\",\n          \"format\": \"double\",\n          \"minimum\": 0,\n          \"description\": \"Most recent dividend amount per share (BLPAPI field: DVD_SH_LAST).\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg/refs/heads/main/json-schema/bloomberg-security-schema.json
tags:
- Analytics
- Business Intelligence
- Data License
- Enterprise
- Execution Management
- Financial Services
- Market Data
- News
- Quantitative Analysis
- Trading
- Transaction Cost Analysis
title: Bloomberg Security
---
