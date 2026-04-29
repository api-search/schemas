---
description: The start date requested for a given date range in **YYYY-MM-DD** format. In the context of corporate actions, this filters the response to only include events within the date range. The frequency between the startDate and endDate is always set to the "event" frequency- meaning the service will return only events within those inclusive boundaries. Leaving both startDate and endDate blank will pull "all" events for each requested ids.
layout: schema
name: startDateCA
properties_list: []
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-global-prices-start-date-ca-schema.json
slug: factset-global-prices-start-date-ca
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"startDateCA\",\n  \"type\": \"string\",\n  \"description\": \"The start date requested for a given date range in **YYYY-MM-DD** format. In the context of corporate actions, this filters the response to only include events within the date range. The frequency between the startDate and endDate is always set to the \\\"event\\\" frequency- meaning the service will return only events within those inclusive boundaries. Leaving both startDate and endDate blank will pull \\\"all\\\" events for each requested ids.\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-global-prices-start-date-ca-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: startDateCA
---
