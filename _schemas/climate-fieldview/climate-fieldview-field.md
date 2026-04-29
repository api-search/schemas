---
description: Schema representing an agricultural field in the Climate FieldView platform, including its boundary, metadata, and associated agronomic layers.
layout: schema
name: Climate FieldView Field
properties_list:
- description: Unique field identifier
  name: id
  type: string
- description: Field name as entered by the grower
  name: name
  type: string
- description: Name of the grower who owns this field
  name: growerName
  type: string
- description: Farm or operation name the field belongs to
  name: farmName
  type: string
- description: Field area in acres
  name: acreage
  type: number
- description: Field boundary as a GeoJSON polygon
  name: boundary
  type: object
- description: Geographic centroid of the field
  name: centroid
  type: object
- description: US state abbreviation where the field is located
  name: state
  type: string
- description: County name where the field is located
  name: county
  type: string
- description: Field creation timestamp in the platform
  name: createdAt
  type: string
- description: Last field modification timestamp
  name: updatedAt
  type: string
provider_name: Climate FieldView
provider_slug: climate-fieldview
schema_file: json-schema/climate-fieldview-field-schema.json
slug: climate-fieldview-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.climate.com/api/schemas/field\",\n  \"title\": \"Climate FieldView Field\",\n  \"description\": \"Schema representing an agricultural field in the Climate FieldView platform, including its boundary, metadata, and associated agronomic layers.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique field identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Field name as entered by the grower\",\n      \"maxLength\": 255\n    },\n    \"growerName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the grower who owns this field\"\n    },\n    \"farmName\": {\n      \"type\": \"string\",\n      \"description\": \"Farm or operation name the field belongs to\"\n    },\n    \"acreage\": {\n      \"type\"\
  : \"number\",\n      \"format\": \"double\",\n      \"description\": \"Field area in acres\",\n      \"minimum\": 0\n    },\n    \"boundary\": {\n      \"$ref\": \"#/$defs/GeoJsonFeature\",\n      \"description\": \"Field boundary as a GeoJSON polygon\"\n    },\n    \"centroid\": {\n      \"$ref\": \"#/$defs/GeoPoint\",\n      \"description\": \"Geographic centroid of the field\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"US state abbreviation where the field is located\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"county\": {\n      \"type\": \"string\",\n      \"description\": \"County name where the field is located\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Field creation timestamp in the platform\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last field modification timestamp\"\n    }\n\
  \  },\n  \"$defs\": {\n    \"GeoJsonFeature\": {\n      \"type\": \"object\",\n      \"required\": [\"type\", \"geometry\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Feature\"\n        },\n        \"geometry\": {\n          \"oneOf\": [\n            { \"$ref\": \"#/$defs/Polygon\" },\n            { \"$ref\": \"#/$defs/MultiPolygon\" }\n          ]\n        },\n        \"properties\": {\n          \"type\": [\"object\", \"null\"]\n        }\n      }\n    },\n    \"Polygon\": {\n      \"type\": \"object\",\n      \"required\": [\"type\", \"coordinates\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Polygon\"\n        },\n        \"coordinates\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/Position\"\n            },\n            \"minItems\": 4\n          }\n   \
  \     }\n      }\n    },\n    \"MultiPolygon\": {\n      \"type\": \"object\",\n      \"required\": [\"type\", \"coordinates\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"MultiPolygon\"\n        },\n        \"coordinates\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/Position\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"Position\": {\n      \"type\": \"array\",\n      \"description\": \"[longitude, latitude] coordinate pair\",\n      \"minItems\": 2,\n      \"maxItems\": 3,\n      \"items\": {\n        \"type\": \"number\"\n      }\n    },\n    \"GeoPoint\": {\n      \"type\": \"object\",\n      \"required\": [\"latitude\", \"longitude\"],\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\"\
  ,\n          \"format\": \"double\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/climate-fieldview/refs/heads/main/json-schema/climate-fieldview-field-schema.json
tags:
- Agriculture
- Bayer
- Crop Data
- Field Boundaries
- Harvest
- OAuth2
- Planting
- Precision Ag
title: Climate FieldView Field
---
