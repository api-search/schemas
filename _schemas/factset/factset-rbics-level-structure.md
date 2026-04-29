---
description: RBICS industry levels to include in the response. All levels from 1-N will be returned. For example, '3' returns all levels 1,2 and 3. To request all levels, request level=6. Level 1 is returned by default. |Level|Description|Number of Groups| |||| |1|Economomy|14| |2|Sector|37 |3|Sub-Sector|109| |4|Industry Group|366| |5|Inudstry|901| |6|Sub-Industry|1629|
layout: schema
name: levelStructure
properties_list: []
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-rbics-level-structure-schema.json
slug: factset-rbics-level-structure
source_filename: factset-rbics-level-structure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"levelStructure\",\n  \"type\": \"integer\",\n  \"description\": \"RBICS industry levels to include in the response. All levels from 1-N will be returned. For example, '3' returns all levels 1,2 and 3. To request all levels, request level=6. Level 1 is returned by default.\\n  |Level|Description|Number of Groups|\\n  ||||\\n  |1|Economomy|14|\\n  |2|Sector|37\\n  |3|Sub-Sector|109|\\n  |4|Industry Group|366|\\n  |5|Inudstry|901|\\n  |6|Sub-Industry|1629|\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-rbics-level-structure-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: levelStructure
---
