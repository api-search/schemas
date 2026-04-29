---
description: A recommended product with essential display attributes.
layout: schema
name: RecommendedProduct
properties_list:
- description: Product SKU number.
  name: sku
  type: integer
- description: Product name variations.
  name: names
  type: object
- description: Product image URLs.
  name: images
  type: object
- description: Product pricing information.
  name: prices
  type: object
- description: Related URLs for the product.
  name: links
  type: object
- description: Rank position in the recommendation list.
  name: rank
  type: integer
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/recommendations-api-recommended-product-schema.json
slug: recommendations-api-recommended-product
source_filename: recommendations-api-recommended-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/recommendations-api-recommended-product-schema.json\",\n  \"title\": \"RecommendedProduct\",\n  \"description\": \"A recommended product with essential display attributes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sku\": {\n      \"type\": \"integer\",\n      \"description\": \"Product SKU number.\",\n      \"example\": 1234567\n    },\n    \"names\": {\n      \"type\": \"object\",\n      \"description\": \"Product name variations.\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Product display title.\",\n          \"example\": \"Sample Laptop 15\\\" 16GB RAM\"\n        }\n      }\n    },\n    \"images\": {\n      \"type\": \"object\",\n      \"description\": \"Product image URLs.\",\n      \"properties\": {\n        \"standard\":\
  \ {\n          \"type\": \"string\",\n          \"description\": \"Standard product image URL.\",\n          \"example\": \"https://pisces.bbystatic.com/image2/BestBuy_US/images/products/1234/1234567_sd.jpg\"\n        }\n      }\n    },\n    \"prices\": {\n      \"type\": \"object\",\n      \"description\": \"Product pricing information.\",\n      \"properties\": {\n        \"regular\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Regular price in USD.\",\n          \"example\": 999.99\n        },\n        \"current\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Current (sale) price in USD.\",\n          \"example\": 849.99\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Related URLs for the product.\",\n      \"properties\": {\n        \"product\": {\n          \"type\": \"string\",\n          \"description\": \"API URL for\
  \ full product data.\",\n          \"example\": \"https://api.bestbuy.com/v1/products/1234567.json\"\n        },\n        \"web\": {\n          \"type\": \"string\",\n          \"description\": \"URL of the product page on bestbuy.com.\",\n          \"example\": \"https://www.bestbuy.com/site/sample-laptop/1234567.p\"\n        },\n        \"addToCart\": {\n          \"type\": \"string\",\n          \"description\": \"URL for adding to cart.\",\n          \"example\": \"https://www.bestbuy.com/cart/api/v1/addToCart\"\n        }\n      }\n    },\n    \"rank\": {\n      \"type\": \"integer\",\n      \"description\": \"Rank position in the recommendation list.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/recommendations-api-recommended-product-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: RecommendedProduct
---
