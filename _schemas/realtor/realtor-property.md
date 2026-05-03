---
description: Schema representing a real estate property listing from Realtor.com. Captures listing details, physical characteristics, location, pricing, MLS information, tax and price history, and nearby school data.
layout: schema
name: Realtor.com Property
properties_list:
- description: Unique identifier for the property on Realtor.com.
  name: property_id
  type: string
- description: Unique identifier for the specific listing of the property.
  name: listing_id
  type: string
- description: Current listing status of the property.
  name: status
  type: string
- description: Current listing price in US dollars.
  name: list_price
  type: number
- description: ISO 8601 date-time when the property was listed.
  name: list_date
  type: string
- description: Price at which the property last sold in US dollars.
  name: last_sold_price
  type: number
- description: Date when the property last sold.
  name: last_sold_date
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: location
  type: object
- description: Array of property photo objects.
  name: photos
  type: array
- description: Tags describing property features such as garage, pool, or waterfront.
  name: tags
  type: array
- description: ''
  name: mls
  type: object
- description: Historical price changes for the property.
  name: price_history
  type: array
- description: Property tax assessment history.
  name: tax_history
  type: array
- description: Nearby schools with ratings and distance information.
  name: schools
  type: array
provider_name: realtor
provider_slug: realtor
schema_file: json-schema/realtor-property-schema.json
slug: realtor-property
source_filename: realtor-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://realtor.com/schemas/realtor/property.json\",\n  \"title\": \"Realtor.com Property\",\n  \"description\": \"Schema representing a real estate property listing from Realtor.com. Captures listing details, physical characteristics, location, pricing, MLS information, tax and price history, and nearby school data.\",\n  \"type\": \"object\",\n  \"required\": [\"property_id\"],\n  \"properties\": {\n    \"property_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the property on Realtor.com.\"\n    },\n    \"listing_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the specific listing of the property.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current listing status of the property.\",\n      \"enum\": [\"for_sale\", \"for_rent\", \"recently_sold\", \"off_market\", \"ready_to_build\"\
  ]\n    },\n    \"list_price\": {\n      \"type\": \"number\",\n      \"description\": \"Current listing price in US dollars.\",\n      \"minimum\": 0\n    },\n    \"list_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 date-time when the property was listed.\"\n    },\n    \"last_sold_price\": {\n      \"type\": \"number\",\n      \"description\": \"Price at which the property last sold in US dollars.\",\n      \"minimum\": 0\n    },\n    \"last_sold_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the property last sold.\"\n    },\n    \"description\": {\n      \"$ref\": \"#/$defs/PropertyDescription\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/Location\"\n    },\n    \"photos\": {\n      \"type\": \"array\",\n      \"description\": \"Array of property photo objects.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Photo\"\n      }\n    },\n    \"tags\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"Tags describing property features such as garage, pool, or waterfront.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"mls\": {\n      \"$ref\": \"#/$defs/MlsInfo\"\n    },\n    \"price_history\": {\n      \"type\": \"array\",\n      \"description\": \"Historical price changes for the property.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PriceHistoryEntry\"\n      }\n    },\n    \"tax_history\": {\n      \"type\": \"array\",\n      \"description\": \"Property tax assessment history.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TaxHistoryEntry\"\n      }\n    },\n    \"schools\": {\n      \"type\": \"array\",\n      \"description\": \"Nearby schools with ratings and distance information.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/NearbySchool\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"PropertyDescription\": {\n      \"type\": \"object\",\n      \"description\": \"Detailed property\
  \ characteristics and features.\",\n      \"properties\": {\n        \"beds\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of bedrooms.\",\n          \"minimum\": 0\n        },\n        \"baths\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of bathrooms.\",\n          \"minimum\": 0\n        },\n        \"baths_full\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of full bathrooms.\",\n          \"minimum\": 0\n        },\n        \"baths_half\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of half bathrooms.\",\n          \"minimum\": 0\n        },\n        \"sqft\": {\n          \"type\": \"integer\",\n          \"description\": \"Interior living area in square feet.\",\n          \"minimum\": 0\n        },\n        \"lot_sqft\": {\n          \"type\": \"integer\",\n          \"description\": \"Lot area in square feet.\",\n          \"minimum\": 0\n        },\n    \
  \    \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Property type classification.\",\n          \"enum\": [\"single_family\", \"multi_family\", \"condo\", \"townhome\", \"mobile\", \"land\", \"farm\"]\n        },\n        \"year_built\": {\n          \"type\": \"integer\",\n          \"description\": \"Year the property was constructed.\",\n          \"minimum\": 1600,\n          \"maximum\": 2030\n        },\n        \"garage\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of garage spaces.\",\n          \"minimum\": 0\n        },\n        \"stories\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of stories in the property.\",\n          \"minimum\": 0\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Free-text description of the property from the listing.\"\n        }\n      }\n    },\n    \"Location\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Geographic location and address information for the property.\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"object\",\n          \"description\": \"Structured address components.\",\n          \"properties\": {\n            \"line\": {\n              \"type\": \"string\",\n              \"description\": \"Street address line.\"\n            },\n            \"city\": {\n              \"type\": \"string\",\n              \"description\": \"City name.\"\n            },\n            \"state_code\": {\n              \"type\": \"string\",\n              \"description\": \"Two-letter state abbreviation.\",\n              \"pattern\": \"^[A-Z]{2}$\",\n              \"minLength\": 2,\n              \"maxLength\": 2\n            },\n            \"state\": {\n              \"type\": \"string\",\n              \"description\": \"Full state name.\"\n            },\n            \"postal_code\": {\n              \"type\": \"string\",\n              \"description\": \"\
  Five-digit ZIP code.\",\n              \"pattern\": \"^[0-9]{5}$\"\n            },\n            \"county\": {\n              \"type\": \"string\",\n              \"description\": \"County name.\"\n            },\n            \"coordinate\": {\n              \"type\": \"object\",\n              \"description\": \"Geographic coordinates.\",\n              \"properties\": {\n                \"lat\": {\n                  \"type\": \"number\",\n                  \"description\": \"Latitude.\",\n                  \"minimum\": -90,\n                  \"maximum\": 90\n                },\n                \"lon\": {\n                  \"type\": \"number\",\n                  \"description\": \"Longitude.\",\n                  \"minimum\": -180,\n                  \"maximum\": 180\n                }\n              }\n            }\n          }\n        },\n        \"neighborhood_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the neighborhood.\"\n        }\n     \
  \ }\n    },\n    \"Photo\": {\n      \"type\": \"object\",\n      \"description\": \"A property photo.\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the property photo.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Caption or description of the photo.\"\n        }\n      }\n    },\n    \"MlsInfo\": {\n      \"type\": \"object\",\n      \"description\": \"MLS listing information.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"MLS listing identifier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"MLS name.\"\n        },\n        \"abbreviation\": {\n          \"type\": \"string\",\n          \"description\": \"MLS abbreviation.\"\n        }\n      }\n    },\n    \"PriceHistoryEntry\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"A single entry in the property price history.\",\n      \"properties\": {\n        \"date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Date of the price event.\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\": \"Price in US dollars at the time of the event.\",\n          \"minimum\": 0\n        },\n        \"event\": {\n          \"type\": \"string\",\n          \"description\": \"Type of price event.\",\n          \"enum\": [\"listed\", \"sold\", \"price_changed\", \"delisted\", \"pending\"]\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"Data source for the price record.\"\n        }\n      }\n    },\n    \"TaxHistoryEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A single entry in the property tax assessment history.\",\n      \"properties\": {\n        \"year\": {\n          \"type\": \"\
  integer\",\n          \"description\": \"Tax assessment year.\"\n        },\n        \"tax\": {\n          \"type\": \"number\",\n          \"description\": \"Annual property tax amount in US dollars.\",\n          \"minimum\": 0\n        },\n        \"assessment\": {\n          \"type\": \"object\",\n          \"description\": \"Property tax assessment breakdown.\",\n          \"properties\": {\n            \"total\": {\n              \"type\": \"number\",\n              \"description\": \"Total assessed value in US dollars.\",\n              \"minimum\": 0\n            },\n            \"land\": {\n              \"type\": \"number\",\n              \"description\": \"Assessed land value in US dollars.\",\n              \"minimum\": 0\n            },\n            \"building\": {\n              \"type\": \"number\",\n              \"description\": \"Assessed building value in US dollars.\",\n              \"minimum\": 0\n            }\n          }\n        }\n      }\n    },\n    \"NearbySchool\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Information about a school near the property.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the school.\"\n        },\n        \"education_levels\": {\n          \"type\": \"array\",\n          \"description\": \"Grade levels served such as elementary, middle, or high.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"rating\": {\n          \"type\": \"integer\",\n          \"description\": \"School rating on a scale of 1 to 10.\",\n          \"minimum\": 1,\n          \"maximum\": 10\n        },\n        \"distance_in_miles\": {\n          \"type\": \"number\",\n          \"description\": \"Distance from the property in miles.\",\n          \"minimum\": 0\n        },\n        \"funding_type\": {\n          \"type\": \"string\",\n          \"description\": \"Funding type of the school.\",\n          \"enum\"\
  : [\"public\", \"private\", \"charter\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/json-schema/realtor-property-schema.json
tags: []
title: Realtor.com Property
---
