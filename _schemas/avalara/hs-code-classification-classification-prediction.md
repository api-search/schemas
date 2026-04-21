---
description: ClassificationPrediction schema from Avalara API
layout: schema
name: ClassificationPrediction
properties_list:
- description: Predicted HS Code
  name: hsCode
  type: string
- description: HS Code description
  name: description
  type: string
- description: Confidence score (0-1)
  name: confidence
  type: number
- description: ''
  name: parentCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/hs-code-classification-classification-prediction-schema.json
slug: hs-code-classification-classification-prediction
tags:
- Taxes
title: ClassificationPrediction
---
