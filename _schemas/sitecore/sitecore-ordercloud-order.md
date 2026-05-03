---
description: Schema representing an order in the Sitecore OrderCloud commerce platform. Orders capture the full lifecycle of a purchase transaction from creation through fulfillment, including line items, payment, shipping, and promotions.
layout: schema
name: Sitecore OrderCloud Order
properties_list:
- description: The unique identifier of the order, either system-generated or provided at creation
  name: ID
  type: string
- description: The user who created or owns the order
  name: FromUser
  type: object
- description: The identifier of the user who placed the order
  name: FromUserID
  type: string
- description: The identifier of the billing address for this order
  name: BillingAddressID
  type: string
- description: The billing address details for this order
  name: BillingAddress
  type: object
- description: The identifier of the shipping address for this order
  name: ShippingAddressID
  type: string
- description: Free-form comments attached to the order by the buyer or administrator
  name: Comments
  type: string
- description: The total number of distinct line items in this order
  name: LineItemCount
  type: integer
- description: The current workflow status of the order
  name: Status
  type: string
- description: The ISO 8601 timestamp when the order was first created
  name: DateCreated
  type: string
- description: The ISO 8601 timestamp when the order was submitted for fulfillment
  name: DateSubmitted
  type: string
- description: The ISO 8601 timestamp when the order was approved (for orders requiring approval)
  name: DateApproved
  type: string
- description: The ISO 8601 timestamp when the order was declined by an approver
  name: DateDeclined
  type: string
- description: The ISO 8601 timestamp when the order was canceled
  name: DateCanceled
  type: string
- description: The ISO 8601 timestamp when the order was fulfilled and marked complete
  name: DateCompleted
  type: string
- description: The order subtotal calculated from line item prices before promotions, shipping, and tax
  name: Subtotal
  type: number
- description: The total shipping cost applied to the order
  name: ShippingCost
  type: number
- description: The total tax amount calculated for the order
  name: TaxCost
  type: number
- description: The total discount amount subtracted from the order by applied promotions
  name: PromotionDiscount
  type: number
- description: The final order total after adding shipping, tax, and subtracting promotions
  name: Total
  type: number
- description: Whether the order has been submitted for fulfillment
  name: IsSubmitted
  type: boolean
- description: Extended properties for storing custom order-level attributes not covered by the standard schema
  name: xp
  type: object
provider_name: sitecore
provider_slug: sitecore
schema_file: json-schema/sitecore-ordercloud-order-schema.json
slug: sitecore-ordercloud-order
source_filename: sitecore-ordercloud-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://sitecore.com/schemas/ordercloud/order.json\",\n  \"title\": \"Sitecore OrderCloud Order\",\n  \"description\": \"Schema representing an order in the Sitecore OrderCloud commerce platform. Orders capture the full lifecycle of a purchase transaction from creation through fulfillment, including line items, payment, shipping, and promotions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the order, either system-generated or provided at creation\"\n    },\n    \"FromUser\": {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"The user who created or owns the order\"\n    },\n    \"FromUserID\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user who placed the order\"\n    },\n    \"BillingAddressID\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The identifier of the billing address for this order\"\n    },\n    \"BillingAddress\": {\n      \"$ref\": \"#/$defs/Address\",\n      \"description\": \"The billing address details for this order\"\n    },\n    \"ShippingAddressID\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the shipping address for this order\"\n    },\n    \"Comments\": {\n      \"type\": \"string\",\n      \"description\": \"Free-form comments attached to the order by the buyer or administrator\",\n      \"maxLength\": 2000\n    },\n    \"LineItemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of distinct line items in this order\",\n      \"minimum\": 0\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current workflow status of the order\",\n      \"enum\": [\n        \"Unsubmitted\",\n        \"Open\",\n        \"AwaitingApproval\",\n        \"Declined\",\n        \"Completed\",\n        \"Canceled\"\n  \
  \    ]\n    },\n    \"DateCreated\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp when the order was first created\",\n      \"format\": \"date-time\"\n    },\n    \"DateSubmitted\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp when the order was submitted for fulfillment\",\n      \"format\": \"date-time\"\n    },\n    \"DateApproved\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp when the order was approved (for orders requiring approval)\",\n      \"format\": \"date-time\"\n    },\n    \"DateDeclined\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp when the order was declined by an approver\",\n      \"format\": \"date-time\"\n    },\n    \"DateCanceled\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 8601 timestamp when the order was canceled\",\n      \"format\": \"date-time\"\n    },\n    \"DateCompleted\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The ISO 8601 timestamp when the order was fulfilled and marked complete\",\n      \"format\": \"date-time\"\n    },\n    \"Subtotal\": {\n      \"type\": \"number\",\n      \"description\": \"The order subtotal calculated from line item prices before promotions, shipping, and tax\",\n      \"format\": \"double\",\n      \"minimum\": 0\n    },\n    \"ShippingCost\": {\n      \"type\": \"number\",\n      \"description\": \"The total shipping cost applied to the order\",\n      \"format\": \"double\",\n      \"minimum\": 0\n    },\n    \"TaxCost\": {\n      \"type\": \"number\",\n      \"description\": \"The total tax amount calculated for the order\",\n      \"format\": \"double\",\n      \"minimum\": 0\n    },\n    \"PromotionDiscount\": {\n      \"type\": \"number\",\n      \"description\": \"The total discount amount subtracted from the order by applied promotions\",\n      \"format\": \"double\",\n      \"minimum\": 0\n    },\n    \"Total\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"The final order total after adding shipping, tax, and subtracting promotions\",\n      \"format\": \"double\",\n      \"minimum\": 0\n    },\n    \"IsSubmitted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the order has been submitted for fulfillment\"\n    },\n    \"xp\": {\n      \"type\": \"object\",\n      \"description\": \"Extended properties for storing custom order-level attributes not covered by the standard schema\",\n      \"additionalProperties\": true\n    }\n  },\n  \"$defs\": {\n    \"LineItem\": {\n      \"type\": \"object\",\n      \"description\": \"A product line item within an OrderCloud order\",\n      \"required\": [\"ProductID\", \"Quantity\"],\n      \"properties\": {\n        \"ID\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of this line item within the order\"\n        },\n        \"ProductID\": {\n          \"type\": \"string\",\n       \
  \   \"description\": \"The identifier of the product being purchased in this line item\"\n        },\n        \"Quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of units being purchased for this product\",\n          \"minimum\": 1\n        },\n        \"DateAdded\": {\n          \"type\": \"string\",\n          \"description\": \"The ISO 8601 timestamp when this line item was added to the order\",\n          \"format\": \"date-time\"\n        },\n        \"QuantityShipped\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of units that have been shipped for this line item\",\n          \"minimum\": 0\n        },\n        \"UnitPrice\": {\n          \"type\": \"number\",\n          \"description\": \"The price per unit for this product at the time of ordering\",\n          \"format\": \"double\",\n          \"minimum\": 0\n        },\n        \"PromotionDiscount\": {\n          \"type\": \"number\",\n          \"description\"\
  : \"The promotional discount applied to this specific line item\",\n          \"format\": \"double\",\n          \"minimum\": 0\n        },\n        \"LineTotal\": {\n          \"type\": \"number\",\n          \"description\": \"The total price for this line item (unit price multiplied by quantity, minus discounts)\",\n          \"format\": \"double\",\n          \"minimum\": 0\n        },\n        \"LineSubtotal\": {\n          \"type\": \"number\",\n          \"description\": \"The subtotal for this line item before promotions and discounts\",\n          \"format\": \"double\",\n          \"minimum\": 0\n        },\n        \"ShippingAddressID\": {\n          \"type\": \"string\",\n          \"description\": \"The shipping address identifier for this specific line item, overrides the order-level address\"\n        },\n        \"Product\": {\n          \"$ref\": \"#/$defs/LineItemProduct\",\n          \"description\": \"Snapshot of product details at the time the line item was added\"\
  \n        },\n        \"Specs\": {\n          \"type\": \"array\",\n          \"description\": \"Spec option selections that identify the specific product variant\",\n          \"items\": {\n            \"$ref\": \"#/$defs/LineItemSpec\"\n          }\n        },\n        \"xp\": {\n          \"type\": \"object\",\n          \"description\": \"Extended properties for custom line item attributes\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"LineItemProduct\": {\n      \"type\": \"object\",\n      \"description\": \"A snapshot of product information captured at the time a line item was added\",\n      \"properties\": {\n        \"ID\": {\n          \"type\": \"string\",\n          \"description\": \"The product identifier\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The product display name\"\n        },\n        \"Description\": {\n          \"type\": \"string\",\n          \"description\": \"The product\
  \ description\"\n        },\n        \"QuantityMultiplier\": {\n          \"type\": \"integer\",\n          \"description\": \"The minimum purchase quantity increment\"\n        },\n        \"ShipWeight\": {\n          \"type\": \"number\",\n          \"description\": \"The shipping weight of the product\",\n          \"format\": \"double\"\n        },\n        \"xp\": {\n          \"type\": \"object\",\n          \"description\": \"Extended properties for custom product attributes\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"LineItemSpec\": {\n      \"type\": \"object\",\n      \"description\": \"A spec option selection defining which product variant is in the line item\",\n      \"properties\": {\n        \"SpecID\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the spec (e.g., Color, Size)\"\n        },\n        \"OptionID\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the\
  \ selected spec option value\"\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"description\": \"The display value of the selected spec option\"\n        }\n      }\n    },\n    \"Payment\": {\n      \"type\": \"object\",\n      \"description\": \"A payment record associated with an order\",\n      \"properties\": {\n        \"ID\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of this payment\"\n        },\n        \"Type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of payment instrument used\",\n          \"enum\": [\"PurchaseOrder\", \"CreditCard\", \"SpendingAccount\"]\n        },\n        \"CreditCardID\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the credit card used (for CreditCard type payments)\"\n        },\n        \"SpendingAccountID\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the spending\
  \ account used\"\n        },\n        \"Description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of this payment\"\n        },\n        \"Amount\": {\n          \"type\": \"number\",\n          \"description\": \"The payment amount in the order currency\",\n          \"format\": \"double\",\n          \"minimum\": 0\n        },\n        \"Accepted\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the payment has been accepted\"\n        },\n        \"xp\": {\n          \"type\": \"object\",\n          \"description\": \"Extended properties for custom payment attributes\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A shipping or billing address for an order\",\n      \"properties\": {\n        \"ID\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the address record\"\n        },\n\
  \        \"FirstName\": {\n          \"type\": \"string\",\n          \"description\": \"The recipient's first name at this address\"\n        },\n        \"LastName\": {\n          \"type\": \"string\",\n          \"description\": \"The recipient's last name at this address\"\n        },\n        \"Company\": {\n          \"type\": \"string\",\n          \"description\": \"The company name at this address\"\n        },\n        \"Street1\": {\n          \"type\": \"string\",\n          \"description\": \"The primary street address line\"\n        },\n        \"Street2\": {\n          \"type\": \"string\",\n          \"description\": \"The secondary street address line (suite, apartment, etc.)\"\n        },\n        \"City\": {\n          \"type\": \"string\",\n          \"description\": \"The city name\"\n        },\n        \"State\": {\n          \"type\": \"string\",\n          \"description\": \"The state, province, or region code\"\n        },\n        \"Zip\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The postal or ZIP code\"\n        },\n        \"Country\": {\n          \"type\": \"string\",\n          \"description\": \"The ISO 3166-1 alpha-2 country code\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"example\": \"US\"\n        },\n        \"Phone\": {\n          \"type\": \"string\",\n          \"description\": \"The phone number at this address\"\n        },\n        \"xp\": {\n          \"type\": \"object\",\n          \"description\": \"Extended properties for custom address attributes\",\n          \"additionalProperties\": true\n        }\n      }\n    },\n    \"UserReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to the user who placed or owns the order\",\n      \"properties\": {\n        \"ID\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the user\"\n        },\n        \"FirstName\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The user's first name\"\n        },\n        \"LastName\": {\n          \"type\": \"string\",\n          \"description\": \"The user's last name\"\n        },\n        \"Username\": {\n          \"type\": \"string\",\n          \"description\": \"The user's login username\"\n        },\n        \"Email\": {\n          \"type\": \"string\",\n          \"description\": \"The user's email address\",\n          \"format\": \"email\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sitecore/refs/heads/main/json-schema/sitecore-ordercloud-order-schema.json
tags: []
title: Sitecore OrderCloud Order
---
