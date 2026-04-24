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
tags:
- Business Intelligence
- Company Data
- CRM
- Firmographic Data
- NAICS
- SIC
title: BizAPI Company
---
