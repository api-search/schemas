---
description: Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. *<p>Make note, GET Method URL request lines are also limited to a total length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective "POST" method.</p>*
layout: schema
name: paiIds
properties_list: []
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-esg-pai-ids-schema.json
slug: factset-esg-pai-ids
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"paiIds\",\n  \"type\": \"array\",\n  \"description\": \"Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input.  *<p>Make note, GET Method URL request lines are also limited to a total length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \\\"POST\\\" method.</p>*\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-esg-pai-ids-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: paiIds
---
