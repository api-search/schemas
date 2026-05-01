---
description: A member represents a person who has signed up for a Ghost publication. Members can be free subscribers who receive newsletters, or paid subscribers with access to premium content through membership tiers. Members have associated labels for segmentation, newsletter subscriptions, and Stripe-based paid subscriptions.
layout: schema
name: Ghost Member
properties_list:
- description: Unique identifier for the member
  name: id
  type: string
- description: Universally unique identifier for the member
  name: uuid
  type: string
- description: Email address of the member, used as the primary identifier for signups
  name: email
  type: string
- description: Display name of the member
  name: name
  type:
  - string
  - 'null'
- description: Internal note about the member, visible only to staff
  name: note
  type:
  - string
  - 'null'
- description: Geolocation data captured at signup time, stored as a JSON string
  name: geolocation
  type:
  - string
  - 'null'
- description: Membership status based on subscription state
  name: status
  type: string
- description: Labels applied to the member for segmentation and filtering
  name: labels
  type: array
- description: Paid subscriptions associated with the member, managed through Stripe
  name: subscriptions
  type: array
- description: Newsletters the member is subscribed to receive
  name: newsletters
  type: array
- description: Gravatar URL generated from the member email address
  name: avatar_image
  type: string
- description: Total number of emails sent to this member
  name: email_count
  type: integer
- description: Total number of emails opened by this member
  name: email_opened_count
  type: integer
- description: Email open rate as a percentage
  name: email_open_rate
  type:
  - number
  - 'null'
- description: ISO 8601 timestamp when the member signed up
  name: created_at
  type: string
- description: ISO 8601 timestamp when the member record was last updated
  name: updated_at
  type: string
provider_name: Ghost
provider_slug: ghost
schema_file: json-schema/ghost-member-schema.json
slug: ghost-member
source_filename: ghost-member-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://ghost.org/schemas/ghost/member.json\",\n  \"title\": \"Ghost Member\",\n  \"description\": \"A member represents a person who has signed up for a Ghost publication. Members can be free subscribers who receive newsletters, or paid subscribers with access to premium content through membership tiers. Members have associated labels for segmentation, newsletter subscriptions, and Stripe-based paid subscriptions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"email\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the member\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Universally unique identifier for the member\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"\
  Email address of the member, used as the primary identifier for signups\"\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Display name of the member\",\n      \"maxLength\": 191\n    },\n    \"note\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Internal note about the member, visible only to staff\",\n      \"maxLength\": 2000\n    },\n    \"geolocation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Geolocation data captured at signup time, stored as a JSON string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Membership status based on subscription state\",\n      \"enum\": [\"free\", \"paid\", \"comped\"]\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the member for segmentation and filtering\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Label\"\n      }\n    },\n    \"subscriptions\": {\n      \"\
  type\": \"array\",\n      \"description\": \"Paid subscriptions associated with the member, managed through Stripe\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Subscription\"\n      }\n    },\n    \"newsletters\": {\n      \"type\": \"array\",\n      \"description\": \"Newsletters the member is subscribed to receive\",\n      \"items\": {\n        \"$ref\": \"#/$defs/NewsletterSubscription\"\n      }\n    },\n    \"avatar_image\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Gravatar URL generated from the member email address\"\n    },\n    \"email_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of emails sent to this member\",\n      \"minimum\": 0\n    },\n    \"email_opened_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of emails opened by this member\",\n      \"minimum\": 0\n    },\n    \"email_open_rate\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\"\
  : \"Email open rate as a percentage\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the member signed up\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the member record was last updated\"\n    }\n  },\n  \"$defs\": {\n    \"Label\": {\n      \"type\": \"object\",\n      \"description\": \"A label for categorizing and segmenting members\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the label\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the label\",\n          \"minLength\": 1,\n          \"maxLength\": 191\n        },\n        \"\
  slug\": {\n          \"type\": \"string\",\n          \"description\": \"URL-safe slug for the label\",\n          \"maxLength\": 191\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Creation timestamp\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Last update timestamp\"\n        }\n      }\n    },\n    \"Subscription\": {\n      \"type\": \"object\",\n      \"description\": \"A paid subscription managed through Stripe, linking a member to a membership tier\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Stripe subscription identifier\"\n        },\n        \"customer\": {\n          \"type\": \"object\",\n          \"description\": \"Stripe customer associated with the subscription\",\n          \"properties\": {\n            \"id\": {\n  \
  \            \"type\": \"string\",\n              \"description\": \"Stripe customer ID\"\n            },\n            \"name\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"Customer display name\"\n            },\n            \"email\": {\n              \"type\": \"string\",\n              \"format\": \"email\",\n              \"description\": \"Customer email address\"\n            }\n          }\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current subscription status\",\n          \"enum\": [\"active\", \"trialing\", \"canceled\", \"unpaid\", \"past_due\"]\n        },\n        \"start_date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the subscription started\"\n        },\n        \"default_payment_card_last4\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Last four digits of the payment card on\
  \ file\",\n          \"pattern\": \"^\\\\d{4}$\"\n        },\n        \"cancel_at_period_end\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the subscription will cancel at the end of the current billing period\"\n        },\n        \"cancellation_reason\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Reason provided for subscription cancellation\"\n        },\n        \"current_period_end\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"End date of the current billing period\"\n        },\n        \"price\": {\n          \"type\": \"object\",\n          \"description\": \"Pricing details for the subscription\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"Stripe price identifier\"\n            },\n            \"nickname\": {\n              \"type\": [\"string\", \"null\"],\n              \"\
  description\": \"Human-readable price name\"\n            },\n            \"amount\": {\n              \"type\": \"integer\",\n              \"description\": \"Price amount in the smallest currency unit (e.g., cents)\",\n              \"minimum\": 0\n            },\n            \"interval\": {\n              \"type\": \"string\",\n              \"description\": \"Billing interval\",\n              \"enum\": [\"month\", \"year\"]\n            },\n            \"currency\": {\n              \"type\": \"string\",\n              \"description\": \"ISO 4217 currency code\",\n              \"pattern\": \"^[A-Z]{3}$\"\n            }\n          }\n        }\n      }\n    },\n    \"NewsletterSubscription\": {\n      \"type\": \"object\",\n      \"description\": \"A newsletter that the member is subscribed to\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Newsletter identifier\"\n        },\n        \"\
  name\": {\n          \"type\": \"string\",\n          \"description\": \"Newsletter display name\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Subscription status for this newsletter\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/json-schema/ghost-member-schema.json
tags:
- Content Management
- Publishing
- Headless CMS
- Blogging
- Newsletters
- Memberships
title: Ghost Member
---
