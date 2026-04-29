---
description: A company represents a legal entity within AvaTax that can calculate and report taxes. Companies contain locations, nexus declarations, items, and other tax configuration data.
layout: schema
name: Avalara Company
properties_list:
- description: Unique identifier for the company
  name: id
  type: integer
- description: Short code identifying this company in transactions
  name: companyCode
  type: string
- description: Display name of the company
  name: name
  type: string
- description: Account ID that owns this company
  name: accountId
  type: integer
- description: Parent company ID for multi-company hierarchies
  name: parentCompanyId
  type: integer
- description: Whether this is the default company for the account
  name: isDefault
  type: boolean
- description: Whether the company is currently active
  name: isActive
  type: boolean
- description: Tax identification number (EIN, TIN, VAT number)
  name: taxpayerIdNumber
  type: string
- description: Whether the company has a completed tax profile
  name: hasProfile
  type: boolean
- description: Whether this company is a reporting entity
  name: isReportingEntity
  type: boolean
- description: Two-character ISO 3166 country code for the default country
  name: defaultCountry
  type: string
- description: Three-character ISO 4217 currency code
  name: baseCurrencyCode
  type: string
- description: Level at which tax rounding is applied
  name: roundingLevelId
  type: string
- description: ''
  name: address
  type: object
- description: Nexus declarations for this company
  name: nexus
  type: array
- description: Physical locations belonging to this company
  name: locations
  type: array
- description: Date and time the company was created
  name: createdDate
  type: string
- description: Date and time the company was last modified
  name: modifiedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avalara-company-schema.json
slug: avalara-company
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.avalara.com/schemas/avalara/company.json\",\n  \"title\": \"Avalara Company\",\n  \"description\": \"A company represents a legal entity within AvaTax that can calculate and report taxes. Companies contain locations, nexus declarations, items, and other tax configuration data.\",\n  \"type\": \"object\",\n  \"required\": [\"companyCode\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the company\"\n    },\n    \"companyCode\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 25,\n      \"description\": \"Short code identifying this company in transactions\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 250,\n      \"description\": \"Display name of the company\"\n    },\n    \"accountId\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Account ID that owns this company\"\n    },\n    \"parentCompanyId\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent company ID for multi-company hierarchies\"\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the default company for the account\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the company is currently active\"\n    },\n    \"taxpayerIdNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Tax identification number (EIN, TIN, VAT number)\"\n    },\n    \"hasProfile\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the company has a completed tax profile\"\n    },\n    \"isReportingEntity\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this company is a reporting entity\"\n    },\n    \"defaultCountry\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{2}$\",\n      \"\
  description\": \"Two-character ISO 3166 country code for the default country\"\n    },\n    \"baseCurrencyCode\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"Three-character ISO 4217 currency code\"\n    },\n    \"roundingLevelId\": {\n      \"type\": \"string\",\n      \"enum\": [\"Line\", \"Document\"],\n      \"description\": \"Level at which tax rounding is applied\"\n    },\n    \"address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"nexus\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Nexus\"\n      },\n      \"description\": \"Nexus declarations for this company\"\n    },\n    \"locations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Location\"\n      },\n      \"description\": \"Physical locations belonging to this company\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date\
  \ and time the company was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the company was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A physical address\",\n      \"properties\": {\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"line2\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"region\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        }\n      }\n    },\n    \"Nexus\": {\n      \"type\": \"object\",\n      \"description\": \"A nexus declaration indicating tax obligation in a jurisdiction\",\n      \"properties\": {\n        \"id\": {\n\
  \          \"type\": \"integer\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Two-character ISO 3166 country code\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"State or province code\"\n        },\n        \"jurisTypeId\": {\n          \"type\": \"string\",\n          \"enum\": [\"STA\", \"CTY\", \"CIT\", \"STJ\", \"CNT\"]\n        },\n        \"jurisCode\": {\n          \"type\": \"string\"\n        },\n        \"jurisName\": {\n          \"type\": \"string\"\n        },\n        \"nexusTypeId\": {\n          \"type\": \"string\",\n          \"enum\": [\"None\", \"SalesOrSellersUseTax\", \"SalesTax\", \"SSTVolunteer\", \"SSTNonVolunteer\"]\n        },\n        \"effectiveDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"endDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        }\n      }\n    },\n    \"\
  Location\": {\n      \"type\": \"object\",\n      \"description\": \"A physical location belonging to a company\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"locationCode\": {\n          \"type\": \"string\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"addressTypeId\": {\n          \"type\": \"string\",\n          \"enum\": [\"Firm\", \"Location\", \"Salesperson\"]\n        },\n        \"addressCategoryId\": {\n          \"type\": \"string\",\n          \"enum\": [\"Storefront\", \"MainOffice\", \"Warehouse\", \"Salesperson\", \"Other\"]\n        },\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"region\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        }\n\
  \      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avalara-company-schema.json
tags:
- Taxes
title: Avalara Company
---
