---
description: A product in a Shopify store. Products are the goods and services that merchants sell. They include information such as title, description, price, images, and variants.
layout: schema
name: Shopify Product
properties_list:
- description: Unique numeric identifier for the product
  name: id
  type: integer
- description: The name of the product
  name: title
  type: string
- description: The description of the product in HTML format
  name: body_html
  type:
  - string
  - 'null'
- description: The name of the product vendor
  name: vendor
  type: string
- description: A categorization for the product used for filtering and searching
  name: product_type
  type: string
- description: A URL-friendly unique string for the product automatically generated from the title
  name: handle
  type: string
- description: The date and time when the product was created in ISO 8601 format
  name: created_at
  type: string
- description: The date and time when the product was last modified in ISO 8601 format
  name: updated_at
  type: string
- description: The date and time when the product was published. Null if the product is not published.
  name: published_at
  type:
  - string
  - 'null'
- description: The suffix of the Liquid template used for the product page
  name: template_suffix
  type:
  - string
  - 'null'
- description: Whether the product is published to the Point of Sale channel
  name: published_scope
  type: string
- description: A comma-separated list of searchable keywords associated with the product
  name: tags
  type: string
- description: The status of the product
  name: status
  type: string
- description: The GraphQL Admin API identifier in the format gid://shopify/Product/{id}
  name: admin_graphql_api_id
  type: string
- description: The product variants. Each product can have up to 100 variants.
  name: variants
  type: array
- description: The custom product options. A product can have up to 3 options.
  name: options
  type: array
- description: The product images. A product can have up to 250 images.
  name: images
  type: array
- description: The primary product image
  name: image
  type: object
provider_name: Shopify
provider_slug: shopify
schema_file: json-schema/shopify-product-schema.json
slug: shopify-product
source_filename: shopify-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://shopify.dev/schemas/product.json\",\n  \"title\": \"Shopify Product\",\n  \"description\": \"A product in a Shopify store. Products are the goods and services that merchants sell. They include information such as title, description, price, images, and variants.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the product\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the product\"\n    },\n    \"body_html\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The description of the product in HTML format\"\n    },\n    \"vendor\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the product vendor\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"A categorization\
  \ for the product used for filtering and searching\"\n    },\n    \"handle\": {\n      \"type\": \"string\",\n      \"description\": \"A URL-friendly unique string for the product automatically generated from the title\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the product was created in ISO 8601 format\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the product was last modified in ISO 8601 format\"\n    },\n    \"published_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the product was published. Null if the product is not published.\"\n    },\n    \"template_suffix\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The suffix of the Liquid template used for the product page\"\n    },\n\
  \    \"published_scope\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the product is published to the Point of Sale channel\",\n      \"enum\": [\"web\", \"global\"]\n    },\n    \"tags\": {\n      \"type\": \"string\",\n      \"description\": \"A comma-separated list of searchable keywords associated with the product\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the product\",\n      \"enum\": [\"active\", \"archived\", \"draft\"]\n    },\n    \"admin_graphql_api_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL Admin API identifier in the format gid://shopify/Product/{id}\"\n    },\n    \"variants\": {\n      \"type\": \"array\",\n      \"description\": \"The product variants. Each product can have up to 100 variants.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Variant\"\n      }\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"description\": \"The custom product\
  \ options. A product can have up to 3 options.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ProductOption\"\n      }\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"description\": \"The product images. A product can have up to 250 images.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Image\"\n      }\n    },\n    \"image\": {\n      \"description\": \"The primary product image\",\n      \"$ref\": \"#/$defs/Image\"\n    }\n  },\n  \"required\": [\"id\", \"title\"],\n  \"$defs\": {\n    \"Variant\": {\n      \"type\": \"object\",\n      \"description\": \"A product variant representing a specific version of a product defined by its option values\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique numeric identifier\"\n        },\n        \"product_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID of the parent product\"\n        },\n        \"title\": {\n          \"\
  type\": \"string\",\n          \"description\": \"The variant title composed of option values\"\n        },\n        \"price\": {\n          \"type\": \"string\",\n          \"description\": \"The price of the variant as a decimal string\"\n        },\n        \"sku\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Stock keeping unit for tracking inventory\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"description\": \"The position of the variant in the product variant list\"\n        },\n        \"inventory_policy\": {\n          \"type\": \"string\",\n          \"description\": \"Whether to continue selling when out of stock\",\n          \"enum\": [\"deny\", \"continue\"]\n        },\n        \"compare_at_price\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The original price for comparison or sale display\"\n        },\n        \"fulfillment_service\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The fulfillment service associated with the variant\"\n        },\n        \"inventory_management\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The fulfillment service that tracks inventory for the variant\"\n        },\n        \"option1\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The value of the first product option\"\n        },\n        \"option2\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The value of the second product option\"\n        },\n        \"option3\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The value of the third product option\"\n        },\n        \"taxable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether tax is charged on the variant\"\n        },\n        \"barcode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The barcode, UPC, or\
  \ ISBN for the variant\"\n        },\n        \"grams\": {\n          \"type\": \"integer\",\n          \"description\": \"The weight of the variant in grams\"\n        },\n        \"weight\": {\n          \"type\": \"number\",\n          \"description\": \"The weight of the variant in the unit specified by weight_unit\"\n        },\n        \"weight_unit\": {\n          \"type\": \"string\",\n          \"description\": \"The unit of weight measurement\",\n          \"enum\": [\"g\", \"kg\", \"oz\", \"lb\"]\n        },\n        \"inventory_item_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The ID of the corresponding inventory item\"\n        },\n        \"inventory_quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The total tracked inventory quantity\"\n        },\n        \"requires_shipping\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the variant requires shipping\"\n        },\n        \"image_id\"\
  : {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The ID of the image associated with the variant\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"admin_graphql_api_id\": {\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\"id\", \"product_id\", \"title\", \"price\"]\n    },\n    \"ProductOption\": {\n      \"type\": \"object\",\n      \"description\": \"A product option such as Size or Color\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"product_id\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The option name\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"The position of the option in the list\"\n        },\n        \"values\": {\n          \"type\": \"array\",\n          \"description\": \"The available values for this option\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"Image\": {\n      \"type\": \"object\",\n      \"description\": \"A product image\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\"\n        },\n        \"product_id\": {\n          \"type\": \"integer\"\n        },\n        \"position\": {\n          \"type\": \"integer\",\n          \"description\": \"The position of the image in the list\"\n        },\n        \"alt\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Alternative text for accessibility\"\n        },\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"height\": {\n          \"type\": \"integer\"\n        },\n   \
  \     \"src\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the image\"\n        },\n        \"variant_ids\": {\n          \"type\": \"array\",\n          \"description\": \"Variant IDs associated with this image\",\n          \"items\": {\n            \"type\": \"integer\"\n          }\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"admin_graphql_api_id\": {\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\"id\", \"src\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/json-schema/shopify-product-schema.json
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
title: Shopify Product
---
