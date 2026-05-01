---
description: A pricing agreement for a discounted rate for a specific outbound bandwidth that your MediaConnect account will use each month over a specific time period. The discounted rate in the reservation applies to outbound bandwidth for all flows from your account until your account reaches the amount of bandwidth in your reservation. If you use more outbound bandwidth than the agreed upon amount in a single month, the overage is charged at the on-demand rate.
layout: schema
name: Reservation
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
  name: End
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
  name: ReservationArn
  type: object
- description: ''
  name: ReservationName
  type: object
- description: ''
  name: ReservationState
  type: object
- description: ''
  name: ResourceSpecification
  type: object
- description: ''
  name: Start
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-reservation-schema.json
slug: mediaconnect-api-reservation
source_filename: mediaconnect-api-reservation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-reservation-schema.json\",\n  \"title\": \"Reservation\",\n  \"description\": \"A pricing agreement for a discounted rate for a specific outbound bandwidth that your MediaConnect account will use each month over a specific time period. The discounted rate in the reservation applies to outbound bandwidth for all flows from your account until your account reaches the amount of bandwidth in your reservation. If you use more outbound bandwidth than the agreed upon amount in a single month, the overage is charged at the on-demand rate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrencyCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currencyCode\"\n        \
  \  },\n          \"description\": \"The type of currency that is used for billing. The currencyCode used for your reservation is US dollars.\"\n        }\n      ]\n    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"duration\"\n          },\n          \"description\": \"The length of time that this reservation is active. MediaConnect defines this value in the offering.\"\n        }\n      ]\n    },\n    \"DurationUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"durationUnits\"\n          },\n          \"description\": \"The unit of measurement for the duration of the reservation. MediaConnect defines this value in the offering.\"\n        }\n      ]\n    },\n    \"End\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"end\"\n          },\n          \"description\": \"The day and time that this reservation expires. This value is calculated based on the start date and time that you set and the offering's duration.\"\n        }\n      ]\n    },\n    \"OfferingArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offeringArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) that MediaConnect assigns to the offering.\"\n        }\n      ]\n    },\n    \"OfferingDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offeringDescription\"\n          },\n          \"description\": \"A description of the offering. MediaConnect defines this value in the offering.\"\n        }\n      ]\n \
  \   },\n    \"PricePerUnit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pricePerUnit\"\n          },\n          \"description\": \"The cost of a single unit. This value, in combination with priceUnits, makes up the rate. MediaConnect defines this value in the offering.\"\n        }\n      ]\n    },\n    \"PriceUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PriceUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"priceUnits\"\n          },\n          \"description\": \"The unit of measurement that is used for billing. This value, in combination with pricePerUnit, makes up the rate. MediaConnect defines this value in the offering.\"\n        }\n      ]\n    },\n    \"ReservationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"reservationArn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) that MediaConnect assigns to the reservation when you purchase an offering.\"\n        }\n      ]\n    },\n    \"ReservationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservationName\"\n          },\n          \"description\": \"The name that you assigned to the reservation when you purchased the offering.\"\n        }\n      ]\n    },\n    \"ReservationState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reservationState\"\n          },\n          \"description\": \"The status of your reservation.\"\n        }\n      ]\n    },\n    \"ResourceSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceSpecification\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceSpecification\"\n          },\n          \"description\": \"A definition of the amount of outbound bandwidth that you would be reserving if you purchase the offering. MediaConnect defines the values that make up the resourceSpecification in the offering.\"\n        }\n      ]\n    },\n    \"Start\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"start\"\n          },\n          \"description\": \"The day and time that the reservation becomes active. You set this value when you purchase the offering.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrencyCode\",\n    \"ReservationState\",\n    \"OfferingArn\",\n    \"ReservationArn\",\n    \"Start\",\n    \"OfferingDescription\",\n    \"ReservationName\",\n    \"End\",\n    \"Duration\",\n    \"DurationUnits\",\n    \"PricePerUnit\",\n\
  \    \"ResourceSpecification\",\n    \"PriceUnits\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-reservation-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: Reservation
---
