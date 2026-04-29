---
description: Age prediction result for a first name from the Agify.io API.
layout: schema
name: AgePrediction
properties_list:
- description: Number of data points used to make the prediction. Higher count indicates greater confidence.
  name: count
  type: integer
- description: The first name that was evaluated.
  name: name
  type: string
- description: Predicted age for the given name. Null if there is insufficient data for a prediction.
  name: age
  type: integer
- description: The ISO 3166-1 alpha-2 country code used for localization, if provided in the request.
  name: country_id
  type: string
provider_name: Agify.io
provider_slug: agify-io
schema_file: json-schema/agify-io-age-prediction-schema.json
slug: agify-io-age-prediction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agify-io/refs/heads/main/json-schema/agify-io-age-prediction-schema.json\",\n  \"title\": \"AgePrediction\",\n  \"description\": \"Age prediction result for a first name from the Agify.io API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of data points used to make the prediction. Higher count indicates greater confidence.\",\n      \"example\": 12345\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The first name that was evaluated.\",\n      \"example\": \"John\"\n    },\n    \"age\": {\n      \"type\": \"integer\",\n      \"description\": \"Predicted age for the given name. Null if there is insufficient data for a prediction.\",\n      \"example\": 42\n    },\n    \"country_id\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The ISO 3166-1 alpha-2 country code used for localization, if provided in the request.\",\n      \"example\": \"US\"\n    }\n  },\n  \"required\": [\"count\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agify-io/refs/heads/main/json-schema/agify-io-age-prediction-schema.json
tags:
- Age Prediction
- Name Analysis
- Demographics
- REST API
title: AgePrediction
---
