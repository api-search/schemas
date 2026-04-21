---
description: ClassificationResult schema from Avalara API
layout: schema
name: ClassificationResult
properties_list:
- description: ''
  name: itemCode
  type: string
- description: ''
  name: description
  type: string
- description: Classified HS Code
  name: hsCode
  type: string
- description: ''
  name: hsCodeDescription
  type: string
- description: Classification confidence score (0-1)
  name: confidence
  type: number
- description: ''
  name: country
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/item-classification-classification-result-schema.json
slug: item-classification-classification-result
tags:
- Taxes
title: ClassificationResult
---
