---
description: A business entity record returned by the BizAPI Business Intelligence API, containing firmographic data including identification numbers, industry codes, address, contact information, financial indicators, and corporate hierarchy details.
layout: schema
name: BizAPI Company
properties_list:
- description: DUNS number uniquely identifying the business entity.
  name: duns_number
  type: string
- description: Legal name of the company.
  name: company_name
  type: string
- description: Doing-business-as (trade) name.
  name: dba
  type: string
- description: 4-digit Standard Industrial Classification code.
  name: sic_code_4
  type: string
- description: 8-digit Standard Industrial Classification code.
  name: sic_code_8
  type: string
- description: 6-digit North American Industry Classification System code.
  name: naics_code_6
  type: string
- description: Street address of the business location.
  name: street
  type: string
- description: City of the business location.
  name: city
  type: string
- description: State or province of the business location.
  name: state
  type: string
- description: ZIP or postal code of the business location.
  name: zip
  type: string
- description: Country of the business location.
  name: country
  type: string
- description: Latitude coordinate of the business location.
  name: latitude
  type: number
- description: Longitude coordinate of the business location.
  name: longitude
  type: number
- description: Primary phone number.
  name: phone
  type: string
- description: Fax number.
  name: fax
  type: string
- description: Primary contact email address.
  name: email
  type: string
- description: Company website URL.
  name: url
  type: string
- description: Stock exchange ticker symbol.
  name: stock_ticker
  type: string
- description: Name of the top contact at the company.
  name: top_contact_name
  type: string
- description: Title of the top contact at the company.
  name: top_contact_title
  type: string
- description: Annual sales volume.
  name: sales_volume
  type: string
- description: Total number of employees.
  name: total_employees
  type: string
- description: Number of employees at this location.
  name: employees_on_site
  type: string
- description: Year the company was established.
  name: year_started
  type: string
- description: Location type indicator.
  name: location_type
  type: string
- description: Subsidiary status indicator.
  name: subsidiary_indicator
  type: string
- description: DUNS number of the parent company.
  name: parent_duns
  type: string
- description: Name of the parent company.
  name: parent_name
  type: string
- description: DUNS number of the domestic ultimate parent.
  name: domestic_ultimate_duns
  type: string
- description: Name of the domestic ultimate parent.
  name: domestic_ultimate_name
  type: string
- description: DUNS number of the global ultimate parent.
  name: global_ultimate_duns
  type: string
- description: Name of the global ultimate parent.
  name: global_ultimate_name
  type: string
- description: Corporate hierarchy code.
  name: hierarchy_code
  type: string
- description: Number of family members in the corporate hierarchy.
  name: family_member_count
  type: string
provider_name: BizAPI
provider_slug: bizapi
schema_file: json-schema/bizapi-company-schema.json
slug: bizapi-company
source_json: "{\n  \"$id\": \"bizapi-company-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BizAPI Company\",\n  \"description\": \"A business entity record returned by the BizAPI Business Intelligence API, containing firmographic data including identification numbers, industry codes, address, contact information, financial indicators, and corporate hierarchy details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duns_number\": {\n      \"type\": \"string\",\n      \"description\": \"DUNS number uniquely identifying the business entity.\"\n    },\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Legal name of the company.\"\n    },\n    \"dba\": {\n      \"type\": \"string\",\n      \"description\": \"Doing-business-as (trade) name.\"\n    },\n    \"sic_code_4\": {\n      \"type\": \"string\",\n      \"description\": \"4-digit Standard Industrial Classification code.\",\n      \"pattern\": \"^[0-9]{4}$\"\
  \n    },\n    \"sic_code_8\": {\n      \"type\": \"string\",\n      \"description\": \"8-digit Standard Industrial Classification code.\",\n      \"pattern\": \"^[0-9]{8}$\"\n    },\n    \"naics_code_6\": {\n      \"type\": \"string\",\n      \"description\": \"6-digit North American Industry Classification System code.\",\n      \"pattern\": \"^[0-9]{6}$\"\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"description\": \"Street address of the business location.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City of the business location.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province of the business location.\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP or postal code of the business location.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of the business location.\"\n    },\n    \"latitude\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"Latitude coordinate of the business location.\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude coordinate of the business location.\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number.\"\n    },\n    \"fax\": {\n      \"type\": \"string\",\n      \"description\": \"Fax number.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Primary contact email address.\",\n      \"format\": \"email\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Company website URL.\",\n      \"format\": \"uri\"\n    },\n    \"stock_ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Stock exchange ticker symbol.\"\n    },\n    \"top_contact_name\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"Name of the top contact at the company.\"\n    },\n    \"top_contact_title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the top contact at the company.\"\n    },\n    \"sales_volume\": {\n      \"type\": \"string\",\n      \"description\": \"Annual sales volume.\"\n    },\n    \"total_employees\": {\n      \"type\": \"string\",\n      \"description\": \"Total number of employees.\"\n    },\n    \"employees_on_site\": {\n      \"type\": \"string\",\n      \"description\": \"Number of employees at this location.\"\n    },\n    \"year_started\": {\n      \"type\": \"string\",\n      \"description\": \"Year the company was established.\",\n      \"pattern\": \"^[0-9]{4}$\"\n    },\n    \"location_type\": {\n      \"type\": \"string\",\n      \"description\": \"Location type indicator.\",\n      \"enum\": [\"HQ\", \"Branch\", \"SL\"]\n    },\n    \"subsidiary_indicator\": {\n      \"type\": \"string\",\n      \"description\": \"Subsidiary status\
  \ indicator.\"\n    },\n    \"parent_duns\": {\n      \"type\": \"string\",\n      \"description\": \"DUNS number of the parent company.\"\n    },\n    \"parent_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the parent company.\"\n    },\n    \"domestic_ultimate_duns\": {\n      \"type\": \"string\",\n      \"description\": \"DUNS number of the domestic ultimate parent.\"\n    },\n    \"domestic_ultimate_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the domestic ultimate parent.\"\n    },\n    \"global_ultimate_duns\": {\n      \"type\": \"string\",\n      \"description\": \"DUNS number of the global ultimate parent.\"\n    },\n    \"global_ultimate_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the global ultimate parent.\"\n    },\n    \"hierarchy_code\": {\n      \"type\": \"string\",\n      \"description\": \"Corporate hierarchy code.\"\n    },\n    \"family_member_count\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Number of family members in the corporate hierarchy.\"\n    }\n  },\n  \"required\": [\n    \"company_name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bizapi/refs/heads/main/json-schema/bizapi-company-schema.json
tags:
- Business Intelligence
- Company Data
- CRM
- Firmographic Data
- NAICS
- SIC
title: BizAPI Company
---
