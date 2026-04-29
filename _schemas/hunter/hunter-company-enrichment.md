---
description: ''
layout: schema
name: CompanyEnrichment
properties_list:
- description: Unique identifier for the company record.
  name: id
  type: string
- description: Company name.
  name: name
  type: '[''string'', ''null'']'
- description: Legal name of the company.
  name: legalName
  type: '[''string'', ''null'']'
- description: Company domain name.
  name: domain
  type: string
- description: Alternate domain names.
  name: domainAliases
  type: array
- description: ''
  name: site
  type: object
- description: Industry classification.
  name: category
  type: object
- description: Tags associated with the company.
  name: tags
  type: array
- description: Company description.
  name: description
  type: '[''string'', ''null'']'
- description: Year the company was founded.
  name: foundedYear
  type: '[''integer'', ''null'']'
- description: Location description.
  name: location
  type: '[''string'', ''null'']'
- description: Time zone name.
  name: timeZone
  type: '[''string'', ''null'']'
- description: UTC offset in hours.
  name: utcOffset
  type: '[''number'', ''null'']'
- description: Company logo URL.
  name: logo
  type: '[''string'', ''null'']'
- description: ''
  name: facebook
  type: object
- description: ''
  name: linkedin
  type: object
- description: ''
  name: twitter
  type: object
- description: ''
  name: crunchbase
  type: object
- description: Email service provider.
  name: emailProvider
  type: '[''string'', ''null'']'
- description: Company type.
  name: type
  type: '[''string'', ''null'']'
- description: Entity type classification.
  name: company_type
  type: '[''string'', ''null'']'
- description: Stock ticker symbol.
  name: ticker
  type: '[''string'', ''null'']'
- description: ''
  name: identifiers
  type: object
- description: Primary phone number.
  name: phone
  type: '[''string'', ''null'']'
- description: ''
  name: metrics
  type: object
- description: Date when the record was last indexed.
  name: indexedAt
  type: '[''string'', ''null'']'
- description: Technologies used by the company.
  name: tech
  type: array
- description: Categories of technologies used.
  name: techCategories
  type: array
- description: ''
  name: parent
  type: object
- description: ''
  name: ultimateParent
  type: object
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-company-enrichment-schema.json
slug: hunter-company-enrichment
source_filename: hunter-company-enrichment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompanyEnrichment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the company record.\"\n    },\n    \"name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Company name.\"\n    },\n    \"legalName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Legal name of the company.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Company domain name.\"\n    },\n    \"domainAliases\": {\n      \"type\": \"array\",\n      \"description\": \"Alternate domain names.\"\n    },\n    \"site\": {\n      \"type\": \"object\"\n    },\n    \"category\": {\n      \"type\": \"object\",\n      \"description\": \"Industry classification.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the company.\"\
  \n    },\n    \"description\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Company description.\"\n    },\n    \"foundedYear\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Year the company was founded.\"\n    },\n    \"location\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Location description.\"\n    },\n    \"timeZone\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Time zone name.\"\n    },\n    \"utcOffset\": {\n      \"type\": \"['number', 'null']\",\n      \"description\": \"UTC offset in hours.\"\n    },\n    \"logo\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Company logo URL.\"\n    },\n    \"facebook\": {\n      \"type\": \"object\"\n    },\n    \"linkedin\": {\n      \"type\": \"object\"\n    },\n    \"twitter\": {\n      \"type\": \"object\"\n    },\n    \"crunchbase\": {\n      \"type\": \"object\"\n    },\n    \"emailProvider\": {\n      \"type\"\
  : \"['string', 'null']\",\n      \"description\": \"Email service provider.\"\n    },\n    \"type\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Company type.\"\n    },\n    \"company_type\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Entity type classification.\"\n    },\n    \"ticker\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Stock ticker symbol.\"\n    },\n    \"identifiers\": {\n      \"type\": \"object\"\n    },\n    \"phone\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Primary phone number.\"\n    },\n    \"metrics\": {\n      \"type\": \"object\"\n    },\n    \"indexedAt\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Date when the record was last indexed.\"\n    },\n    \"tech\": {\n      \"type\": \"array\",\n      \"description\": \"Technologies used by the company.\"\n    },\n    \"techCategories\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Categories of technologies used.\"\n    },\n    \"parent\": {\n      \"type\": \"object\"\n    },\n    \"ultimateParent\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-company-enrichment-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: CompanyEnrichment
---
