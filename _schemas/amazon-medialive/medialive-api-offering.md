---
description: Reserved resources available for purchase
layout: schema
name: Offering
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CurrencyCode
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: DurationUnits
  type: object
- description: ''
  name: FixedPrice
  type: object
- description: ''
  name: OfferingDescription
  type: object
- description: ''
  name: OfferingId
  type: object
- description: ''
  name: OfferingType
  type: object
- description: ''
  name: Region
  type: object
- description: ''
  name: ResourceSpecification
  type: object
- description: ''
  name: UsagePrice
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-offering-schema.json
slug: medialive-api-offering
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-offering-schema.json\",\n  \"title\": \"Offering\",\n  \"description\": \"Reserved resources available for purchase\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"Unique offering ARN, e.g. 'arn:aws:medialive:us-west-2:123456789012:offering:87654321'\"\n        }\n      ]\n    },\n    \"CurrencyCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currencyCode\"\n          },\n          \"description\": \"Currency code for usagePrice and fixedPrice in ISO-4217\
  \ format, e.g. 'USD'\"\n        }\n      ]\n    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"duration\"\n          },\n          \"description\": \"Lease duration, e.g. '12'\"\n        }\n      ]\n    },\n    \"DurationUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OfferingDurationUnits\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"durationUnits\"\n          },\n          \"description\": \"Units for duration, e.g. 'MONTHS'\"\n        }\n      ]\n    },\n    \"FixedPrice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fixedPrice\"\n          },\n          \"description\": \"One-time charge for each reserved resource, e.g. '0.0' for a NO_UPFRONT offering\"\n        }\n      ]\n\
  \    },\n    \"OfferingDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offeringDescription\"\n          },\n          \"description\": \"Offering description, e.g. 'HD AVC output at 10-20 Mbps, 30 fps, and standard VQ in US West (Oregon)'\"\n        }\n      ]\n    },\n    \"OfferingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offeringId\"\n          },\n          \"description\": \"Unique offering ID, e.g. '87654321'\"\n        }\n      ]\n    },\n    \"OfferingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OfferingType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offeringType\"\n          },\n          \"description\": \"Offering type, e.g. 'NO_UPFRONT'\"\n        }\n      ]\n   \
  \ },\n    \"Region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"region\"\n          },\n          \"description\": \"AWS region, e.g. 'us-west-2'\"\n        }\n      ]\n    },\n    \"ResourceSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservationResourceSpecification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceSpecification\"\n          },\n          \"description\": \"Resource configuration details\"\n        }\n      ]\n    },\n    \"UsagePrice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"usagePrice\"\n          },\n          \"description\": \"Recurring usage charge for each reserved resource, e.g. '157.0'\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-offering-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Offering
---
