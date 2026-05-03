---
description: Represents a user within an Experience Cloud site, including profile details, reputation, and community membership information.
layout: schema
name: Community User
properties_list:
- description: Unique 18-character Salesforce user ID
  name: id
  type: string
- description: Salesforce username (typically email format)
  name: username
  type: string
- description: Full display name of the user
  name: name
  type: string
- description: First name of the user
  name: firstName
  type: string
- description: Last name of the user
  name: lastName
  type: string
- description: Display name shown in the community (may be nickname)
  name: displayName
  type: string
- description: Community-specific nickname for the user
  name: communityNickname
  type: string
- description: Email address of the user
  name: email
  type: string
- description: Professional title of the user
  name: title
  type: string
- description: Company or organization name
  name: companyName
  type: string
- description: Type of user (e.g., Internal, Guest, External)
  name: type
  type: string
- description: User's profile photo URLs in various sizes
  name: photo
  type: object
- description: User's reputation information in the community
  name: reputation
  type: object
- description: API resource URL for this user
  name: url
  type: string
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
schema_file: json-schema/salesforce-experience-cloud-community-user-schema.json
slug: salesforce-experience-cloud-community-user
source_filename: salesforce-experience-cloud-community-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/experience-cloud/community-user.json\",\n  \"title\": \"Community User\",\n  \"description\": \"Represents a user within an Experience Cloud site, including profile details, reputation, and community membership information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce user ID\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce username (typically email format)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the user\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the user\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the user\"\n    },\n    \"displayName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Display name shown in the community (may be nickname)\"\n    },\n    \"communityNickname\": {\n      \"type\": \"string\",\n      \"description\": \"Community-specific nickname for the user\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Professional title of the user\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Company or organization name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of user (e.g., Internal, Guest, External)\",\n      \"enum\": [\"Internal\", \"Guest\", \"External\", \"ChatterFree\", \"ChatterExternal\"]\n    },\n    \"photo\": {\n      \"type\": \"object\",\n      \"description\": \"User's profile photo URLs in various sizes\",\n      \"properties\": {\n\
  \        \"fullEmailPhotoUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Full-size photo URL for email\"\n        },\n        \"largePhotoUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Large profile photo URL\"\n        },\n        \"smallPhotoUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Small profile photo URL (thumbnail)\"\n        },\n        \"standardEmailPhotoUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Standard-size photo URL for email\"\n        }\n      }\n    },\n    \"reputation\": {\n      \"type\": \"object\",\n      \"description\": \"User's reputation information in the community\",\n      \"properties\": {\n        \"reputationPoints\": {\n          \"type\": \"number\",\n          \"description\": \"Total reputation points earned\"\n        },\n\
  \        \"reputationLevel\": {\n          \"type\": \"object\",\n          \"description\": \"Current reputation level\",\n          \"properties\": {\n            \"levelLabel\": {\n              \"type\": \"string\",\n              \"description\": \"Display label for the reputation level\"\n            },\n            \"levelNumber\": {\n              \"type\": \"integer\",\n              \"description\": \"Numeric level value\"\n            }\n          }\n        }\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API resource URL for this user\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/json-schema/salesforce-experience-cloud-community-user-schema.json
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
title: Community User
---
