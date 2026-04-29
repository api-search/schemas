---
description: Information about an address.
layout: schema
name: Address
properties_list:
- description: ''
  name: ContactName
  type: object
- description: ''
  name: ContactPhoneNumber
  type: object
- description: ''
  name: AddressLine1
  type: object
- description: ''
  name: AddressLine2
  type: object
- description: ''
  name: AddressLine3
  type: object
- description: ''
  name: City
  type: object
- description: ''
  name: StateOrRegion
  type: object
- description: ''
  name: DistrictOrCounty
  type: object
- description: ''
  name: PostalCode
  type: object
- description: ''
  name: CountryCode
  type: object
- description: ''
  name: Municipality
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-address-schema.json
slug: openapi-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \" Information about an address. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ContactName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContactName\"\n        },\n        {\n          \"description\": \"The name of the contact.\"\n        }\n      ]\n    },\n    \"ContactPhoneNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContactPhoneNumber\"\n        },\n        {\n          \"description\": \"The phone number of the contact.\"\n        }\n      ]\n    },\n    \"AddressLine1\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressLine1\"\n        },\n        {\n          \"description\": \"The first line of the\
  \ address.\"\n        }\n      ]\n    },\n    \"AddressLine2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressLine2\"\n        },\n        {\n          \"description\": \"The second line of the address.\"\n        }\n      ]\n    },\n    \"AddressLine3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressLine3\"\n        },\n        {\n          \"description\": \"The third line of the address.\"\n        }\n      ]\n    },\n    \"City\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/City\"\n        },\n        {\n          \"description\": \"The city for the address.\"\n        }\n      ]\n    },\n    \"StateOrRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateOrRegion\"\n        },\n        {\n          \"description\": \"The state for the address.\"\n        }\n      ]\n    },\n    \"DistrictOrCounty\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/DistrictOrCounty\"\n        },\n        {\n          \"description\": \"The district or county for the address.\"\n        }\n      ]\n    },\n    \"PostalCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PostalCode\"\n        },\n        {\n          \"description\": \"The postal code for the address.\"\n        }\n      ]\n    },\n    \"CountryCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountryCode\"\n        },\n        {\n          \"description\": \"The ISO-3166 two-letter country code for the address.\"\n        }\n      ]\n    },\n    \"Municipality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Municipality\"\n        },\n        {\n          \"description\": \"The municipality for the address.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AddressLine1\",\n    \"City\",\n    \"StateOrRegion\",\n    \"PostalCode\",\n\
  \    \"CountryCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-address-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: Address
---
