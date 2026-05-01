---
description: JSON Schema for the Google Content API for Shopping product and related objects.
layout: schema
name: Google Content API for Shopping Schema
properties_list: []
provider_name: Google Content API for Shopping
provider_slug: google-shopping
schema_file: json-schema/google-shopping.json
slug: google-shopping
source_filename: google-shopping.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-shopping/refs/heads/main/json-schema/google-shopping.json\",\n  \"title\": \"Google Content API for Shopping Schema\",\n  \"description\": \"JSON Schema for the Google Content API for Shopping product and related objects.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"Product\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"REST ID of the product.\"\n        },\n        \"offerId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique product identifier in the merchant's store.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Title of the product.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the product.\"\
  \n        },\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the product page.\"\n        },\n        \"imageLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the product image.\"\n        },\n        \"contentLanguage\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter language code.\"\n        },\n        \"targetCountry\": {\n          \"type\": \"string\",\n          \"description\": \"CLDR territory code.\"\n        },\n        \"channel\": {\n          \"type\": \"string\",\n          \"enum\": [\"online\", \"local\"],\n          \"description\": \"Product channel.\"\n        },\n        \"availability\": {\n          \"type\": \"string\",\n          \"description\": \"Availability status.\"\n        },\n        \"condition\": {\n          \"type\": \"string\",\n          \"enum\": [\"new\", \"refurbished\", \"used\"],\n\
  \          \"description\": \"Condition of the product.\"\n        },\n        \"price\": {\n          \"$ref\": \"#/$defs/Price\"\n        },\n        \"brand\": {\n          \"type\": \"string\",\n          \"description\": \"Brand of the product.\"\n        },\n        \"gtin\": {\n          \"type\": \"string\",\n          \"description\": \"Global Trade Item Number.\"\n        },\n        \"mpn\": {\n          \"type\": \"string\",\n          \"description\": \"Manufacturer Part Number.\"\n        },\n        \"googleProductCategory\": {\n          \"type\": \"string\",\n          \"description\": \"Google product category.\"\n        }\n      }\n    },\n    \"Price\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The price value.\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code.\"\n        }\n      }\n    },\n \
  \   \"ProductsListResponse\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\"\n        },\n        \"nextPageToken\": {\n          \"type\": \"string\"\n        },\n        \"resources\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Product\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-shopping/refs/heads/main/json-schema/google-shopping.json
tags:
- E-Commerce
- Google Shopping
- Merchant Center
- Product Listings
- Retail
- Shopping
title: Google Content API for Shopping Schema
---
