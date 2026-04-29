---
description: A mail folder in a user's mailbox, such as Inbox and Drafts. Mail folders can contain messages, other Outlook items, and child mail folders.
layout: schema
name: MailFolder
properties_list:
- description: The unique identifier of the mail folder. Read-only.
  name: id
  type: string
- description: The mail folder's display name.
  name: displayName
  type: string
- description: The unique identifier for the parent mail folder.
  name: parentFolderId
  type: string
- description: The number of immediate child mail folders in the current folder.
  name: childFolderCount
  type: integer
- description: The number of items marked as unread in the folder.
  name: unreadItemCount
  type: integer
- description: The number of items in the folder.
  name: totalItemCount
  type: integer
- description: Indicates whether the mail folder is hidden. Can only be set when creating the folder.
  name: isHidden
  type: boolean
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-graph-mail-mail-folder-schema.json
slug: microsoft-graph-mail-mail-folder
source_filename: microsoft-graph-mail-mail-folder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MailFolder\",\n  \"type\": \"object\",\n  \"description\": \"A mail folder in a user's mailbox, such as Inbox and Drafts. Mail folders can contain messages, other Outlook items, and child mail folders.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the mail folder. Read-only.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The mail folder's display name.\"\n    },\n    \"parentFolderId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the parent mail folder.\"\n    },\n    \"childFolderCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of immediate child mail folders in the current folder.\"\n    },\n    \"unreadItemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items marked as unread\
  \ in the folder.\"\n    },\n    \"totalItemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the folder.\"\n    },\n    \"isHidden\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the mail folder is hidden. Can only be set when creating the folder.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-graph-mail-mail-folder-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: MailFolder
---
