---
description: An order in SAP Commerce Cloud representing a completed purchase transaction with line items, delivery information, payment details, and fulfillment status.
layout: schema
name: SAP Commerce Cloud Order
properties_list:
- description: Unique order code
  name: code
  type: string
- description: Order processing status
  name: status
  type: string
- description: Human-readable order status
  name: statusDisplay
  type: string
- description: Order creation timestamp
  name: created
  type: string
- description: Total number of distinct items in the order
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
- description: Order line items
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
- description: Shipment consignments for fulfillment tracking
  name: consignments
  type: array
- description: ''
  name: user
  type: object
- description: Promotions applied at the order level
  name: appliedOrderPromotions
  type: array
- description: Promotions applied at the product level
  name: appliedProductPromotions
  type: array
- description: Vouchers applied to the order
  name: appliedVouchers
  type: array
provider_name: SAP Commerce Cloud
provider_slug: sap-commerce-cloud
schema_file: json-schema/sap-commerce-cloud-order-schema.json
slug: sap-commerce-cloud-order
source_filename: sap-commerce-cloud-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-commerce-cloud/order.json\",\n  \"title\": \"SAP Commerce Cloud Order\",\n  \"description\": \"An order in SAP Commerce Cloud representing a completed purchase transaction with line items, delivery information, payment details, and fulfillment status.\",\n  \"type\": \"object\",\n  \"required\": [\"code\"],\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order code\",\n      \"minLength\": 1\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Order processing status\"\n    },\n    \"statusDisplay\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable order status\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Order creation timestamp\"\n    },\n    \"totalItems\": {\n      \"type\": \"integer\"\
  ,\n      \"minimum\": 0,\n      \"description\": \"Total number of distinct items in the order\"\n    },\n    \"totalUnitCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total quantity of units across all entries\"\n    },\n    \"subTotal\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"deliveryCost\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"totalTax\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"totalPrice\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"totalPriceWithTax\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"totalDiscounts\": {\n      \"$ref\": \"#/$defs/Price\"\n    },\n    \"entries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/OrderEntry\"\n      },\n      \"description\": \"Order line items\"\n    },\n    \"deliveryAddress\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"deliveryMode\": {\n      \"$ref\": \"#/$defs/DeliveryMode\"\n    },\n    \"paymentInfo\"\
  : {\n      \"$ref\": \"#/$defs/PaymentDetails\"\n    },\n    \"consignments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Consignment\"\n      },\n      \"description\": \"Shipment consignments for fulfillment tracking\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/Principal\"\n    },\n    \"appliedOrderPromotions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PromotionResult\"\n      },\n      \"description\": \"Promotions applied at the order level\"\n    },\n    \"appliedProductPromotions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PromotionResult\"\n      },\n      \"description\": \"Promotions applied at the product level\"\n    },\n    \"appliedVouchers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Voucher\"\n      },\n      \"description\": \"Vouchers applied to the order\"\n    }\n  },\n  \"$defs\": {\n    \"Price\": {\n      \"\
  type\": \"object\",\n      \"description\": \"Price or monetary amount\",\n      \"properties\": {\n        \"currencyIso\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"ISO 4217 currency code\"\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"Numeric value\"\n        },\n        \"formattedValue\": {\n          \"type\": \"string\",\n          \"description\": \"Locale-formatted value string\"\n        }\n      }\n    },\n    \"OrderEntry\": {\n      \"type\": \"object\",\n      \"description\": \"Individual line item in an order\",\n      \"properties\": {\n        \"entryNumber\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Zero-based entry number\"\n        },\n        \"product\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"Product code\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Product name\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"description\": \"Product URL\"\n            }\n          }\n        },\n        \"quantity\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Ordered quantity\"\n        },\n        \"basePrice\": {\n          \"$ref\": \"#/$defs/Price\"\n        },\n        \"totalPrice\": {\n          \"$ref\": \"#/$defs/Price\"\n        },\n        \"updateable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the entry can still be modified\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"Physical address\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Address identifier\"\n \
  \       },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"First name\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"description\": \"Last name\"\n        },\n        \"line1\": {\n          \"type\": \"string\",\n          \"description\": \"Address line 1\"\n        },\n        \"line2\": {\n          \"type\": \"string\",\n          \"description\": \"Address line 2\"\n        },\n        \"town\": {\n          \"type\": \"string\",\n          \"description\": \"City or town\"\n        },\n        \"region\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isocode\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code\"\n        },\n        \"country\": {\n         \
  \ \"type\": \"object\",\n          \"properties\": {\n            \"isocode\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address\"\n        }\n      }\n    },\n    \"DeliveryMode\": {\n      \"type\": \"object\",\n      \"description\": \"Delivery or shipping method\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Delivery mode code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Delivery mode name\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Delivery mode description\"\n\
  \        },\n        \"deliveryCost\": {\n          \"$ref\": \"#/$defs/Price\"\n        }\n      }\n    },\n    \"PaymentDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Payment method details\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Payment details identifier\"\n        },\n        \"accountHolderName\": {\n          \"type\": \"string\",\n          \"description\": \"Card holder name\"\n        },\n        \"cardNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Masked card number\"\n        },\n        \"cardType\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"expiryMonth\": {\n          \"type\": \"string\",\n          \"description\": \"Card expiry month\"\n       \
  \ },\n        \"expiryYear\": {\n          \"type\": \"string\",\n          \"description\": \"Card expiry year\"\n        },\n        \"billingAddress\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n    },\n    \"Consignment\": {\n      \"type\": \"object\",\n      \"description\": \"Shipment consignment for order fulfillment\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Consignment code\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Consignment status\"\n        },\n        \"statusDisplay\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable status\"\n        },\n        \"trackingID\": {\n          \"type\": \"string\",\n          \"description\": \"Carrier tracking ID\"\n        },\n        \"entries\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"quantity\": {\n                \"type\": \"integer\"\n              },\n              \"shippedQuantity\": {\n                \"type\": \"integer\"\n              },\n              \"orderEntry\": {\n                \"$ref\": \"#/$defs/OrderEntry\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"Principal\": {\n      \"type\": \"object\",\n      \"description\": \"User or principal reference\",\n      \"properties\": {\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"User unique identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name\"\n        }\n      }\n    },\n    \"PromotionResult\": {\n      \"type\": \"object\",\n      \"description\": \"Applied promotion result\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Promotion description\"\n        },\n        \"promotion\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\"\n            },\n            \"title\": {\n              \"type\": \"string\"\n            },\n            \"description\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"Voucher\": {\n      \"type\": \"object\",\n      \"description\": \"Applied voucher\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Voucher code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Voucher name\"\n        },\n        \"value\": {\n          \"type\": \"number\",\n          \"description\": \"Voucher value\"\n        },\n        \"freeShipping\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the voucher provides free shipping\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/json-schema/sap-commerce-cloud-order-schema.json
tags:
- B2B
- B2C
- Commerce
- Customer Experience
- Ecommerce
- Omnichannel
- Retail
title: SAP Commerce Cloud Order
---
