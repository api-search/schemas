---
description: A user review for a Tripadvisor location including rating, text, trip type, and reviewer information.
layout: schema
name: Tripadvisor Review
properties_list:
- description: The unique identifier for this review.
  name: id
  type: integer
- description: The language code of the review.
  name: lang
  type: string
- description: The Tripadvisor location ID this review is for.
  name: location_id
  type: integer
- description: The date and time the review was published in ISO 8601 format.
  name: published_date
  type: string
- description: The overall rating given by the reviewer.
  name: rating
  type: integer
- description: The number of helpful votes this review has received.
  name: helpful_votes
  type: integer
- description: URL of the rating bubble image for this review's rating.
  name: rating_image_url
  type: string
- description: URL of the full review on Tripadvisor.
  name: url
  type: string
- description: The full text content of the review.
  name: text
  type: string
- description: The title or headline of the review.
  name: title
  type: string
- description: The type of trip associated with this review.
  name: trip_type
  type: string
- description: The date of travel associated with this review in YYYY-MM format.
  name: travel_date
  type: string
- description: ''
  name: user
  type: object
- description: Sub-rating scores for specific aspects of the location (e.g., service, value, cleanliness).
  name: subratings
  type: object
provider_name: tripadvisor
provider_slug: tripadvisor
schema_file: json-schema/tripadvisor-review-schema.json
slug: tripadvisor-review
source_filename: tripadvisor-review-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer-tripadvisor.com/schemas/tripadvisor/review.json\",\n  \"title\": \"Tripadvisor Review\",\n  \"description\": \"A user review for a Tripadvisor location including rating, text, trip type, and reviewer information.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"rating\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier for this review.\"\n    },\n    \"lang\": {\n      \"type\": \"string\",\n      \"description\": \"The language code of the review.\",\n      \"minLength\": 2,\n      \"maxLength\": 5\n    },\n    \"location_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The Tripadvisor location ID this review is for.\"\n    },\n    \"published_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the review was published in ISO\
  \ 8601 format.\"\n    },\n    \"rating\": {\n      \"type\": \"integer\",\n      \"description\": \"The overall rating given by the reviewer.\",\n      \"minimum\": 1,\n      \"maximum\": 5\n    },\n    \"helpful_votes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of helpful votes this review has received.\",\n      \"minimum\": 0\n    },\n    \"rating_image_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the rating bubble image for this review's rating.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the full review on Tripadvisor.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The full text content of the review.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title or headline of the review.\",\n      \"maxLength\": 200\n    },\n    \"trip_type\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The type of trip associated with this review.\",\n      \"enum\": [\"business\", \"couples\", \"family\", \"friends\", \"solo\"]\n    },\n    \"travel_date\": {\n      \"type\": \"string\",\n      \"description\": \"The date of travel associated with this review in YYYY-MM format.\",\n      \"pattern\": \"^\\\\d{4}-\\\\d{2}$\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/UserReference\"\n    },\n    \"subratings\": {\n      \"type\": \"object\",\n      \"description\": \"Sub-rating scores for specific aspects of the location (e.g., service, value, cleanliness).\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/SubRating\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"UserReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a Tripadvisor user who authored the review.\",\n      \"properties\": {\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the\
  \ reviewer.\"\n        },\n        \"user_location\": {\n          \"type\": \"object\",\n          \"description\": \"The reviewer's stated location.\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The display name of the reviewer's location.\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The location ID of the reviewer's location.\"\n            }\n          }\n        },\n        \"avatar\": {\n          \"type\": \"object\",\n          \"description\": \"Avatar images for the reviewer.\",\n          \"properties\": {\n            \"thumbnail\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL of the reviewer's thumbnail avatar.\"\n            },\n            \"small\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"\
  URL of the reviewer's small avatar.\"\n            },\n            \"large\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"URL of the reviewer's large avatar.\"\n            }\n          }\n        }\n      }\n    },\n    \"SubRating\": {\n      \"type\": \"object\",\n      \"description\": \"A sub-rating score for a specific aspect of a location.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the sub-rating category (e.g., Service, Value).\"\n        },\n        \"rating_image_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the rating bubble image for this sub-rating.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The sub-rating numeric value.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/json-schema/tripadvisor-review-schema.json
tags: []
title: Tripadvisor Review
---
