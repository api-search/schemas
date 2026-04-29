---
description: SharePoint user profile.
layout: schema
name: UserProfile
properties_list:
- description: ''
  name: AccountName
  type: string
- description: ''
  name: DisplayName
  type: string
- description: ''
  name: Email
  type: string
- description: ''
  name: Title
  type: string
- description: ''
  name: Department
  type: string
- description: ''
  name: PictureUrl
  type: string
- description: ''
  name: PersonalUrl
  type: string
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-user-profile-schema.json
slug: sharepoint-user-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-user-profile-schema.json\",\n  \"title\": \"UserProfile\",\n  \"description\": \"SharePoint user profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountName\": {\n      \"type\": \"string\",\n      \"example\": \"i:0#.f|membership|user@contoso.com\"\n    },\n    \"DisplayName\": {\n      \"type\": \"string\",\n      \"example\": \"Jane Smith\"\n    },\n    \"Email\": {\n      \"type\": \"string\",\n      \"example\": \"jane.smith@contoso.com\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"example\": \"Senior Developer\"\n    },\n    \"Department\": {\n      \"type\": \"string\",\n      \"example\": \"Engineering\"\n    },\n    \"PictureUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://contoso.sharepoint.com/_layouts/15/userphoto.aspx?size=L&accountname=user@contoso.com\"\
  \n    },\n    \"PersonalUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://contoso-my.sharepoint.com/personal/user_contoso_com/\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-user-profile-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: UserProfile
---
