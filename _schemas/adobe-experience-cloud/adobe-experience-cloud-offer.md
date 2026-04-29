---
description: A personalized offer used in Adobe Journey Optimizer and Target for delivering tailored content to customers based on eligibility rules, priority, and placement configuration.
layout: schema
name: Adobe Experience Cloud Offer
properties_list:
- description: The unique identifier for the offer.
  name: offerId
  type: string
- description: The human-readable name of the offer.
  name: name
  type: string
- description: A description of the offer content and purpose.
  name: description
  type: string
- description: The lifecycle status of the offer.
  name: status
  type: string
- description: Whether this is a personalized or fallback offer.
  name: offerType
  type: string
- description: The content representations for different channels and placements.
  name: representations
  type: array
- description: The eligibility rule defining which profiles can receive this offer.
  name: eligibilityRule
  type: object
- description: The priority ranking when multiple offers are eligible.
  name: priority
  type: integer
- description: Frequency capping constraints.
  name: cappingConstraint
  type: object
- description: When the offer becomes eligible for delivery.
  name: startDate
  type: string
- description: When the offer is no longer eligible for delivery.
  name: endDate
  type: string
- description: Tags for categorizing offers into collections.
  name: tags
  type: array
- description: When the offer was created.
  name: created
  type: string
- description: When the offer was last modified.
  name: lastModified
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/adobe-experience-cloud-offer.json
slug: adobe-experience-cloud-offer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"adobe-experience-cloud-offer.json\",\n  \"title\": \"Adobe Experience Cloud Offer\",\n  \"description\": \"A personalized offer used in Adobe Journey Optimizer and Target for delivering tailored content to customers based on eligibility rules, priority, and placement configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"offerId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the offer.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the offer.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the offer content and purpose.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"approved\", \"archived\"],\n      \"description\": \"The lifecycle status of the offer.\"\n    },\n    \"offerType\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\"personalized\", \"fallback\"],\n      \"description\": \"Whether this is a personalized or fallback offer.\"\n    },\n    \"representations\": {\n      \"type\": \"array\",\n      \"description\": \"The content representations for different channels and placements.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"channel\": {\n            \"type\": \"string\",\n            \"description\": \"The delivery channel (web, email, mobile, etc.).\"\n          },\n          \"placementId\": {\n            \"type\": \"string\",\n            \"description\": \"The placement where this representation can be displayed.\"\n          },\n          \"content\": {\n            \"type\": \"string\",\n            \"description\": \"The content payload (HTML, JSON, text, or image URL).\"\n          },\n          \"contentType\": {\n            \"type\": \"string\",\n            \"enum\": [\"text/html\", \"application/json\"\
  , \"text/plain\", \"image/*\"],\n            \"description\": \"The MIME type of the content.\"\n          }\n        }\n      }\n    },\n    \"eligibilityRule\": {\n      \"type\": \"object\",\n      \"description\": \"The eligibility rule defining which profiles can receive this offer.\",\n      \"properties\": {\n        \"ruleId\": {\n          \"type\": \"string\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The priority ranking when multiple offers are eligible.\"\n    },\n    \"cappingConstraint\": {\n      \"type\": \"object\",\n      \"description\": \"Frequency capping constraints.\",\n      \"properties\": {\n        \"maxImpressions\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of times the offer can be shown.\"\n        },\n        \"scope\": {\n          \"type\": \"string\",\n          \"enum\": [\"global\"\
  , \"perProfile\"],\n          \"description\": \"Whether capping applies globally or per profile.\"\n        }\n      }\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the offer becomes eligible for delivery.\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the offer is no longer eligible for delivery.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags for categorizing offers into collections.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the offer was created.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the offer was last modified.\"\n    }\n  },\n  \"required\": [\"offerId\", \"name\"\
  , \"offerType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/adobe-experience-cloud-offer.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Adobe Experience Cloud Offer
---
