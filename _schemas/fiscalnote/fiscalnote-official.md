---
description: A government official including legislators, executives, and appointees tracked by FiscalNote across U.S. and international jurisdictions.
layout: schema
name: FiscalNote Government Official
properties_list:
- description: Unique identifier for the official.
  name: id
  type: string
- description: First name of the official.
  name: firstName
  type: string
- description: Last name of the official.
  name: lastName
  type: string
- description: Full name of the official.
  name: fullName
  type: string
- description: Official title or position.
  name: title
  type: string
- description: Political party affiliation.
  name: party
  type: string
- description: Jurisdiction the official serves in.
  name: jurisdiction
  type: string
- description: U.S. state abbreviation if applicable.
  name: state
  type: string
- description: Legislative chamber if applicable.
  name: chamber
  type: string
- description: District the official represents.
  name: district
  type: string
- description: Whether the official is currently serving.
  name: active
  type: boolean
- description: Biographical summary.
  name: biography
  type: string
- description: URL to the official's photo.
  name: photoUrl
  type: string
- description: ''
  name: contactInfo
  type: object
- description: ''
  name: socialMedia
  type: object
- description: Committees the official serves on.
  name: committees
  type: array
- description: Number of bills sponsored.
  name: sponsoredBillCount
  type: integer
- description: Number of bills co-sponsored.
  name: cosponsoredBillCount
  type: integer
- description: Start date of the current term.
  name: termStart
  type: string
- description: End date of the current term.
  name: termEnd
  type: string
- description: URL to the official's profile on FiscalNote.
  name: url
  type: string
- description: Timestamp when the record was created.
  name: createdAt
  type: string
- description: Timestamp when the record was last updated.
  name: updatedAt
  type: string
provider_name: FiscalNote
provider_slug: fiscalnote
schema_file: json-schema/fiscalnote-official-schema.json
slug: fiscalnote-official
source_filename: fiscalnote-official-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fiscalnote.com/schemas/fiscalnote/official.json\",\n  \"title\": \"FiscalNote Government Official\",\n  \"description\": \"A government official including legislators, executives, and appointees tracked by FiscalNote across U.S. and international jurisdictions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"fullName\", \"jurisdiction\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the official.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the official.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the official.\"\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the official.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"Official title or position.\"\n    },\n    \"party\": {\n      \"type\": \"string\",\n      \"description\": \"Political party affiliation.\"\n    },\n    \"jurisdiction\": {\n      \"type\": \"string\",\n      \"description\": \"Jurisdiction the official serves in.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"U.S. state abbreviation if applicable.\",\n      \"minLength\": 2,\n      \"maxLength\": 2\n    },\n    \"chamber\": {\n      \"type\": \"string\",\n      \"description\": \"Legislative chamber if applicable.\",\n      \"enum\": [\"senate\", \"house\"]\n    },\n    \"district\": {\n      \"type\": \"string\",\n      \"description\": \"District the official represents.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the official is currently serving.\"\n    },\n    \"biography\": {\n      \"type\": \"string\",\n      \"description\": \"Biographical summary.\"\n    },\n    \"photoUrl\": {\n     \
  \ \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the official's photo.\"\n    },\n    \"contactInfo\": {\n      \"$ref\": \"#/$defs/ContactInfo\"\n    },\n    \"socialMedia\": {\n      \"$ref\": \"#/$defs/SocialMedia\"\n    },\n    \"committees\": {\n      \"type\": \"array\",\n      \"description\": \"Committees the official serves on.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CommitteeMembership\"\n      }\n    },\n    \"sponsoredBillCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of bills sponsored.\",\n      \"minimum\": 0\n    },\n    \"cosponsoredBillCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of bills co-sponsored.\",\n      \"minimum\": 0\n    },\n    \"termStart\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date of the current term.\"\n    },\n    \"termEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"\
  description\": \"End date of the current term.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the official's profile on FiscalNote.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"ContactInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Contact information for a government official.\",\n      \"properties\": {\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"Email address.\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number.\"\n        },\n        \"address\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"Mailing address.\"\n        },\n        \"website\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Official website.\"\n        }\n      }\n    },\n    \"SocialMedia\": {\n      \"type\": \"object\",\n      \"description\": \"Social media profiles.\",\n      \"properties\": {\n        \"twitter\": {\n          \"type\": \"string\",\n          \"description\": \"Twitter/X handle.\"\n        },\n        \"facebook\": {\n          \"type\": \"string\",\n          \"description\": \"Facebook profile URL or handle.\"\n        },\n        \"youtube\": {\n          \"type\": \"string\",\n          \"description\": \"YouTube channel URL.\"\n        }\n      }\n    },\n    \"CommitteeMembership\": {\n      \"type\": \"object\",\n      \"description\": \"A committee membership record.\",\n      \"required\": [\"committeeId\", \"committeeName\"],\n      \"properties\": {\n        \"committeeId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the committee.\"\n        },\n        \"committeeName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the committee.\"\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"Role on the committee.\",\n          \"enum\": [\"chair\", \"vice_chair\", \"ranking_member\", \"member\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/json-schema/fiscalnote-official-schema.json
tags:
- Government
- Legislation
- Policy
- Political Intelligence
- Regulation
title: FiscalNote Government Official
---
