---
description: A product in SAP Commerce Cloud representing a purchasable item with catalog information, pricing, stock levels, images, classifications, and customer reviews.
layout: schema
name: SAP Commerce Cloud Product
properties_list:
- description: Unique product code within the catalog
  name: code
  type: string
- description: Display name of the product
  name: name
  type: string
- description: Short product summary for listing pages
  name: summary
  type: string
- description: Full product description, may contain HTML
  name: description
  type: string
- description: Product manufacturer name
  name: manufacturer
  type: string
- description: European Article Number (barcode)
  name: ean
  type: string
- description: Relative URL to the product page
  name: url
  type: string
- description: Whether the product can be added to cart and purchased
  name: purchasable
  type: boolean
- description: Average customer review rating
  name: averageRating
  type: number
- description: Total number of customer reviews
  name: numberOfReviews
  type: integer
- description: ''
  name: price
  type: object
- description: ''
  name: stock
  type: object
- description: Product images in various formats
  name: images
  type: array
- description: Categories the product belongs to
  name: categories
  type: array
- description: Classification attributes and feature values
  name: classifications
  type: array
- description: Available product variants (e.g., size, color)
  name: variantOptions
  type: array
provider_name: SAP Commerce Cloud
provider_slug: sap-commerce-cloud
schema_file: json-schema/sap-commerce-cloud-product-schema.json
slug: sap-commerce-cloud-product
source_filename: sap-commerce-cloud-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-commerce-cloud/product.json\",\n  \"title\": \"SAP Commerce Cloud Product\",\n  \"description\": \"A product in SAP Commerce Cloud representing a purchasable item with catalog information, pricing, stock levels, images, classifications, and customer reviews.\",\n  \"type\": \"object\",\n  \"required\": [\"code\", \"name\"],\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Unique product code within the catalog\",\n      \"minLength\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the product\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Short product summary for listing pages\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full product description, may contain HTML\"\n    },\n    \"manufacturer\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Product manufacturer name\"\n    },\n    \"ean\": {\n      \"type\": \"string\",\n      \"description\": \"European Article Number (barcode)\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Relative URL to the product page\"\n    },\n    \"purchasable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product can be added to cart and purchased\"\n    },\n    \"averageRating\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 5,\n      \"description\": \"Average customer review rating\"\n    },\n    \"numberOfReviews\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total number of customer reviews\"\n    },\n    \"price\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"stock\": {\n      \"$ref\": \"#/$defs/Stock\"\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Image\"\
  \n      },\n      \"description\": \"Product images in various formats\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CategoryRef\"\n      },\n      \"description\": \"Categories the product belongs to\"\n    },\n    \"classifications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Classification\"\n      },\n      \"description\": \"Classification attributes and feature values\"\n    },\n    \"variantOptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/VariantOption\"\n      },\n      \"description\": \"Available product variants (e.g., size, color)\"\n    }\n  },\n  \"$defs\": {\n    \"Price\": {\n      \"type\": \"object\",\n      \"description\": \"Price information for a product\",\n      \"properties\": {\n        \"currencyIso\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 4217 currency code\",\n          \"pattern\": \"^[A-Z]{3}$\"\
  \n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Numeric price value\"\n        },\n        \"formattedValue\": {\n          \"type\": \"string\",\n          \"description\": \"Locale-formatted price string\"\n        },\n        \"priceType\": {\n          \"type\": \"string\",\n          \"enum\": [\"BUY\", \"FROM\"],\n          \"description\": \"Type of price\"\n        }\n      }\n    },\n    \"Stock\": {\n      \"type\": \"object\",\n      \"description\": \"Stock availability information\",\n      \"properties\": {\n        \"stockLevelStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"inStock\", \"lowStock\", \"outOfStock\"],\n          \"description\": \"Stock level status indicator\"\n        },\n        \"stockLevel\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Actual available stock quantity\"\n        }\n      }\n    },\n    \"Image\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Product image in a specific format\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Image URL\"\n        },\n        \"altText\": {\n          \"type\": \"string\",\n          \"description\": \"Image alt text for accessibility\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"enum\": [\"thumbnail\", \"product\", \"zoom\", \"cartIcon\"],\n          \"description\": \"Image format/size\"\n        },\n        \"imageType\": {\n          \"type\": \"string\",\n          \"enum\": [\"PRIMARY\", \"GALLERY\"],\n          \"description\": \"Image classification\"\n        },\n        \"galleryIndex\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Position within the image gallery\"\n        }\n      }\n    },\n    \"CategoryRef\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Reference to a product category\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Category code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Category display name\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"Category page URL\"\n        }\n      }\n    },\n    \"Classification\": {\n      \"type\": \"object\",\n      \"description\": \"Product classification with feature attributes\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Classification category code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Classification category name\"\n        },\n        \"features\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"code\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"comparable\": {\n                \"type\": \"boolean\"\n              },\n              \"featureValues\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"value\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"VariantOption\": {\n      \"type\": \"object\",\n      \"description\": \"Product variant option\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Variant product code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Variant display\
  \ name\"\n        },\n        \"stock\": {\n          \"$ref\": \"#/$defs/Stock\"\n        },\n        \"priceData\": {\n          \"$ref\": \"#/$defs/Price\"\n        },\n        \"variantOptionQualifiers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"qualifier\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/json-schema/sap-commerce-cloud-product-schema.json
tags:
- B2B
- B2C
- Commerce
- Customer Experience
- Ecommerce
- Omnichannel
- Retail
title: SAP Commerce Cloud Product
---
