---
description: ClassifyRequest schema from Avalara API
layout: schema
name: ClassifyRequest
properties_list:
- description: Product description for classification
  name: description
  type: string
- description: ISO 3166-1 alpha-2 destination country
  name: destinationCountry
  type: string
- description: ISO 3166-1 alpha-2 origin country
  name: originCountry
  type: string
- description: Additional product attributes
  name: attributes
  type: object
- description: Product identifier
  name: itemCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/hs-code-classification-classify-request-schema.json
slug: hs-code-classification-classify-request
tags:
- Taxes
title: ClassifyRequest
---
