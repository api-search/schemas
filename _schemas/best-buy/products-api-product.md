---
description: A Best Buy product with pricing, availability, and metadata.
layout: schema
name: Product
properties_list:
- description: Unique Best Buy product identifier (SKU number).
  name: sku
  type: integer
- description: Product display name.
  name: name
  type: string
- description: Regular (non-sale) price in USD.
  name: regularPrice
  type: number
- description: Current sale price in USD.
  name: salePrice
  type: number
- description: Whether the product is currently on sale.
  name: onSale
  type: boolean
- description: Product manufacturer or brand name.
  name: manufacturer
  type: string
- description: Manufacturer model number.
  name: modelNumber
  type: string
- description: Brief product description.
  name: shortDescription
  type: string
- description: Detailed product description.
  name: longDescription
  type: string
- description: URL of the primary product image.
  name: image
  type: string
- description: URL of the product page on bestbuy.com.
  name: url
  type: string
- description: URL for adding this product to the shopping cart.
  name: addToCartUrl
  type: string
- description: Whether the product is available for in-store purchase.
  name: inStoreAvailability
  type: boolean
- description: Whether the product is available online.
  name: onlineAvailability
  type: boolean
- description: Product type (HardGood, Movie, Music, Game, Software, etc.).
  name: type
  type: string
- description: Product class name.
  name: class
  type: string
- description: Product class identifier.
  name: classId
  type: integer
- description: Product subclass name.
  name: subclass
  type: string
- description: Product subclass identifier.
  name: subclassId
  type: integer
- description: Department name.
  name: department
  type: string
- description: Department identifier.
  name: departmentId
  type: integer
- description: Hierarchical category path from root to this product's category.
  name: categoryPath
  type: array
- description: Total number of customer reviews.
  name: customerReviewCount
  type: integer
- description: Average customer review rating out of 5.
  name: customerReviewAverage
  type: number
- description: Date and time the price was last updated.
  name: priceUpdateDate
  type: string
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/products-api-product-schema.json
slug: products-api-product
source_filename: products-api-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/products-api-product-schema.json\",\n  \"title\": \"Product\",\n  \"description\": \"A Best Buy product with pricing, availability, and metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sku\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique Best Buy product identifier (SKU number).\",\n      \"example\": 1234567\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Product display name.\",\n      \"example\": \"Sample Laptop 15\\\" 16GB RAM\"\n    },\n    \"regularPrice\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Regular (non-sale) price in USD.\",\n      \"example\": 999.99\n    },\n    \"salePrice\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Current sale price\
  \ in USD.\",\n      \"example\": 849.99\n    },\n    \"onSale\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product is currently on sale.\",\n      \"example\": true\n    },\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"Product manufacturer or brand name.\",\n      \"example\": \"SampleBrand\"\n    },\n    \"modelNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Manufacturer model number.\",\n      \"example\": \"SB-1234\"\n    },\n    \"shortDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Brief product description.\",\n      \"example\": \"High-performance laptop for everyday computing.\"\n    },\n    \"longDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed product description.\",\n      \"example\": \"Detailed description of the laptop features and specifications.\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the\
  \ primary product image.\",\n      \"example\": \"https://pisces.bbystatic.com/image2/BestBuy_US/images/products/1234/1234567_sd.jpg\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the product page on bestbuy.com.\",\n      \"example\": \"https://www.bestbuy.com/site/sample-laptop/1234567.p\"\n    },\n    \"addToCartUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL for adding this product to the shopping cart.\",\n      \"example\": \"https://www.bestbuy.com/cart/api/v1/addToCart?items%5B0%5D%5BskuId%5D=1234567\"\n    },\n    \"inStoreAvailability\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product is available for in-store purchase.\",\n      \"example\": true\n    },\n    \"onlineAvailability\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product is available online.\",\n      \"example\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Product type (HardGood, Movie, Music, Game, Software, etc.).\",\n      \"example\": \"HardGood\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"Product class name.\",\n      \"example\": \"LAPTOPS/NOTEBOOKS\"\n    },\n    \"classId\": {\n      \"type\": \"integer\",\n      \"description\": \"Product class identifier.\",\n      \"example\": 539\n    },\n    \"subclass\": {\n      \"type\": \"string\",\n      \"description\": \"Product subclass name.\",\n      \"example\": \"ALL LAPTOPS\"\n    },\n    \"subclassId\": {\n      \"type\": \"integer\",\n      \"description\": \"Product subclass identifier.\",\n      \"example\": 2408\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department name.\",\n      \"example\": \"COMPUTERS\"\n    },\n    \"departmentId\": {\n      \"type\": \"integer\",\n      \"description\": \"Department identifier.\",\n      \"example\": 3\n    },\n    \"categoryPath\": {\n      \"type\": \"\
  array\",\n      \"description\": \"Hierarchical category path from root to this product's category.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CategoryRef\"\n      }\n    },\n    \"customerReviewCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of customer reviews.\",\n      \"example\": 450\n    },\n    \"customerReviewAverage\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average customer review rating out of 5.\",\n      \"example\": 4.5\n    },\n    \"priceUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the price was last updated.\",\n      \"example\": \"2026-04-01T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/products-api-product-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: Product
---
