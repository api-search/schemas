---
description: ''
layout: schema
name: SearchOptions
properties_list:
- description: The acquisition date or the acquisition date range.
  name: acquisitionDate
  type: object
- description: The geographic search area expressed as a bbox string (decimal degrees values separated by a comma). Values are min lon,min lat, max lon, max lat.
  name: bbox
  type: string
- description: The cloud cover percentage or the cloud cover percentage range.
  name: cloudCover
  type: object
- description: The commercial reference.
  name: commercialReference
  type: string
- description: The constellation or constellation list (comma separated list). Possible values will be described in a future endpoint (*/api/v1/opensearch/domains/constellation*).
  name: constellation
  type: string
- description: ''
  name: correlationId
  type: object
- description: ''
  name: expirationDate
  type: object
- description: The geographic search area.
  name: geometry
  type: object
- description: ''
  name: id
  type: object
- description: The incident angle or the incident angle range in degree.
  name: incidenceAngle
  type: object
- description: The maximum number of items that the response can contain.
  name: itemsPerPage
  type: integer
- description: The requested page
  name: page
  type: integer
- description: The parent identifier (identified as sourceId in other catalogs)
  name: parentIdentifier
  type: string
- description: The platform or platform list (comma separated list). Possible values will be described in a future endpoint (*/api/v1/opensearch/domains/platform*).
  name: platform
  type: string
- description: The product type or product type list (comma separated list). Possible values will be described in a future endpoint (*/api/v1/opensearch/domains/productType*).
  name: productType
  type: string
- description: The production status or production status list (comma separated list).
  name: productionStatus
  type: string
- description: The publication date or the publication date range.
  name: publicationDate
  type: object
- description: A generic query parameter, will search in productType and title. Search is in "contains" mode.
  name: q
  type: string
- description: The resolution or the resolution range in meters.
  name: resolution
  type: object
- description: The snow cover percentage or the snow cover percentage range.
  name: snowCover
  type: object
- description: The order strategy for the items. Accepted values are all opensearch attributes separated by a comma. Minus sign can be used to sort descending on the attribute. Otherwise the sort is ascending.
  name: sortBy
  type: string
- description: The product identifier inside original referential
  name: sourceIdentifier
  type: string
- description: The workspace id/name or workspace id/name list (comma separated list)
  name: workspace
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-search-options-schema.json
slug: oneatlas-search-options
source_filename: oneatlas-search-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-options-schema.json\",\n  \"title\": \"SearchOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acquisitionDate\": {\n      \"description\": \"The acquisition date or the acquisition date range.\",\n      \"oneOf\": [\n        {\n          \"description\": \"The acquisition date.\",\n          \"example\": \"2017-08-29T00:00:00Z\",\n          \"format\": \"date-time\",\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The acquisition dates range.\\n\\nRanges are expressed as follow:\\n  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\n  - End with `[` means *end\
  \ value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"[2017-08-29T00:00:00Z\",\n          \"format\": \"date-time-range\",\n          \"type\": \"string\"\n        }\n      ]\n    },\n    \"bbox\": {\n      \"description\": \"The geographic search area expressed as a bbox string (decimal degrees values  separated by a comma). Values are min lon,min lat, max lon, max lat.\",\n      \"example\": \"1.8292,48.5821,2.9718,49.0811\",\n      \"type\": \"string\"\n    },\n    \"cloudCover\": {\n      \"description\": \"The cloud cover percentage or the cloud cover percentage range.\",\n      \"oneOf\": [\n        {\n          \"description\": \"The cloud cover percentage from 0 to 100.\",\n          \"example\": \"5\",\n          \"format\": \"float\",\n          \"type\": \"number\"\n        },\n        {\n          \"description\": \"The cloud cover percentages range\\n\\nRanges are expressed as follow:\\n  - Comma to separate start value from end\
  \ value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"5[\",\n          \"format\": \"float-range\",\n          \"type\": \"string\"\n        }\n      ]\n    },\n    \"commercialReference\": {\n      \"description\": \"The commercial reference.\",\n      \"example\": \"SO17011862-6\",\n      \"type\": \"string\"\n    },\n    \"constellation\": {\n      \"description\": \"The constellation or constellation list (comma separated list). Possible values will be described in a future endpoint (*/api/v1/opensearch/domains/constellation*).\",\n      \"example\": \"PHR,Sentinel\",\n      \"type\": \"string\"\n    },\n    \"correlationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n \
  \       {\n          \"description\": \"The correlation id or correlation id list (comma separated list). The correlation id is used to trace features sharing the same `X-Ads-Correlation-Id` header when ingested or processed.\"\n        }\n      ]\n    },\n    \"expirationDate\": {\n      \"oneOf\": [\n        {\n          \"description\": \"Date of deletion of the data in the platform and deletion of the metadata item if no other prodution status is defined.\",\n          \"example\": \"2017-08-29T00:00:00Z\",\n          \"format\": \"date-time\",\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Dates range of deletion of the data in the platform and deletion of the metadata item if no other prodution status is defined.\\n\\nRanges are expressed as follow:\\n  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with\
  \ `]` means *start value is excluded*\\n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"[2017-08-29T00:00:00Z\",\n          \"format\": \"date-time-range\",\n          \"type\": \"string\"\n        }\n      ]\n    },\n    \"geometry\": {\n      \"description\": \"The geographic search area.\",\n      \"example\": \"POLYGON((1 1,5 1,5 5,1 5,1 1))\",\n      \"oneOf\": [\n        {\n          \"example\": \"POLYGON((1 1,5 1,5 5,1 5,1 1))\",\n          \"format\": \"WKT\",\n          \"type\": \"string\"\n        },\n        {\n          \"example\": \"{type: \\\"Polygon\\\", coordinates: [[1, 1], [5, 1], [5, 5], [1, 5], [1, 1]]}\",\n          \"format\": \"geojson\",\n          \"type\": \"string\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/GeojsonGeometry\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n\
  \        {\n          \"description\": \"The item id or item id list (comma separated list).\"\n        }\n      ]\n    },\n    \"incidenceAngle\": {\n      \"description\": \"The incident angle or the incident angle range in degree.\",\n      \"oneOf\": [\n        {\n          \"description\": \"The incident angle in degree.\",\n          \"example\": \"5.1542\",\n          \"format\": \"float\",\n          \"type\": \"number\"\n        },\n        {\n          \"description\": \"The incident angle range in degree.\\n\\nRanges are expressed as follow:\\n  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"[80,100]\",\n          \"format\": \"float-range\",\n          \"type\": \"string\"\
  \n        }\n      ]\n    },\n    \"itemsPerPage\": {\n      \"default\": 50,\n      \"description\": \"The maximum number of items that the response can contain.\",\n      \"example\": 100,\n      \"format\": \"int32\",\n      \"maximum\": 500,\n      \"type\": \"integer\"\n    },\n    \"page\": {\n      \"default\": 1,\n      \"description\": \"The requested page\",\n      \"example\": 1,\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"parentIdentifier\": {\n      \"description\": \"The parent identifier (identified as sourceId in other catalogs)\",\n      \"example\": \"DS_SPOT7_201412071054567_FR1_FR1_FR1_FR1_W003N39_01709\",\n      \"type\": \"string\"\n    },\n    \"platform\": {\n      \"description\": \"The platform or platform list (comma separated list). Possible values will be described in a future endpoint (*/api/v1/opensearch/domains/platform*).\",\n      \"example\": \"PHR1A\",\n      \"type\": \"string\"\n    },\n    \"productType\": {\n      \"\
  description\": \"The product type or product type list (comma separated list). Possible values will be described in a future endpoint (*/api/v1/opensearch/domains/productType*).\",\n      \"example\": \"changeDetectionReport,mono\",\n      \"type\": \"string\"\n    },\n    \"productionStatus\": {\n      \"description\": \"The production status or production status list (comma separated list).\",\n      \"enum\": [\n        \"IN_CLOUD\",\n        \"ARCHIVED\"\n      ],\n      \"example\": \"IN_CLOUD\",\n      \"type\": \"string\"\n    },\n    \"publicationDate\": {\n      \"description\": \"The publication date or the publication date range.\",\n      \"oneOf\": [\n        {\n          \"description\": \"The publication date.\",\n          \"example\": \"2017-08-29T00:00:00Z\",\n          \"format\": \"date-time\",\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The publication dates range.\\n\\nRanges are expressed as follow:\\n  - Comma to separate\
  \ start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"[2017-08-29T00:00:00Z\",\n          \"format\": \"date-time-range\",\n          \"type\": \"string\"\n        }\n      ]\n    },\n    \"q\": {\n      \"description\": \"A generic query parameter, will search in productType and title. Search is in \\\"contains\\\" mode.\",\n      \"example\": \"PHR\",\n      \"type\": \"string\"\n    },\n    \"resolution\": {\n      \"description\": \"The resolution or the resolution range in meters.\",\n      \"oneOf\": [\n        {\n          \"description\": \"The resolution in meters.\",\n          \"example\": \"10\",\n          \"format\": \"float\",\n          \"type\": \"number\"\n        },\n        {\n        \
  \  \"description\": \"The resolution range in meters.\\n\\nRanges are expressed as follow:\\n  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"10]\",\n          \"format\": \"float-range\",\n          \"type\": \"number\"\n        }\n      ]\n    },\n    \"snowCover\": {\n      \"description\": \"The snow cover percentage or the snow cover percentage range.\",\n      \"oneOf\": [\n        {\n          \"description\": \"The snow cover percentage from 0 to 100.\",\n          \"example\": \"5\",\n          \"format\": \"float\",\n          \"type\": \"number\"\n        },\n        {\n          \"description\": \"The snow cover percentage range.\\n\\nRanges are expressed as follow:\\n\
  \  - Comma to separate start value from end value\\n  - Start value or end value can be omitted (it means values are infinite)\\n  - Start with `[` means *start value is included*\\n  - Start with `]` means *start value is excluded*\\n  - End with `[` means *end value is included*\\n  - End with `]` means *end value is excluded*\",\n          \"example\": \"5[\",\n          \"format\": \"float-range\",\n          \"type\": \"string\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"default\": \"-acquisitionDate,cloudCover\",\n      \"description\": \"The order strategy for the items.\\n\\nAccepted values are all opensearch attributes separated by a comma. Minus sign can be used to sort descending on the attribute. Otherwise the sort is ascending.\",\n      \"example\": \"-acquisitionDate,cloudCover\",\n      \"type\": \"string\"\n    },\n    \"sourceIdentifier\": {\n      \"description\": \"The product identifier inside original referential\",\n      \"example\": \"DS_SPOT7_201412071054567_FR1_FR1_FR1_FR1_W003N39_01709\"\
  ,\n      \"type\": \"string\"\n    },\n    \"workspace\": {\n      \"description\": \"The workspace id/name or workspace id/name list (comma separated list)\",\n      \"example\": \"dc143057-3457-47b3-af19-4ef8d26d2064\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-search-options-schema.json
tags:
- Imagery
- Satellites
title: SearchOptions
---
