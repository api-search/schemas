---
description: AddressResolutionModel schema from Avalara API
layout: schema
name: AddressResolutionModel
properties_list:
- description: ''
  name: address
  type: object
- description: ''
  name: validatedAddresses
  type: array
- description: ''
  name: coordinates
  type: object
- description: ''
  name: resolutionQuality
  type: string
- description: ''
  name: taxAuthorities
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-address-resolution-model-schema.json
slug: avatax-rest-address-resolution-model
source_filename: avatax-rest-address-resolution-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-address-resolution-model-schema.json\",\n  \"title\": \"AddressResolutionModel\",\n  \"description\": \"AddressResolutionModel schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"$ref\": \"#/components/schemas/AddressInfo\"\n    },\n    \"validatedAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AddressInfo\"\n      }\n    },\n    \"coordinates\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\"\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\"\n        }\n      }\n    },\n    \"resolutionQuality\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\n        \"NotCoded\",\n        \"External\",\n        \"CountryCentroid\",\n        \"RegionCentroid\",\n        \"PartialCentroid\",\n        \"PostalCentroidGood\",\n        \"PostalCentroidBetter\",\n        \"PostalCentroidBest\",\n        \"Intersection\",\n        \"Interpolated\",\n        \"Rooftop\"\n      ]\n    },\n    \"taxAuthorities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaxAuthorityInfo\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-address-resolution-model-schema.json
tags:
- Taxes
title: AddressResolutionModel
---
