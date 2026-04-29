---
description: A savings plan that reserves a certain amount of outbound bandwidth usage at a discounted rate each month over a period of time.
layout: schema
name: Offering
properties_list:
- description: ''
  name: CurrencyCode
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: DurationUnits
  type: object
- description: ''
  name: OfferingArn
  type: object
- description: ''
  name: OfferingDescription
  type: object
- description: ''
  name: PricePerUnit
  type: object
- description: ''
  name: PriceUnits
  type: object
- description: ''
  name: ResourceSpecification
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-offering-schema.json
slug: mediaconnect-api-offering
source_filename: mediaconnect-api-offering-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-offering-schema.json\",\n  \"title\": \"Offering\",\n  \"description\": \"A savings plan that reserves a certain amount of outbound bandwidth usage at a discounted rate each month over a period of time.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrencyCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currencyCode\"\n          },\n          \"description\": \"The type of currency that is used for billing. The currencyCode used for all reservations is US dollars.\"\n        }\n      ]\n    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n          \
  \  \"name\": \"duration\"\n          },\n          \"description\": \"The length of time that your reservation would be active.\"\n        }\n      ]\n    },\n    \"DurationUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"durationUnits\"\n          },\n          \"description\": \"The unit of measurement for the duration of the offering.\"\n        }\n      ]\n    },\n    \"OfferingArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offeringArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) that MediaConnect assigns to the offering.\"\n        }\n      ]\n    },\n    \"OfferingDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"offeringDescription\"\n          },\n          \"description\": \"A description of the offering.\"\n        }\n      ]\n    },\n    \"PricePerUnit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pricePerUnit\"\n          },\n          \"description\": \"The cost of a single unit. This value, in combination with priceUnits, makes up the rate.\"\n        }\n      ]\n    },\n    \"PriceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PriceUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"priceUnits\"\n          },\n          \"description\": \"The unit of measurement that is used for billing. This value, in combination with pricePerUnit, makes up the rate.\"\n        }\n      ]\n    },\n    \"ResourceSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceSpecification\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceSpecification\"\n          },\n          \"description\": \"A definition of the amount of outbound bandwidth that you would be reserving if you purchase the offering.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrencyCode\",\n    \"OfferingArn\",\n    \"OfferingDescription\",\n    \"DurationUnits\",\n    \"Duration\",\n    \"PricePerUnit\",\n    \"ResourceSpecification\",\n    \"PriceUnits\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-offering-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: Offering
---
