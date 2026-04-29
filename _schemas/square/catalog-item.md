---
description: A CatalogObject instance of the ITEM type, also referred to as an item, in the catalog. Represents a product or service that a seller offers for sale.
layout: schema
name: Square Catalog Item
properties_list:
- description: The item's name. This is a searchable attribute for use in applicable query filters.
  name: name
  type: string
- description: The item's description as plain text.
  name: description
  type: string
- description: The item's description as expressed in valid HTML elements.
  name: description_html
  type: string
- description: The text of the item's display label in the Square Point of Sale app. Only up to the first five characters of the string are used.
  name: abbreviation
  type: string
- description: The color of the item's display label in the Square Point of Sale app. This must be a valid hex color code.
  name: label_color
  type: string
- description: Indicates whether the item is taxable (true) or non-taxable (false). Default is true.
  name: is_taxable
  type: boolean
- description: 'The ID of the item''s category, if any. Deprecated: use categories instead.'
  name: category_id
  type: string
- description: The list of categories that this item belongs to.
  name: categories
  type: array
- description: A set of IDs indicating the taxes enabled for this item.
  name: tax_ids
  type: array
- description: A set of CatalogItemModifierListInfo objects representing the modifier lists that apply to this item.
  name: modifier_list_info
  type: array
- description: A list of CatalogItemVariation objects for this item. An item must have at least one variation.
  name: variations
  type: array
- description: The product type of the item. Once set, the product_type value cannot be modified.
  name: product_type
  type: string
- description: If false, the Square Point of Sale app will present the CatalogItem's details screen immediately, allowing the merchant to choose CatalogModifiers before adding the item to the cart.
  name: skip_modifier_screen
  type: boolean
- description: 'List of item options IDs for this item. Used to manage and group item variations in a specified order. Maximum: 6 item options.'
  name: item_options
  type: array
- description: The IDs of images associated with this CatalogItem instance.
  name: image_ids
  type: array
- description: A name to sort the item by. If unspecified, the regular name field is used for sorting.
  name: sort_name
  type: string
- description: The reporting category associated with this item.
  name: reporting_category
  type: object
- description: The channels where this item is available.
  name: channels
  type: array
- description: Whether this item is archived (soft-deleted).
  name: is_archived
  type: boolean
provider_name: Square
provider_slug: square
schema_file: json-schema/catalog-item.json
slug: catalog-item
source_json: "{\n  \"$id\": \"https://github.com/api-evangelist/square/blob/main/json-schema/catalog-item.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Square Catalog Item\",\n  \"description\": \"A CatalogObject instance of the ITEM type, also referred to as an item, in the catalog. Represents a product or service that a seller offers for sale.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The item's name. This is a searchable attribute for use in applicable query filters.\",\n      \"maxLength\": 512\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The item's description as plain text.\",\n      \"maxLength\": 4096\n    },\n    \"description_html\": {\n      \"type\": \"string\",\n      \"description\": \"The item's description as expressed in valid HTML elements.\",\n      \"maxLength\": 65535\n    },\n    \"abbreviation\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"The text of the item's display label in the Square Point of Sale app. Only up to the first five characters of the string are used.\",\n      \"maxLength\": 24\n    },\n    \"label_color\": {\n      \"type\": \"string\",\n      \"description\": \"The color of the item's display label in the Square Point of Sale app. This must be a valid hex color code.\"\n    },\n    \"is_taxable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the item is taxable (true) or non-taxable (false). Default is true.\"\n    },\n    \"category_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the item's category, if any. Deprecated: use categories instead.\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the category.\"\n\
  \          },\n          \"ordinal\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"The order of the category within the item.\"\n          }\n        }\n      },\n      \"description\": \"The list of categories that this item belongs to.\"\n    },\n    \"tax_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"A set of IDs indicating the taxes enabled for this item.\"\n    },\n    \"modifier_list_info\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"modifier_list_id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the CatalogModifierList controlled by this CatalogModifierListInfo.\"\n          },\n          \"min_selected_modifiers\": {\n            \"type\": \"integer\",\n            \"description\": \"The minimum number of modifiers that must be selected\
  \ from the modifier list.\"\n          },\n          \"max_selected_modifiers\": {\n            \"type\": \"integer\",\n            \"description\": \"The maximum number of modifiers that can be selected from the modifier list.\"\n          },\n          \"enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the modifier list is enabled for this item.\"\n          }\n        }\n      },\n      \"description\": \"A set of CatalogItemModifierListInfo objects representing the modifier lists that apply to this item.\"\n    },\n    \"variations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique ID for the catalog variation object.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of this object, always ITEM_VARIATION.\",\n            \"\
  const\": \"ITEM_VARIATION\"\n          },\n          \"item_variation_data\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"item_id\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the CatalogItem associated with this item variation.\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The item variation's name.\"\n              },\n              \"sku\": {\n                \"type\": \"string\",\n                \"description\": \"The item variation's SKU, if any.\"\n              },\n              \"upc\": {\n                \"type\": \"string\",\n                \"description\": \"The universal product code (UPC) of the item variation, if any.\"\n              },\n              \"pricing_type\": {\n                \"type\": \"string\",\n                \"description\": \"Indicates whether the item variation's price is fixed or determined\
  \ at the time of sale.\",\n                \"enum\": [\"FIXED_PRICING\", \"VARIABLE_PRICING\"]\n              },\n              \"price_money\": {\n                \"$ref\": \"money.json\",\n                \"description\": \"The item variation's price, if fixed pricing is used.\"\n              },\n              \"track_inventory\": {\n                \"type\": \"boolean\",\n                \"description\": \"If true, inventory tracking is active for the variation.\"\n              },\n              \"sellable\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether this variation can be sold.\"\n              },\n              \"stockable\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether stock of this variation can be counted.\"\n              }\n            }\n          }\n        }\n      },\n      \"description\": \"A list of CatalogItemVariation objects for this item. An item must have at least one variation.\"\
  \n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"The product type of the item. Once set, the product_type value cannot be modified.\",\n      \"enum\": [\"REGULAR\", \"GIFT_CARD\", \"APPOINTMENTS_SERVICE\", \"FOOD_AND_BEV\", \"LEGACY_SQUARE_ONLINE_SERVICE\", \"LEGACY_SQUARE_ONLINE_MEMBERSHIP\"]\n    },\n    \"skip_modifier_screen\": {\n      \"type\": \"boolean\",\n      \"description\": \"If false, the Square Point of Sale app will present the CatalogItem's details screen immediately, allowing the merchant to choose CatalogModifiers before adding the item to the cart.\"\n    },\n    \"item_options\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"item_option_id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique id of the item option.\"\n          }\n        }\n      },\n      \"description\": \"List of item options IDs for this item. Used to\
  \ manage and group item variations in a specified order. Maximum: 6 item options.\"\n    },\n    \"image_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The IDs of images associated with this CatalogItem instance.\"\n    },\n    \"sort_name\": {\n      \"type\": \"string\",\n      \"description\": \"A name to sort the item by. If unspecified, the regular name field is used for sorting.\"\n    },\n    \"reporting_category\": {\n      \"type\": \"object\",\n      \"description\": \"The reporting category associated with this item.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the reporting category.\"\n        },\n        \"ordinal\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"The order of the reporting category.\"\n        }\n      }\n    },\n    \"channels\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The channels where this item is available.\"\n    },\n    \"is_archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this item is archived (soft-deleted).\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/square/refs/heads/main/json-schema/catalog-item.json
tags:
- Bookings
- Catalog
- Checkout
- Customers
- Disputes
- Ecommerce
- Financial Technology
- Gift Cards
- Inventory
- Invoicing
- Labor
- Locations
- Loyalty
- Merchants
- Orders
- Payments
- Point of Sale
- Refunds
- Retail
- Subscriptions
- Team
- Terminal
- Webhooks
title: Square Catalog Item
---
