---
description: The calculation periodicity for the aggregated period. **Note** - Not all periodicities are supported for each metric, depending on the type of ratio. LTM is set as default and supported for all metrics. See Metrics Parameter for additional detail on which periodicities are available per metric. |Periodicity|Description| |:|:| |LTM|Last Twelve Months |LTMA|Last Twelve Months using Broker Actuals for Estimated Items |STMA| Second Twelve Month Forward |NTMA| 12 Month Forward |0| Latest Reported Calendar Year |1| Current Unreported Year |2| Following Year |QTR| Quarterly - Reported by companies
layout: schema
name: periodicity
properties_list: []
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-benchmarks-periodicity-schema.json
slug: factset-benchmarks-periodicity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"periodicity\",\n  \"type\": \"string\",\n  \"description\": \"The calculation periodicity for the aggregated period. **Note** - Not all periodicities are supported for each metric, depending on the type of ratio. LTM is set as default and supported for all metrics. See Metrics Parameter for additional detail on which periodicities are available per metric.\\n|Periodicity|Description|\\n|:|:|\\n|LTM|Last Twelve Months\\n|LTMA|Last Twelve Months using Broker Actuals for Estimated Items\\n|STMA| Second Twelve Month Forward\\n|NTMA| 12 Month Forward\\n|0| Latest Reported Calendar Year\\n|1| Current Unreported Year\\n|2| Following Year\\n|QTR| Quarterly - Reported by companies\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-benchmarks-periodicity-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: periodicity
---
