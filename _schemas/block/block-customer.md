---
description: Represents a customer profile in a Square seller account.
layout: schema
name: Customer
properties_list:
- description: Unique ID for this customer.
  name: id
  type: string
- description: Customer's first name.
  name: given_name
  type: string
- description: Customer's last name.
  name: family_name
  type: string
- description: Customer's email address.
  name: email_address
  type: string
- description: Customer's phone number.
  name: phone_number
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Block
provider_slug: block
schema_file: json-schema/block-customer-schema.json
slug: block-customer
source_filename: block-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/block/main/json-schema/block-customer-schema.json\",\n  \"title\": \"Customer\",\n  \"description\": \"Represents a customer profile in a Square seller account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique ID for this customer.\",\n      \"example\": \"JDKYHBWT1D4F8MFH63DBMEN8Y4\"\n    },\n    \"given_name\": {\n      \"type\": \"string\",\n      \"description\": \"Customer's first name.\",\n      \"example\": \"Amelia\"\n    },\n    \"family_name\": {\n      \"type\": \"string\",\n      \"description\": \"Customer's last name.\",\n      \"example\": \"Earhart\"\n    },\n    \"email_address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Customer's email address.\",\n      \"example\": \"Amelia.Earhart@example.com\"\n    },\n\
  \    \"phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"Customer's phone number.\",\n      \"example\": \"+11234567890\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-03-23T20:21:54.859Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-03-23T20:21:55Z\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/json-schema/block-customer-schema.json
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
title: Customer
---
