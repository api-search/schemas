---
description: A shopping cart in SAP Commerce Cloud containing products selected for purchase, with delivery and payment configuration for checkout.
layout: schema
name: SAP Commerce Cloud Cart
properties_list:
- description: Unique cart code for authenticated users
  name: code
  type: string
- description: Cart GUID used for anonymous or guest carts
  name: guid
  type: string
- description: Number of distinct line items in the cart
  name: totalItems
  type: integer
- description: Total quantity of units across all entries
  name: totalUnitCount
  type: integer
- description: ''
  name: subTotal
  type: object
- description: ''
  name: deliveryCost
  type: object
- description: ''
  name: totalTax
  type: object
- description: ''
  name: totalPrice
  type: object
- description: ''
  name: totalPriceWithTax
  type: object
- description: ''
  name: totalDiscounts
  type: object
- description: Cart line items
  name: entries
  type: array
- description: ''
  name: deliveryAddress
  type: object
- description: ''
  name: deliveryMode
  type: object
- description: ''
  name: paymentInfo
  type: object
- description: Vouchers applied to the cart
  name: appliedVouchers
  type: array
- description: Order-level promotions applied
  name: appliedOrderPromotions
  type: array
- description: Product-level promotions applied
  name: appliedProductPromotions
  type: array
- description: ''
  name: user
  type: object
- description: ''
  name: orderDiscounts
  type: object
- description: ''
  name: productDiscounts
  type: object
- description: Delivery order groups for split shipments
  name: deliveryOrderGroups
  type: array
provider_name: SAP Commerce Cloud
provider_slug: sap-commerce-cloud
schema_file: json-schema/sap-commerce-cloud-cart-schema.json
slug: sap-commerce-cloud-cart
source_filename: sap-commerce-cloud-cart-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-commerce-cloud/cart.json\",\n  \"title\": \"SAP Commerce Cloud Cart\",\n  \"description\": \"A shopping cart in SAP Commerce Cloud containing products selected for purchase, with delivery and payment configuration for checkout.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Unique cart code for authenticated users\"\n    },\n    \"guid\": {\n      \"type\": \"string\",\n      \"description\": \"Cart GUID used for anonymous or guest carts\"\n    },\n    \"totalItems\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of distinct line items in the cart\"\n    },\n    \"totalUnitCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total quantity of units across all entries\"\n    },\n    \"subTotal\": {\n      \"$ref\"\
  : \"#/$defs/Price\"\n    },\n    \"deliveryCost\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"totalTax\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"totalPrice\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"totalPriceWithTax\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"totalDiscounts\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"entries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CartEntry\"\n      },\n      \"description\": \"Cart line items\"\n    },\n    \"deliveryAddress\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"deliveryMode\": {\n      \"$ref\": \"#/$defs/DeliveryMode\"\n    },\n    \"paymentInfo\": {\n      \"$ref\": \"#/$defs/PaymentDetails\"\n    },\n    \"appliedVouchers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Voucher\"\n      },\n      \"description\": \"Vouchers applied to the cart\"\n    },\n    \"appliedOrderPromotions\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PromotionResult\"\n      },\n      \"description\": \"Order-level promotions applied\"\n    },\n    \"appliedProductPromotions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PromotionResult\"\n      },\n      \"description\": \"Product-level promotions applied\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/Principal\"\n    },\n    \"orderDiscounts\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"productDiscounts\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"deliveryOrderGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"entries\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/CartEntry\"\n            }\n          },\n          \"totalPriceWithTax\": {\n            \"$ref\": \"#/$defs/Price\"\n          }\n        }\n      },\n      \"description\"\
  : \"Delivery order groups for split shipments\"\n    }\n  },\n  \"$defs\": {\n    \"Price\": {\n      \"type\": \"object\",\n      \"description\": \"Price or monetary amount\",\n      \"properties\": {\n        \"currencyIso\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"ISO 4217 currency code\"\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"Numeric value\"\n        },\n        \"formattedValue\": {\n          \"type\": \"string\",\n          \"description\": \"Locale-formatted value string\"\n        }\n      }\n    },\n    \"CartEntry\": {\n      \"type\": \"object\",\n      \"description\": \"Individual item in the shopping cart\",\n      \"properties\": {\n        \"entryNumber\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Zero-based entry index\"\n        },\n        \"product\": {\n          \"type\": \"object\",\n     \
  \     \"properties\": {\n            \"code\": {\n              \"type\": \"string\",\n              \"description\": \"Product code\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Product name\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"description\": \"Product page URL\"\n            },\n            \"images\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"url\": {\n                    \"type\": \"string\"\n                  },\n                  \"format\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Quantity in cart\"\n        },\n        \"basePrice\"\
  : {\n          \"$ref\": \"#/$defs/Price\"\n        },\n        \"totalPrice\": {\n          \"$ref\": \"#/$defs/Price\"\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the quantity can be updated\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Delivery address\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"firstName\": {\n          \"type\": \"string\"\n        },\n        \"lastName\": {\n          \"type\": \"string\"\n        },\n        \"line1\": {\n          \"type\": \"string\"\n        },\n        \"line2\": {\n          \"type\": \"string\"\n        },\n        \"town\": {\n          \"type\": \"string\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isocode\": {\n    \
  \          \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"region\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isocode\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"phone\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"DeliveryMode\": {\n      \"type\": \"object\",\n      \"description\": \"Delivery or shipping method\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Delivery mode code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Delivery mode display name\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Delivery mode description\"\n    \
  \    },\n        \"deliveryCost\": {\n          \"$ref\": \"#/$defs/Price\"\n        }\n      }\n    },\n    \"PaymentDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Payment information for the cart\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"accountHolderName\": {\n          \"type\": \"string\"\n        },\n        \"cardNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Masked card number\"\n        },\n        \"cardType\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"expiryMonth\": {\n          \"type\": \"string\"\n        },\n        \"expiryYear\": {\n          \"type\": \"string\"\n        },\n        \"billingAddress\": {\n          \"$ref\": \"#/$defs/Address\"\n       \
  \ }\n      }\n    },\n    \"Voucher\": {\n      \"type\": \"object\",\n      \"description\": \"Applied voucher or coupon\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"value\": {\n          \"type\": \"number\"\n        },\n        \"freeShipping\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"PromotionResult\": {\n      \"type\": \"object\",\n      \"description\": \"Applied promotion details\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"promotion\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\"\n            },\n            \"title\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"Principal\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Cart owner\",\n      \"properties\": {\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"User identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/json-schema/sap-commerce-cloud-cart-schema.json
tags:
- B2B
- B2C
- Commerce
- Customer Experience
- Ecommerce
- Omnichannel
- Retail
title: SAP Commerce Cloud Cart
---
