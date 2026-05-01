---
description: The address that you want the Snow device(s) associated with a specific job to be shipped to. Addresses are validated at the time of creation. The address you provide must be located within the serviceable area of your region. Although no individual elements of the <code>Address</code> are required, if the address is invalid or unsupported, then an exception is thrown.
layout: schema
name: Address
properties_list:
- description: ''
  name: AddressId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Company
  type: object
- description: ''
  name: Street1
  type: object
- description: ''
  name: Street2
  type: object
- description: ''
  name: Street3
  type: object
- description: ''
  name: City
  type: object
- description: ''
  name: StateOrProvince
  type: object
- description: ''
  name: PrefectureOrDistrict
  type: object
- description: ''
  name: Landmark
  type: object
- description: ''
  name: Country
  type: object
- description: ''
  name: PostalCode
  type: object
- description: ''
  name: PhoneNumber
  type: object
- description: ''
  name: IsRestricted
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-address-schema.json
slug: amazon-snow-family-address
source_filename: amazon-snow-family-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"The address that you want the Snow device(s) associated with a specific job to be shipped to. Addresses are validated at the time of creation. The address you provide must be located within the serviceable area of your region. Although no individual elements of the <code>Address</code> are required, if the address is invalid or unsupported, then an exception is thrown.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The unique ID for an address.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The name of a person to receive a Snow device at an address.\"\n        }\n      ]\n    },\n    \"Company\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the company to receive a Snow device at an address.\"\n        }\n      ]\n    },\n    \"Street1\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The first line in a street address that a Snow device is to be delivered to.\"\n        }\n      ]\n    },\n    \"Street2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The second line in a street address that a Snow device is to be delivered to.\"\n        }\n      ]\n    },\n    \"Street3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/String\"\n        },\n        {\n          \"description\": \"The third line in a street address that a Snow device is to be delivered to.\"\n        }\n      ]\n    },\n    \"City\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The city in an address that a Snow device is to be delivered to.\"\n        }\n      ]\n    },\n    \"StateOrProvince\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The state or province in an address that a Snow device is to be delivered to.\"\n        }\n      ]\n    },\n    \"PrefectureOrDistrict\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"This field is no longer used and the value is ignored.\"\n        }\n      ]\n    },\n    \"Landmark\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"This field is no longer used and the value is ignored.\"\n        }\n      ]\n    },\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The country in an address that a Snow device is to be delivered to.\"\n        }\n      ]\n    },\n    \"PostalCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The postal code in an address that a Snow device is to be delivered to.\"\n        }\n      ]\n    },\n    \"PhoneNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The phone number associated with an address that a Snow device is to be delivered to.\"\n        }\n      ]\n    },\n\
  \    \"IsRestricted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"If the address you are creating is a primary address, then set this option to true. This field is not supported in most regions.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressType\"\n        },\n        {\n          \"description\": \"Differentiates between delivery address and pickup address in the customer account. Provided at job creation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-address-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: Address
---
