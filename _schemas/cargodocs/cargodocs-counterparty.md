---
description: A counterparty in the CargoDocs platform representing an organization or entity involved in a trade or shipping transaction.
layout: schema
name: CargoDocs Counterparty
properties_list:
- description: The unique identifier for the counterparty.
  name: counterpartyId
  type: string
- description: The name of the counterparty.
  name: counterpartyName
  type: string
provider_name: CargoDocs
provider_slug: cargodocs
schema_file: json-schema/cargodocs-counterparty.json
slug: cargodocs-counterparty
source_filename: cargodocs-counterparty.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-counterparty.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CargoDocs Counterparty\",\n  \"description\": \"A counterparty in the CargoDocs platform representing an organization or entity involved in a trade or shipping transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"counterpartyId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the counterparty.\"\n    },\n    \"counterpartyName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the counterparty.\"\n    }\n  },\n  \"required\": [\n    \"counterpartyId\",\n    \"counterpartyName\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/json-schema/cargodocs-counterparty.json
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
title: CargoDocs Counterparty
---
