---
description: A customer in the CargoDocs platform representing an organization that uses CargoDocs services for managing electronic trade documents.
layout: schema
name: CargoDocs Customer
properties_list:
- description: The unique identifier for the customer.
  name: customerId
  type: string
- description: The name of the customer.
  name: customerName
  type: string
provider_name: CargoDocs
provider_slug: cargodocs
schema_file: json-schema/cargodocs-customer.json
slug: cargodocs-customer
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-customer.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CargoDocs Customer\",\n  \"description\": \"A customer in the CargoDocs platform representing an organization that uses CargoDocs services for managing electronic trade documents.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the customer.\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the customer.\"\n    }\n  },\n  \"required\": [\n    \"customerId\",\n    \"customerName\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-customer.json
tags:
- Bills of Lading
- Documentation
- eBoL
- EssDocs
- MLETR
- Shipping
- Supply Chain
- Trade
- Trade Finance
- Warehouse Warrants
title: CargoDocs Customer
---
