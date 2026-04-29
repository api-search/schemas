---
description: Insurance Certificate of Currency confirming active coverage
layout: schema
name: CertificateOfCurrency
properties_list:
- description: Unique identifier for the certificate
  name: certificate_id
  type: string
- description: Policy number the certificate relates to
  name: policy_number
  type: string
- description: Name of the insured party
  name: insured_name
  type: string
- description: Insurance product type
  name: product_type
  type: string
- description: Coverage start date
  name: coverage_start
  type: string
- description: Coverage end date
  name: coverage_end
  type: string
- description: Total sum insured amount
  name: sum_insured
  type: number
- description: Currency code for the sum insured
  name: currency
  type: string
- description: Timestamp when the certificate was issued
  name: issued_at
  type: string
- description: URL to download the certificate as a PDF document
  name: download_url
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-certificate-of-currency-schema.json
slug: api-connect-certificate-of-currency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-certificate-of-currency-schema.json\",\n  \"title\": \"CertificateOfCurrency\",\n  \"description\": \"Insurance Certificate of Currency confirming active coverage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificate_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the certificate\",\n      \"example\": \"cert-500123\"\n    },\n    \"policy_number\": {\n      \"type\": \"string\",\n      \"description\": \"Policy number the certificate relates to\",\n      \"example\": \"ALZ-2026-500567\"\n    },\n    \"insured_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the insured party\",\n      \"example\": \"Jane Smith\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance product type\"\
  ,\n      \"example\": \"home\"\n    },\n    \"coverage_start\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Coverage start date\",\n      \"example\": \"2026-01-01\"\n    },\n    \"coverage_end\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Coverage end date\",\n      \"example\": \"2027-01-01\"\n    },\n    \"sum_insured\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total sum insured amount\",\n      \"example\": 750000.0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code for the sum insured\",\n      \"example\": \"AUD\"\n    },\n    \"issued_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the certificate was issued\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    },\n    \"download_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\
  ,\n      \"description\": \"URL to download the certificate as a PDF document\",\n      \"example\": \"https://api.allianz.com.au/v1/certificates/cert-500123/download\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-certificate-of-currency-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: CertificateOfCurrency
---
