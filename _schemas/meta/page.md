---
description: Represents a Facebook Page as returned by the Graph API Page node. Includes identity, category, contact information, location, and engagement metrics.
layout: schema
name: Meta Graph API Page
properties_list:
- description: The unique numeric identifier for the Page.
  name: id
  type: string
- description: The name of the Page.
  name: name
  type: string
- description: Short description of the Page (deprecated in newer API versions, see 'bio').
  name: about
  type: string
- description: Biography or long description of the Page.
  name: bio
  type: string
- description: The primary category of the Page.
  name: category
  type: string
- description: All categories assigned to the Page.
  name: category_list
  type: array
- description: The Page's cover photo.
  name: cover
  type: object
- description: The description of the Page.
  name: description
  type: string
- description: The description of the Page in HTML format.
  name: description_html
  type: string
- description: The sub-text displayed under the Page name (e.g. category or location).
  name: display_subtext
  type: string
- description: Email addresses listed on the Page.
  name: emails
  type: array
- description: The number of users who like/follow the Page.
  name: fan_count
  type: integer
- description: The number of followers of the Page.
  name: followers_count
  type: integer
- description: When the entity represented by the Page was founded.
  name: founded
  type: string
- description: The name of the global brand Page, if this Page is part of a global brand structure.
  name: global_brand_page_name
  type: string
- description: Operating hours for the business. Keys are day identifiers (e.g. mon_1_open, mon_1_close).
  name: hours
  type: object
- description: Whether the Page is published and publicly visible.
  name: is_published
  type: boolean
- description: Whether the Page has been verified by Facebook.
  name: is_verified
  type: boolean
- description: The Page's Facebook URL.
  name: link
  type: string
- description: The physical location of the business.
  name: location
  type: object
- description: The phone number of the business.
  name: phone
  type: string
- description: The Page's profile picture.
  name: picture
  type: object
- description: The Page's address formatted as a single line.
  name: single_line_address
  type: string
- description: The alias/vanity URL name for the Page.
  name: username
  type: string
- description: The verification status of the Page (e.g. blue_verified, gray_verified, not_verified).
  name: verification_status
  type: string
- description: The URL of the website associated with the Page.
  name: website
  type: string
- description: The number of check-ins at this place.
  name: were_here_count
  type: integer
- description: The WhatsApp number associated with the Page.
  name: whatsapp_number
  type: string
- description: The number of ratings for the Page.
  name: rating_count
  type: integer
- description: Overall star rating of the Page based on user ratings (out of 5).
  name: overall_star_rating
  type: number
- description: The number of people talking about the Page.
  name: talking_about_count
  type: integer
- description: The Page access token (only returned when a Page admin queries with manage_pages permission).
  name: access_token
  type: string
provider_name: Meta
provider_slug: meta
schema_file: json-schema/page.json
slug: page
source_filename: page.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://meta.com/schemas/graph-api/page.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Meta Graph API Page\",\n  \"description\": \"Represents a Facebook Page as returned by the Graph API Page node. Includes identity, category, contact information, location, and engagement metrics.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique numeric identifier for the Page.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Page.\"\n    },\n    \"about\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the Page (deprecated in newer API versions, see 'bio').\"\n    },\n    \"bio\": {\n      \"type\": \"string\",\n      \"description\": \"Biography or long description of the Page.\"\n    },\n    \"category\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The primary category of the Page.\"\n    },\n    \"category_list\": {\n      \"type\": \"array\",\n      \"description\": \"All categories assigned to the Page.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"cover\": {\n      \"type\": \"object\",\n      \"description\": \"The Page's cover photo.\",\n      \"properties\": {\n        \"cover_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the cover photo.\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the cover photo image.\"\n        },\n        \"offset_x\": {\n          \"type\": \"number\",\n          \"description\": \"Horizontal offset percentage for cropping.\"\n    \
  \    },\n        \"offset_y\": {\n          \"type\": \"number\",\n          \"description\": \"Vertical offset percentage for cropping.\"\n        }\n      }\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the Page.\"\n    },\n    \"description_html\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the Page in HTML format.\"\n    },\n    \"display_subtext\": {\n      \"type\": \"string\",\n      \"description\": \"The sub-text displayed under the Page name (e.g. category or location).\"\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses listed on the Page.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"email\"\n      }\n    },\n    \"fan_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of users who like/follow the Page.\"\n    },\n    \"followers_count\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"The number of followers of the Page.\"\n    },\n    \"founded\": {\n      \"type\": \"string\",\n      \"description\": \"When the entity represented by the Page was founded.\"\n    },\n    \"global_brand_page_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the global brand Page, if this Page is part of a global brand structure.\"\n    },\n    \"hours\": {\n      \"type\": \"object\",\n      \"description\": \"Operating hours for the business. Keys are day identifiers (e.g. mon_1_open, mon_1_close).\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"is_published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Page is published and publicly visible.\"\n    },\n    \"is_verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Page has been verified by Facebook.\"\n    },\n    \"link\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"\
  description\": \"The Page's Facebook URL.\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"The physical location of the business.\",\n      \"properties\": {\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\"\n        },\n        \"latitude\": {\n          \"type\": \"number\"\n        },\n        \"longitude\": {\n          \"type\": \"number\"\n        },\n        \"state\": {\n          \"type\": \"string\"\n        },\n        \"street\": {\n          \"type\": \"string\"\n        },\n        \"zip\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"The phone number of the business.\"\n    },\n    \"picture\": {\n      \"type\": \"object\",\n      \"description\": \"The Page's profile picture.\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"object\",\n          \"properties\"\
  : {\n            \"height\": {\n              \"type\": \"integer\"\n            },\n            \"is_silhouette\": {\n              \"type\": \"boolean\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"width\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    },\n    \"single_line_address\": {\n      \"type\": \"string\",\n      \"description\": \"The Page's address formatted as a single line.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The alias/vanity URL name for the Page.\"\n    },\n    \"verification_status\": {\n      \"type\": \"string\",\n      \"description\": \"The verification status of the Page (e.g. blue_verified, gray_verified, not_verified).\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the website associated with the\
  \ Page.\"\n    },\n    \"were_here_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of check-ins at this place.\"\n    },\n    \"whatsapp_number\": {\n      \"type\": \"string\",\n      \"description\": \"The WhatsApp number associated with the Page.\"\n    },\n    \"rating_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of ratings for the Page.\"\n    },\n    \"overall_star_rating\": {\n      \"type\": \"number\",\n      \"description\": \"Overall star rating of the Page based on user ratings (out of 5).\"\n    },\n    \"talking_about_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of people talking about the Page.\"\n    },\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"The Page access token (only returned when a Page admin queries with manage_pages permission).\"\n    }\n  },\n  \"additionalProperties\": true,\n  \"examples\": [\n    {\n      \"id\": \"123456789012345\"\
  ,\n      \"name\": \"Example Business Page\",\n      \"category\": \"Software Company\",\n      \"category_list\": [\n        {\n          \"id\": \"2256\",\n          \"name\": \"Software Company\"\n        }\n      ],\n      \"fan_count\": 50000,\n      \"followers_count\": 52000,\n      \"is_published\": true,\n      \"is_verified\": true,\n      \"link\": \"https://www.facebook.com/examplebusiness\",\n      \"username\": \"examplebusiness\",\n      \"website\": \"https://www.example.com\",\n      \"location\": {\n        \"city\": \"Menlo Park\",\n        \"country\": \"United States\",\n        \"latitude\": 37.4529,\n        \"longitude\": -122.1817,\n        \"state\": \"CA\",\n        \"street\": \"1 Hacker Way\",\n        \"zip\": \"94025\"\n      },\n      \"phone\": \"+1 650-543-4800\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/meta/refs/heads/main/json-schema/page.json
tags:
- Advertising
- Analytics
- Artificial Intelligence
- Messaging
- Social
- Social Media
- Virtual Reality
title: Meta Graph API Page
---
