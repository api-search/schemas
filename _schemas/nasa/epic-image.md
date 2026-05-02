---
description: An Earth image from NASA's EPIC (Earth Polychromatic Imaging Camera) on DSCOVR.
layout: schema
name: EPIC Image
properties_list:
- description: Unique identifier for the image.
  name: identifier
  type: string
- description: Caption describing the image.
  name: caption
  type: string
- description: Image filename without extension.
  name: image
  type: string
- description: Version identifier.
  name: version
  type: string
- description: Date and time the image was taken.
  name: date
  type: string
- description: Geographic coordinates of the image center.
  name: centroid_coordinates
  type: object
- description: ''
  name: dscovr_j2000_position
  type: object
- description: ''
  name: lunar_j2000_position
  type: object
- description: ''
  name: sun_j2000_position
  type: object
- description: ''
  name: attitude_quaternions
  type: object
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/epic-image.json
slug: epic-image
source_filename: epic-image.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/epic-image.json\",\n  \"title\": \"EPIC Image\",\n  \"description\": \"An Earth image from NASA's EPIC (Earth Polychromatic Imaging Camera) on DSCOVR.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the image.\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"Caption describing the image.\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"Image filename without extension.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version identifier.\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the image was taken.\"\n    },\n    \"centroid_coordinates\": {\n \
  \     \"type\": \"object\",\n      \"properties\": {\n        \"lat\": { \"type\": \"number\" },\n        \"lon\": { \"type\": \"number\" }\n      },\n      \"description\": \"Geographic coordinates of the image center.\"\n    },\n    \"dscovr_j2000_position\": {\n      \"$ref\": \"#/$defs/position\"\n    },\n    \"lunar_j2000_position\": {\n      \"$ref\": \"#/$defs/position\"\n    },\n    \"sun_j2000_position\": {\n      \"$ref\": \"#/$defs/position\"\n    },\n    \"attitude_quaternions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"q0\": { \"type\": \"number\" },\n        \"q1\": { \"type\": \"number\" },\n        \"q2\": { \"type\": \"number\" },\n        \"q3\": { \"type\": \"number\" }\n      }\n    }\n  },\n  \"required\": [\"identifier\", \"image\", \"date\"],\n  \"$defs\": {\n    \"position\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"x\": { \"type\": \"number\" },\n        \"y\": { \"type\": \"number\" },\n        \"z\": { \"type\"\
  : \"number\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/epic-image.json
tags:
- Government
- Science
- Space
title: EPIC Image
---
