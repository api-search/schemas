---
description: Request available SASB Spotlights data fields to be included in the response. Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included. |field|description| ||| |fsymId|Factset Regional Security Identifier| |orgId|Unique identifier assigned that is applied on an organization level| |spotlightId|Unique identifier assigned identifying a Spotlight ESG event that is detected at the company level, within a single category.| |requestId|Identifier that was used for the request.| |primaryArticleHeadline|Headline of primary Spotlight article.| |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start date.|
layout: schema
name: fieldsSasbSpotlights
properties_list: []
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-esg-fields-sasb-spotlights-schema.json
slug: factset-esg-fields-sasb-spotlights
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"fieldsSasbSpotlights\",\n  \"type\": \"array\",\n  \"description\": \"Request available SASB Spotlights data fields to be included in the response.\\n Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.\\n \\n  |field|description|\\n  |||\\n  |fsymId|Factset Regional Security Identifier|\\n  |orgId|Unique identifier assigned that is applied on an organization level|\\n  |spotlightId|Unique identifier assigned identifying a Spotlight ESG event that is detected at the company level, within a single category.|\\n  |requestId|Identifier that was used for the request.|\\n  |primaryArticleHeadline|Headline of primary Spotlight article.| \\n  |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start date.|\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-esg-fields-sasb-spotlights-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: fieldsSasbSpotlights
---
