---
description: ''
layout: schema
name: Address
properties_list:
- description: Address identifier
  name: addressId
  type: integer
- description: Address type
  name: addressType
  type: string
- description: ''
  name: addressLine1
  type: string
- description: ''
  name: addressLine2
  type: string
- description: ''
  name: addressLine3
  type: string
- description: ''
  name: townOrCity
  type: string
- description: County/province
  name: region1
  type: string
- description: State
  name: region2
  type: string
- description: ''
  name: postalCode
  type: string
- description: Country code
  name: country
  type: string
- description: ''
  name: primaryFlag
  type: string
- description: ''
  name: dateFrom
  type: string
- description: ''
  name: dateTo
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-address-schema.json
slug: human-resources-address
source_filename: human-resources-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addressId\": {\n      \"type\": \"integer\",\n      \"description\": \"Address identifier\"\n    },\n    \"addressType\": {\n      \"type\": \"string\",\n      \"description\": \"Address type\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\"\n    },\n    \"addressLine3\": {\n      \"type\": \"string\"\n    },\n    \"townOrCity\": {\n      \"type\": \"string\"\n    },\n    \"region1\": {\n      \"type\": \"string\",\n      \"description\": \"County/province\"\n    },\n    \"region2\": {\n      \"type\": \"string\",\n      \"description\": \"State\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code\"\n    },\n    \"primaryFlag\": {\n      \"type\": \"string\"\
  \n    },\n    \"dateFrom\": {\n      \"type\": \"string\"\n    },\n    \"dateTo\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-address-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Address
---
