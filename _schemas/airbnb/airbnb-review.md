---
description: ''
layout: schema
name: Review
properties_list:
- description: The unique identifier of the review.
  name: id
  type: string
- description: The identifier of the associated reservation.
  name: reservation_id
  type: string
- description: Whether the review was written by a guest or host.
  name: reviewer_type
  type: string
- description: The overall star rating from 1 to 5.
  name: rating
  type: integer
- description: The text content of the review.
  name: comments
  type: string
- description: Individual category ratings provided by the reviewer.
  name: category_ratings
  type: object
- description: The host response to the review, if provided.
  name: host_response
  type: string
- description: The timestamp when the review was submitted.
  name: created_at
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-review-schema.json
slug: airbnb-review
source_filename: airbnb-review-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-review-schema.json\",\n  \"title\": \"Review\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the review.\"\n    },\n    \"reservation_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the associated reservation.\"\n    },\n    \"reviewer_type\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the review was written by a guest or host.\",\n      \"enum\": [\n        \"guest\",\n        \"host\"\n      ]\n    },\n    \"rating\": {\n      \"type\": \"integer\",\n      \"description\": \"The overall star rating from 1 to 5.\",\n      \"minimum\": 1,\n      \"maximum\": 5\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"The text content\
  \ of the review.\"\n    },\n    \"category_ratings\": {\n      \"type\": \"object\",\n      \"description\": \"Individual category ratings provided by the reviewer.\",\n      \"properties\": {\n        \"cleanliness\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 5,\n          \"description\": \"Rating for cleanliness.\"\n        },\n        \"communication\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 5,\n          \"description\": \"Rating for communication.\"\n        },\n        \"check_in\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 5,\n          \"description\": \"Rating for check-in experience.\"\n        },\n        \"accuracy\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 5,\n          \"description\": \"Rating for listing accuracy.\"\n        },\n        \"location\": {\n          \"type\": \"integer\",\n\
  \          \"minimum\": 1,\n          \"maximum\": 5,\n          \"description\": \"Rating for location.\"\n        },\n        \"value\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 5,\n          \"description\": \"Rating for value.\"\n        }\n      }\n    },\n    \"host_response\": {\n      \"type\": \"string\",\n      \"description\": \"The host response to the review, if provided.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the review was submitted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-review-schema.json
tags: []
title: Review
---
