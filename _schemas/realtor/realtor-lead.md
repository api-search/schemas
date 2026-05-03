---
description: Schema representing a real estate lead delivered from Realtor.com to a CRM system via the Connections Plus or Lead Delivery API. Captures buyer and seller lead contact information, associated property details, financial qualification data, and transaction likelihood scores.
layout: schema
name: Realtor.com Lead
properties_list:
- description: Unique identifier for the lead assigned by Realtor.com.
  name: lead_id
  type: string
- description: Role of the lead indicating whether they are a buyer or seller.
  name: role
  type: string
- description: ''
  name: contact
  type: object
- description: ''
  name: property
  type: object
- description: ''
  name: finance_info
  type: object
- description: ''
  name: listing_agent
  type: object
- description: Source of the lead on Realtor.com such as listing page, search results, or recommendation.
  name: source
  type: string
- description: Optional message from the consumer expressing their interest or asking questions.
  name: message
  type: string
- description: Indicator of whether the lead is likely to complete a real estate transaction.
  name: is_likely_to_transact
  type: boolean
- description: Probability score from 0 to 1 indicating how likely the lead is to complete a transaction.
  name: probability_to_transact
  type: number
- description: ISO 8601 timestamp when the lead was generated.
  name: timestamp
  type: string
- description: Optional digital signature for verifying the authenticity and integrity of the lead data.
  name: digital_signature
  type: string
provider_name: realtor
provider_slug: realtor
schema_file: json-schema/realtor-lead-schema.json
slug: realtor-lead
source_filename: realtor-lead-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://realtor.com/schemas/realtor/lead.json\",\n  \"title\": \"Realtor.com Lead\",\n  \"description\": \"Schema representing a real estate lead delivered from Realtor.com to a CRM system via the Connections Plus or Lead Delivery API. Captures buyer and seller lead contact information, associated property details, financial qualification data, and transaction likelihood scores.\",\n  \"type\": \"object\",\n  \"required\": [\"lead_id\", \"role\", \"contact\", \"timestamp\"],\n  \"properties\": {\n    \"lead_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the lead assigned by Realtor.com.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"Role of the lead indicating whether they are a buyer or seller.\",\n      \"enum\": [\"buyer\", \"seller\"]\n    },\n    \"contact\": {\n      \"$ref\": \"#/$defs/Contact\"\n    },\n    \"property\"\
  : {\n      \"$ref\": \"#/$defs/Property\"\n    },\n    \"finance_info\": {\n      \"$ref\": \"#/$defs/FinanceInfo\"\n    },\n    \"listing_agent\": {\n      \"$ref\": \"#/$defs/ListingAgent\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source of the lead on Realtor.com such as listing page, search results, or recommendation.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Optional message from the consumer expressing their interest or asking questions.\"\n    },\n    \"is_likely_to_transact\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicator of whether the lead is likely to complete a real estate transaction.\"\n    },\n    \"probability_to_transact\": {\n      \"type\": \"number\",\n      \"description\": \"Probability score from 0 to 1 indicating how likely the lead is to complete a transaction.\",\n      \"minimum\": 0,\n      \"maximum\": 1\n    },\n    \"timestamp\": {\n      \"type\": \"\
  string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the lead was generated.\"\n    },\n    \"digital_signature\": {\n      \"type\": \"string\",\n      \"description\": \"Optional digital signature for verifying the authenticity and integrity of the lead data.\"\n    }\n  },\n  \"$defs\": {\n    \"Contact\": {\n      \"type\": \"object\",\n      \"description\": \"Contact information for the lead.\",\n      \"required\": [\"email\"],\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the lead.\",\n          \"maxLength\": 100\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the lead.\",\n          \"maxLength\": 100\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address of the lead.\"\n        },\n        \"phone\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Phone number of the lead.\",\n          \"pattern\": \"^[+]?[0-9\\\\-\\\\s()]+$\"\n        }\n      }\n    },\n    \"Property\": {\n      \"type\": \"object\",\n      \"description\": \"Property information associated with the lead.\",\n      \"properties\": {\n        \"listing_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the property listing on Realtor.com.\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Full street address of the property.\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City where the property is located.\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter state abbreviation.\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"minLength\": 2,\n          \"maxLength\": 2\n \
  \       },\n        \"zip_code\": {\n          \"type\": \"string\",\n          \"description\": \"Five-digit ZIP code of the property.\",\n          \"pattern\": \"^[0-9]{5}$\"\n        },\n        \"latitude\": {\n          \"type\": \"number\",\n          \"description\": \"Latitude coordinate of the property.\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude coordinate of the property.\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        },\n        \"mls_id\": {\n          \"type\": \"string\",\n          \"description\": \"MLS listing identifier.\"\n        },\n        \"mls_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the MLS that holds the listing.\"\n        },\n        \"listing_status\": {\n          \"type\": \"string\",\n          \"description\": \"Current listing status.\",\n          \"enum\": [\"active\"\
  , \"pending\", \"sold\", \"off_market\"]\n        },\n        \"list_price\": {\n          \"type\": \"number\",\n          \"description\": \"Listing price in dollars.\",\n          \"minimum\": 0\n        },\n        \"beds\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of bedrooms.\",\n          \"minimum\": 0\n        },\n        \"baths\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of bathrooms.\",\n          \"minimum\": 0\n        },\n        \"sqft\": {\n          \"type\": \"integer\",\n          \"description\": \"Interior square footage.\",\n          \"minimum\": 0\n        },\n        \"property_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of property.\",\n          \"enum\": [\"single_family\", \"multi_family\", \"condo\", \"townhome\", \"mobile\", \"land\", \"farm\"]\n        },\n        \"active_days_on_market\": {\n          \"type\": \"integer\",\n          \"description\": \"\
  Number of days the property has been actively listed.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"FinanceInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Financial qualification information provided by the buyer.\",\n      \"properties\": {\n        \"pre_approved\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the buyer is pre-approved for a mortgage.\"\n        },\n        \"budget_min\": {\n          \"type\": \"number\",\n          \"description\": \"Minimum budget in dollars.\",\n          \"minimum\": 0\n        },\n        \"budget_max\": {\n          \"type\": \"number\",\n          \"description\": \"Maximum budget in dollars.\",\n          \"minimum\": 0\n        },\n        \"financing_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of financing intended such as conventional, FHA, VA, or cash.\",\n          \"enum\": [\"conventional\", \"fha\", \"va\", \"cash\", \"other\"]\n      \
  \  }\n      }\n    },\n    \"ListingAgent\": {\n      \"type\": \"object\",\n      \"description\": \"Listing agent contact information associated with the property.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the listing agent.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address of the listing agent.\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number of the listing agent.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/json-schema/realtor-lead-schema.json
tags: []
title: Realtor.com Lead
---
