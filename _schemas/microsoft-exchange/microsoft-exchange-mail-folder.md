---
description: Represents a mail folder in a user's mailbox as exposed through the Microsoft Graph Mail API. Mail folders such as Inbox, Drafts, and Sent Items can contain messages, other Outlook items, and child mail folders. Well-known folder names like inbox, drafts, sentitems, and deleteditems can be used in place of folder IDs.
layout: schema
name: Microsoft Exchange Mail Folder
properties_list:
- description: The mail folder's unique identifier
  name: id
  type: string
- description: The mail folder's display name
  name: displayName
  type: string
- description: The unique identifier for the parent mail folder
  name: parentFolderId
  type: string
- description: The number of immediate child mail folders
  name: childFolderCount
  type: integer
- description: The number of items in the mail folder (includes all item types)
  name: totalItemCount
  type: integer
- description: The number of items in the mail folder marked as unread
  name: unreadItemCount
  type: integer
- description: Indicates whether the mail folder is hidden. Can only be set when creating the folder.
  name: isHidden
  type: boolean
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
schema_file: json-schema/microsoft-exchange-mail-folder-schema.json
slug: microsoft-exchange-mail-folder
source_filename: microsoft-exchange-mail-folder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/microsoft-exchange/json-schema/microsoft-exchange-mail-folder-schema.json\",\n  \"title\": \"Microsoft Exchange Mail Folder\",\n  \"description\": \"Represents a mail folder in a user's mailbox as exposed through the Microsoft Graph Mail API. Mail folders such as Inbox, Drafts, and Sent Items can contain messages, other Outlook items, and child mail folders. Well-known folder names like inbox, drafts, sentitems, and deleteditems can be used in place of folder IDs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The mail folder's unique identifier\",\n      \"readOnly\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The mail folder's display name\"\n    },\n    \"parentFolderId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique\
  \ identifier for the parent mail folder\",\n      \"readOnly\": true\n    },\n    \"childFolderCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of immediate child mail folders\",\n      \"readOnly\": true\n    },\n    \"totalItemCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of items in the mail folder (includes all item types)\",\n      \"readOnly\": true\n    },\n    \"unreadItemCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of items in the mail folder marked as unread\",\n      \"readOnly\": true\n    },\n    \"isHidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the mail folder is hidden. Can only be set when creating the folder.\",\n      \"default\": false\n    }\n  },\n  \"required\": [\"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/json-schema/microsoft-exchange-mail-folder-schema.json
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
title: Microsoft Exchange Mail Folder
---
