---
description: Represents a B2B Data Interchange profile — the system-side resource that represents your EDI sender or receiver entity.
layout: schema
name: Profile
properties_list:
- description: Unique identifier for the profile
  name: profileId
  type: string
- description: Amazon Resource Name (ARN) for the profile
  name: profileArn
  type: string
- description: Name of the profile
  name: name
  type: string
- description: Legal business name of the organization
  name: businessName
  type: string
- description: Phone number for the profile contact
  name: phone
  type: string
- description: Email address for the profile contact
  name: email
  type: string
- description: Whether CloudWatch logging is enabled for this profile
  name: logging
  type: string
- description: CloudWatch log group name for this profile
  name: logGroupName
  type: string
- description: Timestamp when the profile was created
  name: createdAt
  type: string
- description: Timestamp when the profile was last modified
  name: modifiedAt
  type: string
provider_name: Amazon B2B Data Interchange
provider_slug: amazon-b2b-data-interchange
schema_file: json-schema/profile.json
slug: profile
source_filename: profile.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/main/json-schema/profile.json\",\n  \"title\": \"Profile\",\n  \"description\": \"Represents a B2B Data Interchange profile — the system-side resource that represents your EDI sender or receiver entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the profile\",\n      \"pattern\": \"^p-[a-zA-Z0-9]+$\"\n    },\n    \"profileArn\": {\n      \"type\": \"string\",\n      \"description\": \"Amazon Resource Name (ARN) for the profile\",\n      \"pattern\": \"^arn:aws:b2bi:[a-z0-9-]+:[0-9]+:profile/p-[a-zA-Z0-9]+$\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the profile\",\n      \"minLength\": 1,\n      \"maxLength\": 254\n    },\n    \"businessName\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Legal business name of the organization\",\n      \"minLength\": 1,\n      \"maxLength\": 254\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number for the profile contact\",\n      \"pattern\": \"^\\\\+[1-9]\\\\d{1,14}$\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address for the profile contact\"\n    },\n    \"logging\": {\n      \"type\": \"string\",\n      \"enum\": [\"ENABLED\", \"DISABLED\"],\n      \"description\": \"Whether CloudWatch logging is enabled for this profile\"\n    },\n    \"logGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"CloudWatch log group name for this profile\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the profile was created\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\":\
  \ \"date-time\",\n      \"description\": \"Timestamp when the profile was last modified\"\n    }\n  },\n  \"required\": [\"profileId\", \"profileArn\", \"name\", \"businessName\", \"phone\", \"logging\", \"createdAt\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/json-schema/profile.json
tags:
- EDI
- B2B
- Data Interchange
- Supply Chain
- Healthcare
- Financial Services
- Amazon Web Services
- AWS
title: Profile
---
