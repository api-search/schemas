---
description: ''
layout: schema
name: Data13
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: ticker
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: website
  type: string
- description: ''
  name: domainList
  type: array
- description: ''
  name: logo
  type: string
- description: ''
  name: socialMediaUrls
  type: array
- description: ''
  name: revenue
  type: integer
- description: ''
  name: employeeCount
  type: integer
- description: ''
  name: numberOfContactsInZoomInfo
  type: integer
- description: ''
  name: phone
  type: string
- description: ''
  name: fax
  type: string
- description: ''
  name: street
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: zipCode
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: continent
  type: string
- description: ''
  name: companyStatus
  type: string
- description: ''
  name: companyStatusDate
  type: string
- description: ''
  name: descriptionList
  type: array
- description: ''
  name: sicCodes
  type: array
- description: ''
  name: naicsCodes
  type: array
- description: ''
  name: competitors
  type: array
- description: ''
  name: ultimateParentId
  type: integer
- description: ''
  name: ultimateParentName
  type: string
- description: ''
  name: ultimateParentRevenue
  type: integer
- description: ''
  name: ultimateParentEmployees
  type: integer
- description: ''
  name: subUnitCodes
  type: array
- description: ''
  name: subUnitType
  type: string
- description: ''
  name: subUnitIndustries
  type: array
- description: ''
  name: primaryIndustry
  type: array
- description: ''
  name: industries
  type: array
- description: ''
  name: parentId
  type: integer
- description: ''
  name: parentName
  type: string
- description: ''
  name: locationCount
  type: integer
- description: ''
  name: alexaRank
  type: string
- description: ''
  name: metroArea
  type: string
- description: ''
  name: lastUpdatedDate
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: certificationDate
  type: string
- description: ''
  name: certified
  type: boolean
- description: ''
  name: hashtags
  type: array
- description: ''
  name: products
  type: array
- description: ''
  name: techAttributes
  type: array
- description: ''
  name: revenueRange
  type: string
- description: ''
  name: employeeRange
  type: string
- description: ''
  name: companyFunding
  type: array
- description: ''
  name: recentFundingAmount
  type: integer
- description: ''
  name: recentFundingDate
  type: string
- description: ''
  name: totalFundingAmount
  type: integer
- description: ''
  name: employeeGrowth
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data13-schema.json
slug: zoominfo-data13
source_filename: zoominfo-data13-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"domainList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"logo\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"socialMediaUrls\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"https://www.example.com\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n\
  \          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com/resource\"\n          },\n          \"followerCount\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"type\",\n          \"url\",\n          \"followerCount\"\n        ]\n      }\n    },\n    \"revenue\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"employeeCount\": {\n      \"type\": \"integer\",\n      \"example\": 250\n    },\n    \"numberOfContactsInZoomInfo\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+1-555-555-1234\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"city\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"San Francisco\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    },\n    \"continent\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"companyStatus\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"companyStatusDate\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"descriptionList\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          }\n        },\n        \"required\": [\n          \"description\"\n        ]\n      }\n\
  \    },\n    \"sicCodes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"name\"\n        ]\n      }\n    },\n    \"naicsCodes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"name\"\
  \n        ]\n      }\n    },\n    \"competitors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rank\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"id\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"website\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"employeeCount\": {\n            \"type\": \"integer\",\n            \"example\": 250\n          }\n        },\n        \"required\": [\n          \"rank\",\n          \"id\",\n          \"name\",\n          \"website\",\n          \"employeeCount\"\n        ]\n      }\n    },\n    \"ultimateParentId\": {\n      \"type\": \"integer\"\
  ,\n      \"example\": 500123\n    },\n    \"ultimateParentName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"ultimateParentRevenue\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"ultimateParentEmployees\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"subUnitCodes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"subUnitType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"subUnitIndustries\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"primaryIndustry\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"industries\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"parentId\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"parentName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"locationCount\": {\n      \"type\": \"integer\",\n      \"example\": 250\n    },\n    \"alexaRank\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"metroArea\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastUpdatedDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"certificationDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"certified\": {\n      \"type\": \"boolean\",\n      \"example\"\
  : true\n    },\n    \"hashtags\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tag\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"external_id\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"500123\"\n          },\n          \"searchString\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"displayLabel\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          },\n          \"group\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"score\": {\n            \"type\": \"['string',\
  \ 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"priority\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"parentCategory\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"displayScore\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"inverseScoreBase\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"scoreMultipler\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"scoreUnit\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"hidden\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"label\": {\n            \"type\": \"string\",\n     \
  \       \"example\": \"example_value\"\n          },\n          \"categorizedFlag\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"tag\",\n          \"external_id\",\n          \"searchString\",\n          \"displayLabel\",\n          \"description\",\n          \"group\",\n          \"score\",\n          \"priority\",\n          \"parentCategory\",\n          \"displayScore\",\n          \"inverseScoreBase\",\n          \"scoreMultipler\",\n          \"scoreUnit\",\n          \"hidden\",\n          \"label\",\n          \"categorizedFlag\"\n        ]\n      }\n    },\n    \"products\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"techAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n       \
  \ \"properties\": {\n          \"tag\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"categoryParent\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"vendor\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"product\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"attribute\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"website\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"logo\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"\
  domain\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"createdTime\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"modifiedTime\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          }\n        },\n        \"required\": [\n          \"tag\",\n          \"categoryParent\",\n          \"category\",\n          \"vendor\",\n          \"product\",\n          \"attribute\",\n          \"website\",\n          \"logo\",\n          \"domain\",\n          \"createdTime\",\n          \"modifiedTime\",\n          \"description\"\n        ]\n      }\n    },\n    \"revenueRange\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"employeeRange\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"companyFunding\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"date\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"amount\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          }\n        },\n        \"required\": [\n          \"date\",\n          \"type\",\n          \"amount\"\n        ]\n      }\n    },\n    \"recentFundingAmount\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"recentFundingDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"totalFundingAmount\": {\n      \"type\": \"integer\",\n\
  \      \"example\": 100\n    },\n    \"employeeGrowth\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"oneYearGrowthRate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"twoYearGrowthRate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"employeeGrowthDataPoints\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"label\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"employeeCount\": {\n                \"type\": \"integer\",\n                \"example\": 250\n              }\n            },\n            \"required\": [\n              \"label\",\n              \"employeeCount\"\n            ]\n          }\n        }\n      },\n     \
  \ \"required\": [\n        \"oneYearGrowthRate\",\n        \"twoYearGrowthRate\",\n        \"employeeGrowthDataPoints\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"ticker\",\n    \"name\",\n    \"website\",\n    \"domainList\",\n    \"logo\",\n    \"socialMediaUrls\",\n    \"revenue\",\n    \"employeeCount\",\n    \"numberOfContactsInZoomInfo\",\n    \"phone\",\n    \"fax\",\n    \"street\",\n    \"city\",\n    \"state\",\n    \"zipCode\",\n    \"country\",\n    \"continent\",\n    \"companyStatus\",\n    \"companyStatusDate\",\n    \"descriptionList\",\n    \"sicCodes\",\n    \"naicsCodes\",\n    \"competitors\",\n    \"ultimateParentId\",\n    \"ultimateParentName\",\n    \"ultimateParentRevenue\",\n    \"ultimateParentEmployees\",\n    \"subUnitCodes\",\n    \"subUnitType\",\n    \"subUnitIndustries\",\n    \"primaryIndustry\",\n    \"industries\",\n    \"parentId\",\n    \"parentName\",\n    \"locationCount\",\n    \"alexaRank\",\n    \"metroArea\",\n    \"lastUpdatedDate\"\
  ,\n    \"createdDate\",\n    \"certificationDate\",\n    \"certified\",\n    \"hashtags\",\n    \"products\",\n    \"techAttributes\",\n    \"revenueRange\",\n    \"employeeRange\",\n    \"companyFunding\",\n    \"recentFundingAmount\",\n    \"recentFundingDate\",\n    \"totalFundingAmount\",\n    \"employeeGrowth\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data13\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data13-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: Data13
---
