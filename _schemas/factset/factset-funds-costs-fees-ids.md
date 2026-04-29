---
description: The requested Fund Identifier. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** = 1000 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective "POST" method.</p>*
layout: schema
name: costsFeesIds
properties_list: []
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-costs-fees-ids-schema.json
slug: factset-funds-costs-fees-ids
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"costsFeesIds\",\n  \"type\": \"array\",\n  \"description\": \"The requested Fund Identifier. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1000 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \\\"POST\\\" method.</p>*\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-costs-fees-ids-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: costsFeesIds
---
