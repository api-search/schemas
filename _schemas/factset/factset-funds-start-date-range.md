---
description: The start date requested for a given date range in YYYY-MM-DD format. If left blank, the API will default to the day prior to today's previous close. The startDate cannot be equal to the endDate as no return can be computed. Additionally, the startDate MUST be equal to or greater than the `priceFirstDate` found within the /summary endpoint.
layout: schema
name: startDateRange
properties_list: []
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-start-date-range-schema.json
slug: factset-funds-start-date-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"startDateRange\",\n  \"type\": \"string\",\n  \"description\": \"The start date requested for a given date range in YYYY-MM-DD format. If left blank, the API will default to the day prior to today's previous close. The startDate cannot be equal to the endDate as no return can be computed. Additionally, the startDate MUST be equal to or greater than the `priceFirstDate` found within the /summary endpoint.\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-start-date-range-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: startDateRange
---
