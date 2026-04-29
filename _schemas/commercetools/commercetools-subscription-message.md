---
description: A message notification payload delivered by the commercetools Subscriptions system to external message queue destinations. Messages are generated when predefined domain events occur (e.g., OrderCreated, CustomerCreated, ProductPublished) and include common metadata plus a type-specific payload.
layout: schema
name: commercetools Subscription Message
properties_list:
- description: System-generated unique identifier for the message.
  name: id
  type: string
- description: Version number of the message record.
  name: version
  type: integer
- description: Monotonically increasing sequence number scoped to the resource for ordered processing.
  name: sequenceNumber
  type: integer
- description: Reference to the resource that generated this message.
  name: resource
  type: object
- description: Version of the resource at the time the message was generated.
  name: resourceVersion
  type: integer
- description: User-defined identifiers of the resource (e.g., key, orderNumber, sku).
  name: resourceUserProvidedIdentifiers
  type: object
- description: The message type discriminator identifying the specific event (e.g., OrderCreated, CustomerCreated).
  name: type
  type: string
- description: ISO 8601 timestamp when the message was created.
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the message record was last modified.
  name: lastModifiedAt
  type: string
- description: Actor who triggered the event that generated this message.
  name: createdBy
  type: object
- description: Actor who last modified this message record.
  name: lastModifiedBy
  type: object
provider_name: commercetools
provider_slug: commercetools
schema_file: json-schema/commercetools-subscription-message-schema.json
slug: commercetools-subscription-message
source_filename: commercetools-subscription-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/schemas/commercetools/subscription-message.json\",\n  \"title\": \"commercetools Subscription Message\",\n  \"description\": \"A message notification payload delivered by the commercetools Subscriptions system to external message queue destinations. Messages are generated when predefined domain events occur (e.g., OrderCreated, CustomerCreated, ProductPublished) and include common metadata plus a type-specific payload.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"version\", \"sequenceNumber\", \"resource\", \"resourceVersion\", \"type\", \"createdAt\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated unique identifier for the message.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Version number of the message record.\"\n    },\n\
  \    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Monotonically increasing sequence number scoped to the resource for ordered processing.\"\n    },\n    \"resource\": {\n      \"$ref\": \"#/$defs/Reference\",\n      \"description\": \"Reference to the resource that generated this message.\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Version of the resource at the time the message was generated.\"\n    },\n    \"resourceUserProvidedIdentifiers\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined identifiers of the resource (e.g., key, orderNumber, sku).\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The user-defined key of the resource, if set.\"\n        },\n        \"orderNumber\": {\n          \"type\": \"string\",\n          \"description\": \"The order number of the resource\
  \ if it is an order.\"\n        },\n        \"sku\": {\n          \"type\": \"string\",\n          \"description\": \"The SKU of the resource if it is an inventory entry or price.\"\n        },\n        \"slug\": {\n          \"type\": \"object\",\n          \"description\": \"The localized slug map if the resource is a product or category.\"\n        }\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The message type discriminator identifying the specific event (e.g., OrderCreated, CustomerCreated).\",\n      \"enum\": [\n        \"OrderCreated\",\n        \"OrderStateChanged\",\n        \"OrderPaymentStateChanged\",\n        \"OrderShipmentStateChanged\",\n        \"OrderImported\",\n        \"DeliveryAdded\",\n        \"DeliveryAddressSet\",\n        \"DeliveryItemsUpdated\",\n        \"ParcelAddedToDelivery\",\n        \"ParcelTrackingDataUpdated\",\n        \"ReturnInfoAdded\",\n        \"OrderLineItemAdded\",\n        \"OrderLineItemRemoved\"\
  ,\n        \"CustomerCreated\",\n        \"CustomerPasswordChanged\",\n        \"CustomerPasswordUpdated\",\n        \"CustomerEmailChanged\",\n        \"CustomerEmailVerified\",\n        \"CustomerGroupSet\",\n        \"CustomerAddressAdded\",\n        \"CustomerAddressChanged\",\n        \"CustomerAddressRemoved\",\n        \"ProductPublished\",\n        \"ProductUnpublished\",\n        \"ProductCreated\",\n        \"ProductDeleted\",\n        \"ProductVariantAdded\",\n        \"ProductVariantDeleted\",\n        \"InventoryEntryCreated\",\n        \"InventoryEntryDeleted\",\n        \"InventoryEntryQuantitySet\",\n        \"PaymentCreated\",\n        \"PaymentStatusInterfaceCodeSet\",\n        \"PaymentTransactionAdded\",\n        \"PaymentTransactionStateChanged\",\n        \"ApprovalRuleApproved\",\n        \"ApprovalRuleRejected\",\n        \"QuoteRequestCreated\",\n        \"QuoteCreated\",\n        \"ReviewCreated\",\n        \"ReviewRatingSet\",\n        \"StoreCreated\",\n   \
  \     \"StoreDeleted\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the message was created.\"\n    },\n    \"lastModifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the message record was last modified.\"\n    },\n    \"createdBy\": {\n      \"$ref\": \"#/$defs/LastModifiedBy\",\n      \"description\": \"Actor who triggered the event that generated this message.\"\n    },\n    \"lastModifiedBy\": {\n      \"$ref\": \"#/$defs/LastModifiedBy\",\n      \"description\": \"Actor who last modified this message record.\"\n    }\n  },\n  \"$defs\": {\n    \"Reference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to another commercetools resource by type and ID.\",\n      \"required\": [\"typeId\", \"id\"],\n      \"properties\": {\n        \"typeId\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"The type identifier of the referenced resource (e.g., 'order', 'product', 'customer').\",\n          \"enum\": [\n            \"cart\",\n            \"cart-discount\",\n            \"category\",\n            \"channel\",\n            \"customer\",\n            \"customer-group\",\n            \"discount-code\",\n            \"inventory-entry\",\n            \"order\",\n            \"order-edit\",\n            \"payment\",\n            \"product\",\n            \"product-discount\",\n            \"product-selection\",\n            \"product-type\",\n            \"quote\",\n            \"quote-request\",\n            \"review\",\n            \"shipping-method\",\n            \"shopping-list\",\n            \"staged-quote\",\n            \"standalone-price\",\n            \"state\",\n            \"store\",\n            \"tax-category\",\n            \"type\",\n            \"zone\"\n          ]\n        },\n        \"id\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"System-generated unique identifier of the referenced resource.\"\n        }\n      }\n    },\n    \"LastModifiedBy\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the actor who triggered or last modified the event.\",\n      \"properties\": {\n        \"clientId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the API client used to trigger the event.\"\n        },\n        \"externalUserId\": {\n          \"type\": \"string\",\n          \"description\": \"External user identifier set on the API client token.\"\n        },\n        \"customer\": {\n          \"$ref\": \"#/$defs/Reference\",\n          \"description\": \"Reference to the customer who triggered the event, if any.\"\n        },\n        \"anonymousId\": {\n          \"type\": \"string\",\n          \"description\": \"Anonymous session ID if the event was triggered without a customer login.\"\n        },\n        \"isPlatformClient\": {\n\
  \          \"type\": \"boolean\",\n          \"description\": \"Whether the event was triggered via the Merchant Center interface.\"\n        }\n      }\n    },\n    \"ChangeNotification\": {\n      \"type\": \"object\",\n      \"description\": \"A change notification payload for resource create, update, and delete events delivered via changes subscriptions.\",\n      \"required\": [\"notificationType\", \"projectKey\", \"resource\", \"resourceUserProvidedIdentifiers\", \"version\", \"oldVersion\", \"modifiedAt\"],\n      \"properties\": {\n        \"notificationType\": {\n          \"type\": \"string\",\n          \"enum\": [\"ResourceCreated\", \"ResourceUpdated\", \"ResourceDeleted\"],\n          \"description\": \"The type of modification that triggered the change notification.\"\n        },\n        \"projectKey\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the project in which the change occurred.\"\n        },\n        \"resource\": {\n         \
  \ \"$ref\": \"#/$defs/Reference\",\n          \"description\": \"Reference to the resource that was created, updated, or deleted.\"\n        },\n        \"resourceUserProvidedIdentifiers\": {\n          \"type\": \"object\",\n          \"description\": \"User-defined identifiers of the changed resource.\"\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"New version of the resource after the change.\"\n        },\n        \"oldVersion\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Version of the resource before the change (0 for newly created resources).\"\n        },\n        \"modifiedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the change was applied.\"\n        },\n        \"changes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\
  \n          },\n          \"description\": \"List of individual field-level changes applied in this operation.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/json-schema/commercetools-subscription-message-schema.json
tags:
- Commerce
- Composable Commerce
- E-Commerce
- GraphQL
- REST
- SDK
title: commercetools Subscription Message
---
