---
description: ''
layout: schema
name: category
properties_list:
- description: 'Describes data based on source or kind of value - ACTUAL - Historical data collected directly from a press release or a median consensus from brokers after a report date. - ESTIMATE - Forward looking '
  name: category
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-ownership-report-builder-category-schema.json
slug: factset-ownership-report-builder-category
source_filename: factset-ownership-report-builder-category-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"category\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"object\",\n      \"description\": \"Describes data based on source or kind of value\\n- ACTUAL - Historical data collected directly from a press release or a median consensus from brokers after a report date.\\n- ESTIMATE - Forward looking average of broker estimates within a specific time horizon.\\n- GUIDANCE - Forward looking indication or estimate of future performance issued by the company itself.\\n- DETAIL - Indicates data that is more granular and may be secondary in focus.\\n- MAIN - Indicates data is of more impactful or higher importance and may want to be emphasized.\\n- SECTION - Indicates data that is used in sectioning rows in group level STACH format.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-ownership-report-builder-category-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: category
---
