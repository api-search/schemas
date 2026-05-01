---
description: Schema for a Google Cloud Recommendations AI catalog item resource.
layout: schema
name: Catalog Item
properties_list:
- description: Unique identifier of the catalog item.
  name: id
  type: string
- description: Category hierarchies for the catalog item.
  name: categoryHierarchies
  type: array
- description: Title of the catalog item.
  name: title
  type: string
- description: Description of the catalog item.
  name: description
  type: string
- description: Language code of the catalog item content.
  name: languageCode
  type: string
- description: Tags associated with the catalog item.
  name: tags
  type: array
- description: Custom attributes of the catalog item.
  name: itemAttributes
  type: object
- description: Product-specific metadata.
  name: productMetadata
  type: object
provider_name: Google Cloud Recommendations AI
provider_slug: google-cloud-recommendations-ai
schema_file: json-schema/catalog-item.json
slug: catalog-item
source_filename: catalog-item.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-recommendations-ai/refs/heads/main/json-schema/catalog-item.json\",\n  \"title\": \"Catalog Item\",\n  \"description\": \"Schema for a Google Cloud Recommendations AI catalog item resource.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"categoryHierarchies\", \"title\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the catalog item.\"\n    },\n    \"categoryHierarchies\": {\n      \"type\": \"array\",\n      \"description\": \"Category hierarchies for the catalog item.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"categories\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Ordered list of category names from root\
  \ to leaf.\"\n          }\n        }\n      }\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the catalog item.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the catalog item.\"\n    },\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"Language code of the catalog item content.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags associated with the catalog item.\"\n    },\n    \"itemAttributes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom attributes of the catalog item.\",\n      \"properties\": {\n        \"categoricalFeatures\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"object\"\n          }\n        },\n        \"numericalFeatures\": {\n          \"type\": \"object\",\n          \"additionalProperties\"\
  : {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"productMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Product-specific metadata.\",\n      \"properties\": {\n        \"priceRange\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"min\": {\n              \"type\": \"number\",\n              \"description\": \"Minimum product price.\"\n            },\n            \"max\": {\n              \"type\": \"number\",\n              \"description\": \"Maximum product price.\"\n            }\n          }\n        },\n        \"availableQuantity\": {\n          \"type\": \"integer\",\n          \"description\": \"Available quantity of the product.\"\n        },\n        \"canonicalProductUri\": {\n          \"type\": \"string\",\n          \"description\": \"Canonical URI of the product page.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-recommendations-ai/refs/heads/main/json-schema/catalog-item.json
tags:
- E-Commerce
- Google Cloud
- Machine Learning
- Personalization
- Recommendations
- Retail
title: Catalog Item
---
