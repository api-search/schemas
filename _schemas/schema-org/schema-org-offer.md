---
description: An offer to transfer some rights to an item or to provide a service, for example an offer to sell tickets to an event or to rent a movie.
layout: schema
name: Schema.org Offer
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the offer.
  name: name
  type: string
- description: A description of the offer.
  name: description
  type: string
- description: URL of the offer.
  name: url
  type: string
- description: The offer price.
  name: price
  type: object
- description: The currency of the price (ISO 4217).
  name: priceCurrency
  type: string
- description: The date after which the price is no longer available.
  name: priceValidUntil
  type: string
- description: The availability of this item.
  name: availability
  type: string
- description: The beginning of the availability of the product.
  name: availabilityStarts
  type: string
- description: The end of the availability of the product.
  name: availabilityEnds
  type: string
- description: The condition of the item.
  name: itemCondition
  type: string
- description: The entity offering the item.
  name: seller
  type: object
- description: A pointer to the organization making the offer.
  name: offeredBy
  type: object
- description: The item being offered.
  name: itemOffered
  type: object
- description: The Stock Keeping Unit.
  name: sku
  type: string
- description: A Global Trade Item Number.
  name: gtin
  type: string
- description: The Manufacturer Part Number.
  name: mpn
  type: string
- description: The date when the item becomes valid.
  name: validFrom
  type: string
- description: The date after when the item is not valid.
  name: validThrough
  type: string
- description: The ISO 3166-1 (ISO 3166-1 alpha-2) or ISO 3166-2 code for the eligible region.
  name: eligibleRegion
  type: string
- description: The interval and unit of measurement of ordering quantities.
  name: eligibleQuantity
  type: object
- description: The typical delay between the receipt of the order and the goods either leaving the warehouse or being prepared for pickup.
  name: deliveryLeadTime
  type: object
- description: Indicates information about the shipping policies and options.
  name: shippingDetails
  type: object
- description: Specifies a MerchantReturnPolicy.
  name: hasMerchantReturnPolicy
  type: object
- description: A review of the offer.
  name: review
  type: object
- description: The overall rating.
  name: aggregateRating
  type: object
- description: The lowest price of all offers available (for AggregateOffer).
  name: lowPrice
  type: number
- description: The highest price of all offers available (for AggregateOffer).
  name: highPrice
  type: number
- description: The number of offers for the product (for AggregateOffer).
  name: offerCount
  type: integer
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-offer-schema.json
slug: schema-org-offer
source_filename: schema-org-offer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/offer.json\",\n  \"title\": \"Schema.org Offer\",\n  \"description\": \"An offer to transfer some rights to an item or to provide a service, for example an offer to sell tickets to an event or to rent a movie.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"Offer\", \"AggregateOffer\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the offer.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the offer.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the offer.\"\
  \n    },\n    \"price\": {\n      \"oneOf\": [\n        { \"type\": \"number\" },\n        { \"type\": \"string\" }\n      ],\n      \"description\": \"The offer price.\"\n    },\n    \"priceCurrency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"The currency of the price (ISO 4217).\"\n    },\n    \"priceValidUntil\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date after which the price is no longer available.\"\n    },\n    \"availability\": {\n      \"type\": \"string\",\n      \"enum\": [\"BackOrder\", \"Discontinued\", \"InStock\", \"InStoreOnly\", \"LimitedAvailability\", \"OnlineOnly\", \"OutOfStock\", \"PreOrder\", \"PreSale\", \"SoldOut\"],\n      \"description\": \"The availability of this item.\"\n    },\n    \"availabilityStarts\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The beginning of the availability of the product.\"\n    },\n\
  \    \"availabilityEnds\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The end of the availability of the product.\"\n    },\n    \"itemCondition\": {\n      \"type\": \"string\",\n      \"enum\": [\"DamagedCondition\", \"NewCondition\", \"RefurbishedCondition\", \"UsedCondition\"],\n      \"description\": \"The condition of the item.\"\n    },\n    \"seller\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The entity offering the item.\"\n    },\n    \"offeredBy\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"A pointer to the organization making the offer.\"\n    },\n    \"itemOffered\": {\n      \"type\": \"object\",\n      \"description\": \"The item being offered.\",\n     \
  \ \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"The Stock Keeping Unit.\"\n    },\n    \"gtin\": {\n      \"type\": \"string\",\n      \"description\": \"A Global Trade Item Number.\"\n    },\n    \"mpn\": {\n      \"type\": \"string\",\n      \"description\": \"The Manufacturer Part Number.\"\n    },\n    \"validFrom\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date when the item becomes valid.\"\n    },\n    \"validThrough\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date after when the item is not valid.\"\n    },\n    \"eligibleRegion\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 3166-1 (ISO 3166-1 alpha-2) or ISO 3166-2 code for the eligible region.\"\n    },\n    \"eligibleQuantity\": {\n      \"type\": \"\
  object\",\n      \"description\": \"The interval and unit of measurement of ordering quantities.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"QuantitativeValue\" },\n        \"value\": { \"type\": \"number\" },\n        \"minValue\": { \"type\": \"number\" },\n        \"maxValue\": { \"type\": \"number\" },\n        \"unitCode\": { \"type\": \"string\" }\n      }\n    },\n    \"deliveryLeadTime\": {\n      \"type\": \"object\",\n      \"description\": \"The typical delay between the receipt of the order and the goods either leaving the warehouse or being prepared for pickup.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"QuantitativeValue\" },\n        \"value\": { \"type\": \"number\" },\n        \"unitCode\": { \"type\": \"string\" }\n      }\n    },\n    \"shippingDetails\": {\n      \"$ref\": \"#/$defs/OfferShippingDetails\",\n      \"description\": \"Indicates information about the shipping policies and\
  \ options.\"\n    },\n    \"hasMerchantReturnPolicy\": {\n      \"$ref\": \"#/$defs/MerchantReturnPolicy\",\n      \"description\": \"Specifies a MerchantReturnPolicy.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A review of the offer.\"\n    },\n    \"aggregateRating\": {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating.\"\n    },\n    \"lowPrice\": {\n      \"type\": \"number\",\n      \"description\": \"The lowest price of all offers available (for AggregateOffer).\"\n    },\n    \"highPrice\": {\n      \"type\": \"number\",\n      \"description\": \"The highest price of all offers available (for AggregateOffer).\"\n    },\n    \"offerCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of offers for the product (for\
  \ AggregateOffer).\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  },\n  \"$defs\": {\n    \"OfferShippingDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Shipping details for an offer.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"OfferShippingDetails\" },\n        \"shippingRate\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"@type\": { \"const\": \"MonetaryAmount\" },\n            \"value\": { \"type\": \"number\" },\n            \"currency\": { \"type\": \"string\" }\n          }\n        },\n        \"shippingDestination\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"@type\": { \"const\"\
  : \"DefinedRegion\" },\n            \"addressCountry\": { \"type\": \"string\" }\n          }\n        },\n        \"deliveryTime\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"@type\": { \"const\": \"ShippingDeliveryTime\" },\n            \"handlingTime\": { \"type\": \"object\" },\n            \"transitTime\": { \"type\": \"object\" }\n          }\n        }\n      }\n    },\n    \"MerchantReturnPolicy\": {\n      \"type\": \"object\",\n      \"description\": \"A MerchantReturnPolicy.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MerchantReturnPolicy\" },\n        \"applicableCountry\": { \"type\": \"string\" },\n        \"returnPolicyCategory\": { \"type\": \"string\", \"enum\": [\"MerchantReturnFiniteReturnWindow\", \"MerchantReturnNotPermitted\", \"MerchantReturnUnlimitedWindow\", \"MerchantReturnUnspecified\"] },\n        \"merchantReturnDays\": { \"type\": \"integer\" },\n        \"returnMethod\": { \"type\"\
  : \"string\", \"enum\": [\"ReturnAtKiosk\", \"ReturnByMail\", \"ReturnInStore\"] },\n        \"returnFees\": { \"type\": \"string\", \"enum\": [\"FreeReturn\", \"OriginalShippingFees\", \"RestockingFees\", \"ReturnFeesCustomerResponsibility\", \"ReturnShippingFees\"] }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-offer-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org Offer
---
