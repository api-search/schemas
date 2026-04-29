---
description: ShippingLocation schema from Adyen API
layout: schema
name: ShippingLocation
properties_list:
- description: The address details of the shipping location.
  name: address
  type: object
- description: The contact details for the shipping location.
  name: contact
  type: object
- description: The unique identifier of the shipping location, for use as `shippingLocationId` when creating an order.
  name: id
  type: string
- description: The unique name of the shipping location.
  name: name
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-shipping-location-schema.json
slug: management-shipping-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-shipping-location-schema.json\",\n  \"title\": \"ShippingLocation\",\n  \"description\": \"ShippingLocation schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"description\": \"The address details of the shipping location.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"contact\": {\n      \"description\": \"The contact details for the shipping location.\",\n      \"$ref\": \"#/components/schemas/Contact\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the shipping location, for use as `shippingLocationId` when creating an order.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The unique name of the shipping location.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-shipping-location-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ShippingLocation
---
