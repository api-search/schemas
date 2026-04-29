---
description: A financial security representing an instrument in Bloomberg's data universe, including equities, fixed income, derivatives, funds, and other asset classes with reference data, identifiers, and classification information.
layout: schema
name: Bloomberg Buyside Security
properties_list:
- description: Bloomberg ticker symbol (e.g., 'AAPL US Equity')
  name: ticker
  type: string
- description: Full security name
  name: name
  type: string
- description: Abbreviated security name
  name: shortName
  type: string
- description: Primary asset class classification
  name: assetClass
  type: string
- description: Specific security type within the asset class
  name: securityType
  type: string
- description: Primary exchange where the security is listed
  name: exchange
  type: string
- description: Country of domicile (ISO 3166-1 alpha-2)
  name: country
  type: string
- description: Trading currency (ISO 4217)
  name: currency
  type: string
- description: ''
  name: identifiers
  type: object
- description: ''
  name: classification
  type: object
- description: Issuer name
  name: issuer
  type: string
- description: Original issue date
  name: issueDate
  type: string
- description: Maturity date (for fixed income and derivatives)
  name: maturityDate
  type: string
- description: Coupon rate for fixed income securities
  name: couponRate
  type: number
- description: Coupon payment frequency
  name: couponFrequency
  type: string
- description: Par or face value
  name: parAmount
  type: number
- description: Market capitalization (for equities)
  name: marketCap
  type: number
- description: Total shares outstanding (for equities)
  name: sharesOutstanding
  type: number
- description: Indicated dividend yield
  name: dividendYield
  type: number
- description: ''
  name: rating
  type: object
- description: Whether the security is currently active and trading
  name: active
  type: boolean
provider_name: Bloomberg Buyside Enterprise Solutions
provider_slug: bloomberg-buyside-enterprise-solutions
schema_file: json-schema/bloomberg-buyside-security-schema.json
slug: bloomberg-buyside-security
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.bloomberg.com/schemas/buyside/security.json\",\n  \"title\": \"Bloomberg Buyside Security\",\n  \"description\": \"A financial security representing an instrument in Bloomberg's data universe, including equities, fixed income, derivatives, funds, and other asset classes with reference data, identifiers, and classification information.\",\n  \"type\": \"object\",\n  \"required\": [\"ticker\"],\n  \"properties\": {\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg ticker symbol (e.g., 'AAPL US Equity')\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full security name\"\n    },\n    \"shortName\": {\n      \"type\": \"string\",\n      \"description\": \"Abbreviated security name\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"enum\": [\"Equity\", \"Fixed Income\", \"Commodity\", \"Currency\", \"\
  Index\", \"Fund\", \"Mortgage\", \"Municipal\", \"Preferred\", \"Derivative\"],\n      \"description\": \"Primary asset class classification\"\n    },\n    \"securityType\": {\n      \"type\": \"string\",\n      \"description\": \"Specific security type within the asset class\"\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Primary exchange where the security is listed\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of domicile (ISO 3166-1 alpha-2)\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Trading currency (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"identifiers\": {\n      \"$ref\": \"#/$defs/SecurityIdentifiers\"\n    },\n    \"classification\": {\n      \"$ref\": \"#/$defs/SecurityClassification\"\n    },\n    \"issuer\": {\n      \"type\": \"string\",\n      \"description\": \"Issuer name\"\n    },\n   \
  \ \"issueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Original issue date\"\n    },\n    \"maturityDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Maturity date (for fixed income and derivatives)\"\n    },\n    \"couponRate\": {\n      \"type\": \"number\",\n      \"description\": \"Coupon rate for fixed income securities\"\n    },\n    \"couponFrequency\": {\n      \"type\": \"string\",\n      \"enum\": [\"ANNUAL\", \"SEMI_ANNUAL\", \"QUARTERLY\", \"MONTHLY\", \"ZERO\"],\n      \"description\": \"Coupon payment frequency\"\n    },\n    \"parAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Par or face value\"\n    },\n    \"marketCap\": {\n      \"type\": \"number\",\n      \"description\": \"Market capitalization (for equities)\"\n    },\n    \"sharesOutstanding\": {\n      \"type\": \"number\",\n      \"description\": \"Total shares outstanding (for equities)\"\n    },\n \
  \   \"dividendYield\": {\n      \"type\": \"number\",\n      \"description\": \"Indicated dividend yield\"\n    },\n    \"rating\": {\n      \"$ref\": \"#/$defs/CreditRating\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the security is currently active and trading\"\n    }\n  },\n  \"$defs\": {\n    \"SecurityIdentifiers\": {\n      \"type\": \"object\",\n      \"description\": \"Standard financial instrument identifiers\",\n      \"properties\": {\n        \"isin\": {\n          \"type\": \"string\",\n          \"description\": \"International Securities Identification Number\",\n          \"pattern\": \"^[A-Z]{2}[A-Z0-9]{9}[0-9]$\"\n        },\n        \"cusip\": {\n          \"type\": \"string\",\n          \"description\": \"Committee on Uniform Securities Identification Procedures number\",\n          \"pattern\": \"^[A-Z0-9]{9}$\"\n        },\n        \"sedol\": {\n          \"type\": \"string\",\n          \"description\": \"Stock Exchange\
  \ Daily Official List number\",\n          \"pattern\": \"^[A-Z0-9]{7}$\"\n        },\n        \"figi\": {\n          \"type\": \"string\",\n          \"description\": \"Financial Instrument Global Identifier\",\n          \"pattern\": \"^[A-Z]{3}[A-Z0-9]{9}$\"\n        },\n        \"lei\": {\n          \"type\": \"string\",\n          \"description\": \"Legal Entity Identifier of the issuer\",\n          \"pattern\": \"^[A-Z0-9]{20}$\"\n        },\n        \"bloombergId\": {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg unique identifier\"\n        }\n      }\n    },\n    \"SecurityClassification\": {\n      \"type\": \"object\",\n      \"description\": \"Industry and sector classification details\",\n      \"properties\": {\n        \"gicsSector\": {\n          \"type\": \"string\",\n          \"description\": \"GICS sector name\"\n        },\n        \"gicsIndustryGroup\": {\n          \"type\": \"string\",\n          \"description\": \"GICS industry group\
  \ name\"\n        },\n        \"gicsIndustry\": {\n          \"type\": \"string\",\n          \"description\": \"GICS industry name\"\n        },\n        \"gicsSubIndustry\": {\n          \"type\": \"string\",\n          \"description\": \"GICS sub-industry name\"\n        },\n        \"bicsLevel1\": {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg Industry Classification System level 1\"\n        },\n        \"bicsLevel2\": {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg Industry Classification System level 2\"\n        },\n        \"bicsLevel3\": {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg Industry Classification System level 3\"\n        }\n      }\n    },\n    \"CreditRating\": {\n      \"type\": \"object\",\n      \"description\": \"Credit ratings from major rating agencies\",\n      \"properties\": {\n        \"sp\": {\n          \"type\": \"string\",\n          \"description\": \"S&P Global credit\
  \ rating\"\n        },\n        \"moodys\": {\n          \"type\": \"string\",\n          \"description\": \"Moody's credit rating\"\n        },\n        \"fitch\": {\n          \"type\": \"string\",\n          \"description\": \"Fitch credit rating\"\n        },\n        \"compositeRating\": {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg composite credit rating\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-buyside-enterprise-solutions/refs/heads/main/json-schema/bloomberg-buyside-security-schema.json
tags:
- Analytics
- Asset Management
- Buy-Side
- Enterprise Solutions
- Financial Services
- Market Data
- Portfolio Management
- Trading
title: Bloomberg Buyside Security
---
