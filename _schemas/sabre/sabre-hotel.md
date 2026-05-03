---
description: A hotel property as returned from the Sabre Hotels API
layout: schema
name: Sabre Hotel
properties_list:
- description: Sabre GDS property code
  name: hotelCode
  type: string
- description: Hotel chain code (e.g., HH for Hilton, MC for Marriott)
  name: chainCode
  type: string
- description: Hotel property name
  name: name
  type: string
- description: Normalized star rating
  name: starRating
  type: integer
- description: ''
  name: address
  type: object
- description: ''
  name: coordinates
  type: object
- description: List of hotel amenity codes (OTA HAC list)
  name: amenities
  type: array
- description: ''
  name: images
  type: array
- description: ''
  name: lowestRate
  type: object
- description: ''
  name: availableRooms
  type: array
provider_name: Sabre
provider_slug: sabre
schema_file: json-schema/sabre-hotel-schema.json
slug: sabre-hotel
source_filename: sabre-hotel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.sabre.com/schemas/hotel\",\n  \"title\": \"Sabre Hotel\",\n  \"description\": \"A hotel property as returned from the Sabre Hotels API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hotelCode\": {\n      \"type\": \"string\",\n      \"description\": \"Sabre GDS property code\"\n    },\n    \"chainCode\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel chain code (e.g., HH for Hilton, MC for Marriott)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel property name\"\n    },\n    \"starRating\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 5,\n      \"description\": \"Normalized star rating\"\n    },\n    \"address\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"coordinates\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"\
  number\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        }\n      },\n      \"required\": [\"latitude\", \"longitude\"]\n    },\n    \"amenities\": {\n      \"type\": \"array\",\n      \"description\": \"List of hotel amenity codes (OTA HAC list)\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"enum\": [\"Exterior\", \"Lobby\", \"Room\", \"Pool\", \"Restaurant\", \"Other\"]\n          }\n        },\n        \"required\": [\"url\"]\n      }\n    },\n    \"lowestRate\": {\n      \"$ref\": \"#/$defs/Rate\"\n    },\n    \"availableRooms\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RoomType\"\n      }\n    }\n  },\n  \"required\": [\"hotelCode\", \"name\", \"address\"],\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"stateProvince\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"ISO 3166-1 alpha-2 country code\"\n        }\n      },\n      \"required\": [\"city\", \"countryCode\"]\n    },\n    \"Rate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"number\",\n          \"minimum\": 0\n        },\n        \"currencyCode\": {\n          \"type\": \"string\"\
  ,\n          \"pattern\": \"^[A-Z]{3}$\"\n        },\n        \"rateType\": {\n          \"type\": \"string\",\n          \"enum\": [\"PerNight\", \"Total\"]\n        }\n      },\n      \"required\": [\"amount\", \"currencyCode\"]\n    },\n    \"RoomType\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"roomTypeCode\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"maxOccupancy\": {\n          \"type\": \"integer\",\n          \"minimum\": 1\n        },\n        \"bedConfiguration\": {\n          \"type\": \"string\",\n          \"examples\": [\"King\", \"2 Queens\", \"Twin\"]\n        },\n        \"smokingAllowed\": {\n          \"type\": \"boolean\"\n        },\n        \"ratePlans\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"ratePlanCode\": {\n                \"type\": \"string\"\n          \
  \    },\n              \"ratePlanName\": {\n                \"type\": \"string\"\n              },\n              \"dailyRate\": {\n                \"$ref\": \"#/$defs/Rate\"\n              },\n              \"totalRate\": {\n                \"$ref\": \"#/$defs/Rate\"\n              },\n              \"refundable\": {\n                \"type\": \"boolean\"\n              },\n              \"cancellationPolicy\": {\n                \"type\": \"string\"\n              },\n              \"mealPlan\": {\n                \"type\": \"string\",\n                \"enum\": [\"RoomOnly\", \"BedAndBreakfast\", \"HalfBoard\", \"FullBoard\", \"AllInclusive\"]\n              }\n            },\n            \"required\": [\"ratePlanCode\", \"dailyRate\"]\n          }\n        }\n      },\n      \"required\": [\"roomTypeCode\", \"name\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sabre/refs/heads/main/json-schema/sabre-hotel-schema.json
tags:
- Travel
- GDS
- Airlines
- Hotels
- Car Rental
- Booking
title: Sabre Hotel
---
