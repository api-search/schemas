---
description: Dimensions are attributes of your data. For example, the dimension city indicates the city from which an event originates. Dimension values in report responses are strings; for example, the city could be "Paris" or "New York". Requests are allowed up to 9 dimensions.
layout: schema
name: Dimension
properties_list:
- description: 'Used to express a dimension which is the result of a formula of multiple dimensions. Example usages: 1) lower_case(dimension) 2) concatenate(dimension1, symbol, dimension2).'
  name: dimensionExpression
  type: object
- description: The name of the dimension. See the [API Dimensions](https://developers.google.com/analytics/devguides/reporting/data/v1/api-schema#dimensions) for the list of dimension names supported by core reporti
  name: name
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/data-api-dimension-schema.json
slug: data-api-dimension
source_filename: data-api-dimension-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-dimension-schema.json\",\n  \"title\": \"Dimension\",\n  \"description\": \"Dimensions are attributes of your data. For example, the dimension city indicates the city from which an event originates. Dimension values in report responses are strings; for example, the city could be \\\"Paris\\\" or \\\"New York\\\". Requests are allowed up to 9 dimensions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dimensionExpression\": {\n      \"description\": \"Used to express a dimension which is the result of a formula of multiple dimensions. Example usages: 1) lower_case(dimension) 2) concatenate(dimension1, symbol, dimension2).\",\n      \"properties\": {\n        \"concatenate\": {\n          \"description\": \"Used to combine dimension values to a single dimension.\",\n          \"properties\"\
  : {\n            \"delimiter\": {\n              \"description\": \"The delimiter placed between dimension names. Delimiters are often single characters such as \\\"|\\\" or \\\",\\\" but can be longer strings. If a dimension value contains the delimiter, both will be present in response with no distinction. For example if dimension 1 value = \\\"US,FR\\\", dimension 2 value = \\\"JP\\\", and delimiter = \\\",\\\", then the response will contain \\\"US,FR,JP\\\".\",\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"dimensionNames\": {\n              \"description\": \"Names of dimensions. The names must refer back to names in the dimensions field of the request.\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"type\": \"array\"\n            }\n          },\n          \"type\": \"object\"\n        },\n        \"lowerCase\": {\n          \"description\": \"Used to convert\
  \ a dimension value to a single case.\",\n          \"properties\": {\n            \"dimensionName\": {\n              \"description\": \"Name of a dimension. The name must refer back to a name in dimensions field of the request.\",\n              \"type\": \"string\",\n              \"example\": \"Example Name\"\n            }\n          },\n          \"type\": \"object\"\n        },\n        \"upperCase\": {\n          \"description\": \"Used to convert a dimension value to a single case.\",\n          \"properties\": {\n            \"dimensionName\": {\n              \"description\": \"Name of a dimension. The name must refer back to a name in dimensions field of the request.\",\n              \"type\": \"string\",\n              \"example\": \"Example Name\"\n            }\n          },\n          \"type\": \"object\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"name\": {\n      \"description\": \"The name of the dimension. See the [API Dimensions](https://developers.google.com/analytics/devguides/reporting/data/v1/api-schema#dimensions)\
  \ for the list of dimension names supported by core reporting methods such as `runReport` and `batchRunReports`. See [Realtime Dimensions](https://developers.google.com/analytics/devguides/reporting/data/v1/realtime-api-schema#dimensions) for the list of dimension names supported by the `runRealtimeReport` method. See [Funnel Dimensions](https://developers.google.com/analytics/devguides/reporting/data/v1/exploration-api-schema#dimensions) for the list of dimension names supported by the `runFunnelReport` method. If `dimensionExpression` is specified, `name` can be any string that you would like within the allowed character set. For example if a `dimensionExpression` concatenates `country` and `city`, you could call that dimension `countryAndCity`. Dimension names that you choose must match the regular expression `^[a-zA-Z0-9_]$`. Dimensions are referenced by `name` in `dimensionFilter`, `orderBys`, `dimensionExpression`, and `pivots`.\",\n      \"type\": \"string\",\n      \"example\"\
  : \"Example Name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/data-api-dimension-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: Dimension
---
