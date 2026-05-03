---
description: Schema for a carbon emission record in Salesforce Net Zero Cloud, tracking greenhouse gas emissions by scope, source, and reporting period.
layout: schema
name: Salesforce Net Zero Cloud Carbon Emission
properties_list:
- description: Salesforce record ID
  name: Id
  type: string
- description: Auto-generated name for the emission record
  name: Name
  type: string
- description: GHG Protocol scope category
  name: Scope
  type: integer
- description: The source of the emission (e.g., Natural Gas Combustion, Business Travel)
  name: EmissionSource
  type: string
- description: Quantity of greenhouse gas emissions in metric tons of CO2 equivalent
  name: QuantityMtCO2e
  type: number
- description: The fiscal or calendar year for this emission record
  name: ReportingYear
  type: integer
- description: Start date of the reporting period
  name: ReportingPeriodStartDate
  type: string
- description: End date of the reporting period
  name: ReportingPeriodEndDate
  type: string
- description: Salesforce ID of the associated facility record
  name: FacilityId
  type: string
- description: Salesforce ID of the emission factor used for calculation
  name: EmissionFactorId
  type: string
- description: Method used to calculate the emission quantity
  name: CalculationMethod
  type: string
- description: Additional description or notes for this emission record
  name: Description
  type: string
- description: Timestamp when the record was created
  name: CreatedDate
  type: string
- description: Timestamp when the record was last modified
  name: LastModifiedDate
  type: string
provider_name: Salesforce Net Zero Cloud
provider_slug: salesforce-net-zero-cloud
schema_file: json-schema/salesforce-net-zero-cloud-carbon-emission-schema.json
slug: salesforce-net-zero-cloud-carbon-emission
source_filename: salesforce-net-zero-cloud-carbon-emission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salesforce-net-zero-cloud/blob/main/json-schema/salesforce-net-zero-cloud-carbon-emission-schema.json\",\n  \"title\": \"Salesforce Net Zero Cloud Carbon Emission\",\n  \"description\": \"Schema for a carbon emission record in Salesforce Net Zero Cloud, tracking greenhouse gas emissions by scope, source, and reporting period.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce record ID\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated name for the emission record\"\n    },\n    \"Scope\": {\n      \"type\": \"integer\",\n      \"description\": \"GHG Protocol scope category\",\n      \"enum\": [1, 2, 3]\n    },\n    \"EmissionSource\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the emission (e.g., Natural Gas\
  \ Combustion, Business Travel)\"\n    },\n    \"QuantityMtCO2e\": {\n      \"type\": \"number\",\n      \"description\": \"Quantity of greenhouse gas emissions in metric tons of CO2 equivalent\",\n      \"minimum\": 0\n    },\n    \"ReportingYear\": {\n      \"type\": \"integer\",\n      \"description\": \"The fiscal or calendar year for this emission record\",\n      \"minimum\": 1990,\n      \"maximum\": 2100\n    },\n    \"ReportingPeriodStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of the reporting period\"\n    },\n    \"ReportingPeriodEndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date of the reporting period\"\n    },\n    \"FacilityId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the associated facility record\"\n    },\n    \"EmissionFactorId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the emission\
  \ factor used for calculation\"\n    },\n    \"CalculationMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Method used to calculate the emission quantity\",\n      \"enum\": [\"SpendBased\", \"ActivityBased\", \"SupplierSpecific\", \"AverageBased\"]\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional description or notes for this emission record\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was created\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was last modified\"\n    }\n  },\n  \"required\": [\"Scope\", \"QuantityMtCO2e\", \"ReportingYear\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-net-zero-cloud/refs/heads/main/json-schema/salesforce-net-zero-cloud-carbon-emission-schema.json
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Environmental
- ESG
- Net Zero
- Sustainability
title: Salesforce Net Zero Cloud Carbon Emission
---
