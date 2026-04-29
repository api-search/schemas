---
description: Supplier schema from 1Factory API
layout: schema
name: Supplier
properties_list:
- description: ''
  name: ID
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: vendor_code
  type: object
- description: ''
  name: address
  type: object
- description: ''
  name: supply_chain_manager
  type: object
- description: ''
  name: supplier_quality_manager
  type: object
- description: ''
  name: purchasing
  type: object
- description: Indicates if the supplier provides direct materials or services.
  name: direct
  type: boolean
- description: Indicates if the supplier provides indirect materials or services.
  name: indirect
  type: boolean
- description: Indicates if the supplier is considered strategic to the organization.
  name: strategic
  type: boolean
- description: Indicates if the supplier is classified as a small business.
  name: small_business
  type: boolean
- description: List of organization codes associated with the supplier.
  name: organization_codes
  type: array
- description: List of commodity codes that the supplier provides.
  name: commodity_codes
  type: array
- description: List of supplier qualifications and their status history.
  name: qualifications
  type: array
- description: List of supplier certifications and their expiration dates.
  name: certifications
  type: array
- description: Current qualification status derived from the most recent qualification entry.
  name: qualification_status
  type: string
- description: Date and time of the most recent qualification assessment.
  name: last_qualification_date
  type: string
- description: Calculated date when the supplier needs to be re-qualified, based on the last qualification date plus frequency in months.
  name: re_qualification_date
  type: string
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-supplier-schema.json
slug: 1factory-supplier
source_filename: 1factory-supplier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-supplier-schema.json\",\n  \"title\": \"Supplier\",\n  \"description\": \"Supplier schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"$ref\": \"#/components/schemas/ID\"\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/supplier_name\"\n        },\n        {\n          \"nullable\": false\n        }\n      ]\n    },\n    \"vendor_code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/supplier_number\"\n        },\n        {\n          \"nullable\": false\n        }\n      ]\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"supply_chain_manager\": {\n      \"$ref\": \"#/components/schemas/User\"\n    },\n    \"supplier_quality_manager\"\
  : {\n      \"$ref\": \"#/components/schemas/User\"\n    },\n    \"purchasing\": {\n      \"$ref\": \"#/components/schemas/User\"\n    },\n    \"direct\": {\n      \"type\": \"boolean\",\n      \"nullable\": false,\n      \"default\": false,\n      \"description\": \"Indicates if the supplier provides direct materials or services.\"\n    },\n    \"indirect\": {\n      \"type\": \"boolean\",\n      \"nullable\": false,\n      \"default\": false,\n      \"description\": \"Indicates if the supplier provides indirect materials or services.\"\n    },\n    \"strategic\": {\n      \"type\": \"boolean\",\n      \"nullable\": false,\n      \"default\": false,\n      \"description\": \"Indicates if the supplier is considered strategic to the organization.\"\n    },\n    \"small_business\": {\n      \"type\": \"boolean\",\n      \"nullable\": false,\n      \"default\": false,\n      \"description\": \"Indicates if the supplier is classified as a small business.\"\n    },\n    \"organization_codes\"\
  : {\n      \"type\": \"array\",\n      \"nullable\": true,\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"string\",\n        \"maxLength\": 50\n      },\n      \"description\": \"List of organization codes associated with the supplier.\",\n      \"example\": [\n        \"1001\",\n        \"1002\"\n      ]\n    },\n    \"commodity_codes\": {\n      \"type\": \"array\",\n      \"nullable\": true,\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"string\",\n        \"maxLength\": 100\n      },\n      \"description\": \"List of commodity codes that the supplier provides.\",\n      \"example\": [\n        \"Machined\",\n        \"Anodization\"\n      ]\n    },\n    \"qualifications\": {\n      \"type\": \"array\",\n      \"nullable\": true,\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Qualification\"\n      },\n      \"description\": \"List of supplier qualifications and their status history.\"\n    },\n    \"certifications\"\
  : {\n      \"type\": \"array\",\n      \"nullable\": true,\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Certification\"\n      },\n      \"description\": \"List of supplier certifications and their expiration dates.\"\n    },\n    \"qualification_status\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"enum\": [\n        \"New\",\n        \"Approved\",\n        \"Conditional\",\n        \"Disqualified\",\n        \"Inactive\"\n      ],\n      \"description\": \"Current qualification status derived from the most recent qualification entry.\",\n      \"example\": \"Conditional\"\n    },\n    \"last_qualification_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"description\": \"Date and time of the most recent qualification assessment.\",\n      \"example\": \"2016-12-02T00:00:00-08:00\"\n    },\n    \"re_qualification_date\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"description\": \"Calculated date when the supplier needs to be re-qualified, based on the last qualification date plus frequency in months.\",\n      \"example\": \"2017-12-02T00:00:00-08:00\"\n    }\n  },\n  \"required\": [\n    \"ID\",\n    \"name\",\n    \"vendor_code\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-supplier-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Supplier
---
