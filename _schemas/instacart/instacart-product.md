---
description: Represents a product in the Instacart Catalog system. Products are defined at the retailer level and are the same across all of a retailer's stores. Store-specific attributes such as pricing and availability are managed through the Item entity.
layout: schema
name: Instacart Product
properties_list:
- description: The retailer's unique product identifier used to match the product in the Instacart system.
  name: product_code
  type: string
- description: The display name of the product.
  name: name
  type: string
- description: The brand name of the product.
  name: brand
  type: string
- description: A detailed description of the product.
  name: description
  type: string
- description: The size or quantity description of the product, such as 12 oz or 6-pack.
  name: size
  type: string
- description: The Universal Product Code, typically 12 or 14 digits.
  name: upc
  type: string
- description: URL to the primary product image.
  name: image_url
  type: string
- description: The product category in the retailer's taxonomy.
  name: category
  type: string
- description: The product subcategory.
  name: subcategory
  type: string
- description: The store department the product belongs to.
  name: department
  type: string
- description: Additional product attributes such as dietary information, certifications, or nutritional details.
  name: attributes
  type: object
- description: Store-specific item records associated with this product.
  name: items
  type: array
provider_name: instacart
provider_slug: instacart
schema_file: json-schema/instacart-product-schema.json
slug: instacart-product
source_filename: instacart-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://instacart.com/schemas/instacart/product.json\",\n  \"title\": \"Instacart Product\",\n  \"description\": \"Represents a product in the Instacart Catalog system. Products are defined at the retailer level and are the same across all of a retailer's stores. Store-specific attributes such as pricing and availability are managed through the Item entity.\",\n  \"type\": \"object\",\n  \"required\": [\"product_code\", \"name\"],\n  \"properties\": {\n    \"product_code\": {\n      \"type\": \"string\",\n      \"description\": \"The retailer's unique product identifier used to match the product in the Instacart system.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the product.\",\n      \"minLength\": 1,\n      \"maxLength\": 500\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"The brand name of the product.\"\
  \n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the product.\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"The size or quantity description of the product, such as 12 oz or 6-pack.\"\n    },\n    \"upc\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9]{12,14}$\",\n      \"description\": \"The Universal Product Code, typically 12 or 14 digits.\"\n    },\n    \"image_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the primary product image.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The product category in the retailer's taxonomy.\"\n    },\n    \"subcategory\": {\n      \"type\": \"string\",\n      \"description\": \"The product subcategory.\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"The store department the product belongs to.\"\n    },\n\
  \    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Additional product attributes such as dietary information, certifications, or nutritional details.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Store-specific item records associated with this product.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Item\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Item\": {\n      \"type\": \"object\",\n      \"description\": \"An item representing a product at a specific store location, containing store-specific attributes like pricing and availability.\",\n      \"required\": [\"product_code\", \"store_code\"],\n      \"properties\": {\n        \"product_code\": {\n          \"type\": \"string\",\n          \"description\": \"The retailer's product identifier linking this item to its parent product.\"\n        },\n        \"store_code\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The retailer's unique store identifier where this item is sold.\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\": \"The current selling price of the item at this store.\",\n          \"minimum\": 0\n        },\n        \"sale_price\": {\n          \"type\": \"number\",\n          \"description\": \"The promotional or sale price, if applicable.\",\n          \"minimum\": 0\n        },\n        \"sale_start_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The start date of the sale period.\"\n        },\n        \"sale_end_date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The end date of the sale period.\"\n        },\n        \"available\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the item is currently available for purchase at this store.\"\n        },\n\
  \        \"inventory_count\": {\n          \"type\": \"integer\",\n          \"description\": \"The current inventory count at this store.\",\n          \"minimum\": 0\n        },\n        \"aisle\": {\n          \"type\": \"string\",\n          \"description\": \"The store aisle where the item is located.\"\n        },\n        \"shelf\": {\n          \"type\": \"string\",\n          \"description\": \"The shelf location within the aisle.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/json-schema/instacart-product-schema.json
tags: []
title: Instacart Product
---
