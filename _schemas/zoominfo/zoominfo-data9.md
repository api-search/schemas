---
description: ''
layout: schema
name: Data9
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: firstName
  type: string
- description: ''
  name: middleName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: hasCanadianEmail
  type: string
- description: ''
  name: phone
  type: string
- description: ''
  name: directPhoneDoNotCall
  type: boolean
- description: ''
  name: street
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: metroArea
  type: string
- description: ''
  name: zipCode
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: personHasMoved
  type: string
- description: ''
  name: withinEu
  type: boolean
- description: ''
  name: withinCalifornia
  type: boolean
- description: ''
  name: withinCanada
  type: boolean
- description: ''
  name: lastUpdatedDate
  type: string
- description: ''
  name: noticeProvidedDate
  type: string
- description: ''
  name: salutation
  type: string
- description: ''
  name: suffix
  type: string
- description: ''
  name: jobTitle
  type: string
- description: ''
  name: jobFunction
  type: array
- description: ''
  name: education
  type: array
- description: ''
  name: hashedEmails
  type: array
- description: ''
  name: picture
  type: string
- description: ''
  name: mobilePhoneDoNotCall
  type: boolean
- description: ''
  name: externalUrls
  type: array
- description: ''
  name: contactAccuracyScore
  type: integer
- description: ''
  name: isDefunct
  type: boolean
- description: ''
  name: employmentHistory
  type: array
- description: ''
  name: managementLevel
  type: array
- description: ''
  name: company
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data9-schema.json
slug: zoominfo-data9
source_filename: zoominfo-data9-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"hasCanadianEmail\": {\n      \"type\": \"string\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"+1-555-555-1234\"\n    },\n    \"directPhoneDoNotCall\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"example\": \"\
  San Francisco\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"metroArea\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"zipCode\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    },\n    \"personHasMoved\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"withinEu\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"withinCalifornia\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"withinCanada\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"lastUpdatedDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"noticeProvidedDate\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"salutation\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"example\": \"Vice President of Sales\"\n    },\n    \"jobFunction\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"education\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"hashedEmails\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"user@example.com\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"picture\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"mobilePhoneDoNotCall\"\
  : {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"externalUrls\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"https://www.example.com\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com/resource\"\n          }\n        },\n        \"required\": [\n          \"type\",\n          \"url\"\n        ]\n      }\n    },\n    \"contactAccuracyScore\": {\n      \"type\": \"integer\",\n      \"example\": 85\n    },\n    \"isDefunct\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"employmentHistory\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n   \
  \       \"jobTitle\": {\n            \"type\": \"string\",\n            \"example\": \"Vice President of Sales\"\n          },\n          \"managementLevel\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"fromDate\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"toDate\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"company\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"companyId\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"companyName\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              },\n              \"companyPhone\": {\n\
  \                \"type\": \"string\",\n                \"example\": \"+1-555-555-1234\"\n              },\n              \"companyWebsite\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"companyId\",\n              \"companyName\",\n              \"companyPhone\",\n              \"companyWebsite\"\n            ]\n          }\n        },\n        \"required\": [\n          \"jobTitle\",\n          \"managementLevel\",\n          \"fromDate\",\n          \"toDate\",\n          \"company\"\n        ]\n      }\n    },\n    \"managementLevel\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"company\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"division\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n    \
  \    },\n        \"id\": {\n          \"type\": \"integer\",\n          \"example\": 500123\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"descriptionList\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"description\": {\n                \"type\": \"string\",\n                \"example\": \"Enterprise software company\"\n              }\n            },\n            \"required\": [\n              \"description\"\n            ]\n          }\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"example\": \"+1-555-555-1234\"\n        },\n        \"fax\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"street\": {\n          \"type\": \"string\",\n          \"example\": \"\
  example_value\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"example\": \"San Francisco\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"example\": \"CA\"\n        },\n        \"zipCode\": {\n          \"type\": \"string\",\n          \"example\": \"94105\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"example\": \"US\"\n        },\n        \"logo\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"sicCodes\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n    \
  \          }\n            },\n            \"required\": [\n              \"id\",\n              \"name\"\n            ]\n          }\n        },\n        \"naicsCodes\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"name\"\n            ]\n          }\n        },\n        \"website\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"revenue\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"revenueNumeric\": {\n\
  \          \"type\": \"integer\",\n          \"example\": 100\n        },\n        \"employeeCount\": {\n          \"type\": \"integer\",\n          \"example\": 250\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        },\n        \"ticker\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"ranking\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"socialMediaUrls\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": \"https://www.example.com\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"example\": \"standard\"\n              },\n              \"url\": {\n            \
  \    \"type\": \"string\",\n                \"example\": \"https://www.example.com/resource\"\n              },\n              \"followerCount\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"type\",\n              \"url\",\n              \"followerCount\"\n            ]\n          }\n        },\n        \"primaryIndustry\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"industries\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"revenueRange\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"employeeRange\": {\n          \"type\": \"\
  string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"division\",\n        \"id\",\n        \"name\",\n        \"descriptionList\",\n        \"phone\",\n        \"fax\",\n        \"street\",\n        \"city\",\n        \"state\",\n        \"zipCode\",\n        \"country\",\n        \"logo\",\n        \"sicCodes\",\n        \"naicsCodes\",\n        \"website\",\n        \"revenue\",\n        \"revenueNumeric\",\n        \"employeeCount\",\n        \"type\",\n        \"ticker\",\n        \"ranking\",\n        \"socialMediaUrls\",\n        \"primaryIndustry\",\n        \"industries\",\n        \"revenueRange\",\n        \"employeeRange\"\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"firstName\",\n    \"middleName\",\n    \"lastName\",\n    \"email\",\n    \"hasCanadianEmail\",\n    \"phone\",\n    \"directPhoneDoNotCall\",\n    \"street\",\n    \"city\",\n    \"region\",\n    \"metroArea\",\n    \"zipCode\",\n    \"state\"\
  ,\n    \"country\",\n    \"personHasMoved\",\n    \"withinEu\",\n    \"withinCalifornia\",\n    \"withinCanada\",\n    \"lastUpdatedDate\",\n    \"noticeProvidedDate\",\n    \"salutation\",\n    \"suffix\",\n    \"jobTitle\",\n    \"jobFunction\",\n    \"education\",\n    \"hashedEmails\",\n    \"picture\",\n    \"mobilePhoneDoNotCall\",\n    \"externalUrls\",\n    \"contactAccuracyScore\",\n    \"isDefunct\",\n    \"employmentHistory\",\n    \"managementLevel\",\n    \"company\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data9\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data9-schema.json
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
title: Data9
---
