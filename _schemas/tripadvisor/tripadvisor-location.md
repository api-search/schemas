---
description: A Tripadvisor location representing a hotel, restaurant, or attraction with comprehensive details including address, rating, reviews, and photos.
layout: schema
name: Tripadvisor Location
properties_list:
- description: The unique Tripadvisor identifier for this location.
  name: location_id
  type: string
- description: The display name of the location.
  name: name
  type: string
- description: A detailed text description of the location.
  name: description
  type: string
- description: The URL of the location's page on Tripadvisor.
  name: web_url
  type: string
- description: ''
  name: address_obj
  type: object
- description: Array of parent geographic locations in the hierarchy.
  name: ancestors
  type: array
- description: The latitude coordinate of the location.
  name: latitude
  type: string
- description: The longitude coordinate of the location.
  name: longitude
  type: string
- description: The timezone of the location (e.g., America/New_York).
  name: timezone
  type: string
- description: The phone number of the location.
  name: phone
  type: string
- description: The official website URL of the location.
  name: website
  type: string
- description: ''
  name: ranking_data
  type: object
- description: The overall rating on a scale of 1.0 to 5.0.
  name: rating
  type: string
- description: URL of the rating bubble image.
  name: rating_image_url
  type: string
- description: The total number of reviews for this location.
  name: num_reviews
  type: string
- description: Breakdown of review counts by rating level (1-5).
  name: review_rating_count
  type: object
- description: The total number of photos available for this location.
  name: photo_count
  type: string
- description: The price level indicator.
  name: price_level
  type: string
- description: ''
  name: category
  type: object
- description: Array of subcategory classifications for this location.
  name: subcategory
  type: array
- description: Array of cuisine types for restaurant locations.
  name: cuisine
  type: array
- description: ''
  name: hours
  type: object
- description: Array of category groups this location belongs to.
  name: groups
  type: array
- description: Array of trip type ratings for this location.
  name: trip_types
  type: array
- description: Array of awards received by this location.
  name: awards
  type: array
provider_name: tripadvisor
provider_slug: tripadvisor
schema_file: json-schema/tripadvisor-location-schema.json
slug: tripadvisor-location
source_filename: tripadvisor-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer-tripadvisor.com/schemas/tripadvisor/location.json\",\n  \"title\": \"Tripadvisor Location\",\n  \"description\": \"A Tripadvisor location representing a hotel, restaurant, or attraction with comprehensive details including address, rating, reviews, and photos.\",\n  \"type\": \"object\",\n  \"required\": [\"location_id\", \"name\"],\n  \"properties\": {\n    \"location_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Tripadvisor identifier for this location.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the location.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed text description of the location.\"\n    },\n    \"web_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the location's page on Tripadvisor.\"\
  \n    },\n    \"address_obj\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"ancestors\": {\n      \"type\": \"array\",\n      \"description\": \"Array of parent geographic locations in the hierarchy.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Ancestor\"\n      }\n    },\n    \"latitude\": {\n      \"type\": \"string\",\n      \"description\": \"The latitude coordinate of the location.\",\n      \"pattern\": \"^-?\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"longitude\": {\n      \"type\": \"string\",\n      \"description\": \"The longitude coordinate of the location.\",\n      \"pattern\": \"^-?\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"The timezone of the location (e.g., America/New_York).\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the location.\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\":\
  \ \"The official website URL of the location.\"\n    },\n    \"ranking_data\": {\n      \"$ref\": \"#/$defs/RankingData\"\n    },\n    \"rating\": {\n      \"type\": \"string\",\n      \"description\": \"The overall rating on a scale of 1.0 to 5.0.\",\n      \"pattern\": \"^[1-5](\\\\.[05])?$\"\n    },\n    \"rating_image_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the rating bubble image.\"\n    },\n    \"num_reviews\": {\n      \"type\": \"string\",\n      \"description\": \"The total number of reviews for this location.\",\n      \"pattern\": \"^\\\\d+$\"\n    },\n    \"review_rating_count\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of review counts by rating level (1-5).\",\n      \"properties\": {\n        \"1\": { \"type\": \"string\", \"description\": \"Count of 1-star reviews.\" },\n        \"2\": { \"type\": \"string\", \"description\": \"Count of 2-star reviews.\" },\n        \"3\": { \"type\": \"\
  string\", \"description\": \"Count of 3-star reviews.\" },\n        \"4\": { \"type\": \"string\", \"description\": \"Count of 4-star reviews.\" },\n        \"5\": { \"type\": \"string\", \"description\": \"Count of 5-star reviews.\" }\n      }\n    },\n    \"photo_count\": {\n      \"type\": \"string\",\n      \"description\": \"The total number of photos available for this location.\",\n      \"pattern\": \"^\\\\d+$\"\n    },\n    \"price_level\": {\n      \"type\": \"string\",\n      \"description\": \"The price level indicator.\",\n      \"enum\": [\"$\", \"$$\", \"$$ - $$$\", \"$$$\", \"$$$$\"]\n    },\n    \"category\": {\n      \"$ref\": \"#/$defs/Tag\"\n    },\n    \"subcategory\": {\n      \"type\": \"array\",\n      \"description\": \"Array of subcategory classifications for this location.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    },\n    \"cuisine\": {\n      \"type\": \"array\",\n      \"description\": \"Array of cuisine types for restaurant locations.\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    },\n    \"hours\": {\n      \"$ref\": \"#/$defs/Hours\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"Array of category groups this location belongs to.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Group\"\n      }\n    },\n    \"trip_types\": {\n      \"type\": \"array\",\n      \"description\": \"Array of trip type ratings for this location.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TripType\"\n      }\n    },\n    \"awards\": {\n      \"type\": \"array\",\n      \"description\": \"Array of awards received by this location.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Award\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"The physical address of a location.\",\n      \"properties\": {\n        \"street1\": {\n          \"type\": \"string\",\n          \"description\": \"The primary street address\
  \ line.\"\n        },\n        \"street2\": {\n          \"type\": \"string\",\n          \"description\": \"The secondary street address line.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"The city name.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The state or province name.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The country name.\"\n        },\n        \"postalcode\": {\n          \"type\": \"string\",\n          \"description\": \"The postal or ZIP code.\"\n        },\n        \"address_string\": {\n          \"type\": \"string\",\n          \"description\": \"The full formatted address as a single string.\"\n        }\n      }\n    },\n    \"Ancestor\": {\n      \"type\": \"object\",\n      \"description\": \"A parent geographic location in the location hierarchy.\",\n      \"properties\": {\n        \"level\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The level in the geographic hierarchy (e.g., City, Region, Country).\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the ancestor location.\"\n        },\n        \"location_id\": {\n          \"type\": \"string\",\n          \"description\": \"The Tripadvisor location ID of the ancestor.\"\n        }\n      }\n    },\n    \"RankingData\": {\n      \"type\": \"object\",\n      \"description\": \"Ranking information for the location within its category and geography.\",\n      \"properties\": {\n        \"geo_location_id\": {\n          \"type\": \"string\",\n          \"description\": \"The Tripadvisor ID of the geographic area for ranking.\"\n        },\n        \"ranking_string\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable ranking string.\"\n        },\n        \"geo_location_name\": {\n          \"type\": \"string\",\n  \
  \        \"description\": \"The name of the geographic area for ranking.\"\n        },\n        \"ranking_out_of\": {\n          \"type\": \"string\",\n          \"description\": \"The total number of locations in the ranking category.\"\n        },\n        \"ranking\": {\n          \"type\": \"string\",\n          \"description\": \"The numeric rank position.\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A category or classification tag.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the tag.\"\n        },\n        \"localized_name\": {\n          \"type\": \"string\",\n          \"description\": \"The localized display name of the tag.\"\n        }\n      }\n    },\n    \"Group\": {\n      \"type\": \"object\",\n      \"description\": \"A category group with associated sub-categories.\",\n      \"properties\": {\n        \"name\": {\n          \"\
  type\": \"string\",\n          \"description\": \"The name of the group.\"\n        },\n        \"localized_name\": {\n          \"type\": \"string\",\n          \"description\": \"The localized name of the group.\"\n        },\n        \"categories\": {\n          \"type\": \"array\",\n          \"description\": \"Array of category tags within this group.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Tag\"\n          }\n        }\n      }\n    },\n    \"TripType\": {\n      \"type\": \"object\",\n      \"description\": \"Rating data for a specific type of trip.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The trip type name (e.g., business, couples, family).\"\n        },\n        \"localized_name\": {\n          \"type\": \"string\",\n          \"description\": \"The localized trip type name.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The count of reviews\
  \ for this trip type.\"\n        }\n      }\n    },\n    \"Award\": {\n      \"type\": \"object\",\n      \"description\": \"An award or recognition received by the location.\",\n      \"properties\": {\n        \"award_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of award.\"\n        },\n        \"year\": {\n          \"type\": \"string\",\n          \"description\": \"The year the award was given.\",\n          \"pattern\": \"^\\\\d{4}$\"\n        },\n        \"images\": {\n          \"type\": \"object\",\n          \"description\": \"Image URLs for the award badge.\",\n          \"properties\": {\n            \"small\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL for the small award image.\"\n            },\n            \"large\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL for the large award image.\"\n      \
  \      }\n          }\n        },\n        \"display_name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the award.\"\n        }\n      }\n    },\n    \"Hours\": {\n      \"type\": \"object\",\n      \"description\": \"Operating hours information for the location.\",\n      \"properties\": {\n        \"periods\": {\n          \"type\": \"array\",\n          \"description\": \"Array of time periods when the location is open.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"open\": {\n                \"type\": \"object\",\n                \"description\": \"The opening time details.\",\n                \"properties\": {\n                  \"day\": {\n                    \"type\": \"integer\",\n                    \"description\": \"Day of the week (0 = Sunday, 6 = Saturday).\",\n                    \"minimum\": 0,\n                    \"maximum\": 6\n                  },\n              \
  \    \"time\": {\n                    \"type\": \"string\",\n                    \"description\": \"The opening time in 24-hour format (HHMM).\",\n                    \"pattern\": \"^\\\\d{4}$\"\n                  }\n                }\n              },\n              \"close\": {\n                \"type\": \"object\",\n                \"description\": \"The closing time details.\",\n                \"properties\": {\n                  \"day\": {\n                    \"type\": \"integer\",\n                    \"description\": \"Day of the week (0 = Sunday, 6 = Saturday).\",\n                    \"minimum\": 0,\n                    \"maximum\": 6\n                  },\n                  \"time\": {\n                    \"type\": \"string\",\n                    \"description\": \"The closing time in 24-hour format (HHMM).\",\n                    \"pattern\": \"^\\\\d{4}$\"\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"weekday_text\"\
  : {\n          \"type\": \"array\",\n          \"description\": \"Array of human-readable strings describing hours for each day.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/json-schema/tripadvisor-location-schema.json
tags: []
title: Tripadvisor Location
---
