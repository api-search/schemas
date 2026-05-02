---
description: Represents an email message in a user's mailbox as exposed through the Microsoft Graph Mail API. A message is contained within a mail folder and supports operations such as send, reply, forward, and delete.
layout: schema
name: Microsoft Exchange Message
properties_list:
- description: Unique identifier for the message. By default, this value changes when the item is moved from one container to another.
  name: id
  type: string
- description: The subject of the message
  name: subject
  type: string
- description: The body of the message in HTML or text format
  name: body
  type: object
- description: The first 255 characters of the message body in text format
  name: bodyPreview
  type: string
- description: The owner of the mailbox from which the message is sent
  name: from
  type: object
- description: The account used to generate the message
  name: sender
  type: object
- description: 'The To: recipients for the message'
  name: toRecipients
  type: array
- description: 'The Cc: recipients for the message'
  name: ccRecipients
  type: array
- description: 'The Bcc: recipients for the message'
  name: bccRecipients
  type: array
- description: The email addresses to use when replying
  name: replyTo
  type: array
- description: The ID of the conversation the email belongs to
  name: conversationId
  type: string
- description: Indicates the position of the message within the conversation
  name: conversationIndex
  type: string
- description: The date and time the message was created in ISO 8601 UTC format
  name: createdDateTime
  type: string
- description: The date and time the message was last changed
  name: lastModifiedDateTime
  type: string
- description: The date and time the message was received
  name: receivedDateTime
  type: string
- description: The date and time the message was sent
  name: sentDateTime
  type: string
- description: Indicates whether the message has attachments (excludes inline attachments)
  name: hasAttachments
  type: boolean
- description: The importance of the message
  name: importance
  type: string
- description: The classification of the message based on inferred relevance or importance
  name: inferenceClassification
  type: string
- description: The message ID in the format specified by RFC2822
  name: internetMessageId
  type: string
- description: A collection of message headers defined by RFC5322
  name: internetMessageHeaders
  type: array
- description: Indicates whether a delivery receipt is requested
  name: isDeliveryReceiptRequested
  type: boolean
- description: Indicates whether the message is a draft
  name: isDraft
  type: boolean
- description: Indicates whether the message has been read
  name: isRead
  type: boolean
- description: Indicates whether a read receipt is requested
  name: isReadReceiptRequested
  type: boolean
- description: The unique identifier for the message's parent mailFolder
  name: parentFolderId
  type: string
- description: The URL to open the message in Outlook on the web
  name: webLink
  type: string
- description: The follow-up flag status for the message
  name: flag
  type: object
- description: The categories associated with the message
  name: categories
  type: array
- description: The version of the message
  name: changeKey
  type: string
- description: The part of the body unique to the current message
  name: uniqueBody
  type: object
provider_name: Microsoft Exchange
provider_slug: microsoft-exchange
schema_file: json-schema/microsoft-exchange-message-schema.json
slug: microsoft-exchange-message
source_filename: microsoft-exchange-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/microsoft-exchange/json-schema/microsoft-exchange-message-schema.json\",\n  \"title\": \"Microsoft Exchange Message\",\n  \"description\": \"Represents an email message in a user's mailbox as exposed through the Microsoft Graph Mail API. A message is contained within a mail folder and supports operations such as send, reply, forward, and delete.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the message. By default, this value changes when the item is moved from one container to another.\",\n      \"readOnly\": true\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject of the message\"\n    },\n    \"body\": {\n      \"$ref\": \"#/$defs/itemBody\",\n      \"description\": \"The body of the message in HTML or text format\"\n   \
  \ },\n    \"bodyPreview\": {\n      \"type\": \"string\",\n      \"description\": \"The first 255 characters of the message body in text format\",\n      \"maxLength\": 255,\n      \"readOnly\": true\n    },\n    \"from\": {\n      \"$ref\": \"#/$defs/recipient\",\n      \"description\": \"The owner of the mailbox from which the message is sent\"\n    },\n    \"sender\": {\n      \"$ref\": \"#/$defs/recipient\",\n      \"description\": \"The account used to generate the message\"\n    },\n    \"toRecipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/recipient\"\n      },\n      \"description\": \"The To: recipients for the message\"\n    },\n    \"ccRecipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/recipient\"\n      },\n      \"description\": \"The Cc: recipients for the message\"\n    },\n    \"bccRecipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/recipient\"\n\
  \      },\n      \"description\": \"The Bcc: recipients for the message\"\n    },\n    \"replyTo\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/recipient\"\n      },\n      \"description\": \"The email addresses to use when replying\"\n    },\n    \"conversationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the conversation the email belongs to\"\n    },\n    \"conversationIndex\": {\n      \"type\": \"string\",\n      \"contentEncoding\": \"base64\",\n      \"description\": \"Indicates the position of the message within the conversation\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was created in ISO 8601 UTC format\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was last changed\"\
  ,\n      \"readOnly\": true\n    },\n    \"receivedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was received\",\n      \"readOnly\": true\n    },\n    \"sentDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was sent\",\n      \"readOnly\": true\n    },\n    \"hasAttachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message has attachments (excludes inline attachments)\",\n      \"readOnly\": true\n    },\n    \"importance\": {\n      \"type\": \"string\",\n      \"enum\": [\"low\", \"normal\", \"high\"],\n      \"description\": \"The importance of the message\"\n    },\n    \"inferenceClassification\": {\n      \"type\": \"string\",\n      \"enum\": [\"focused\", \"other\"],\n      \"description\": \"The classification of the message based on inferred relevance or importance\"\n\
  \    },\n    \"internetMessageId\": {\n      \"type\": \"string\",\n      \"description\": \"The message ID in the format specified by RFC2822\"\n    },\n    \"internetMessageHeaders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/internetMessageHeader\"\n      },\n      \"description\": \"A collection of message headers defined by RFC5322\",\n      \"readOnly\": true\n    },\n    \"isDeliveryReceiptRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether a delivery receipt is requested\"\n    },\n    \"isDraft\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message is a draft\",\n      \"readOnly\": true\n    },\n    \"isRead\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message has been read\"\n    },\n    \"isReadReceiptRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether a read receipt is requested\"\n    },\n\
  \    \"parentFolderId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the message's parent mailFolder\",\n      \"readOnly\": true\n    },\n    \"webLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to open the message in Outlook on the web\",\n      \"readOnly\": true\n    },\n    \"flag\": {\n      \"$ref\": \"#/$defs/followupFlag\",\n      \"description\": \"The follow-up flag status for the message\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The categories associated with the message\"\n    },\n    \"changeKey\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the message\",\n      \"readOnly\": true\n    },\n    \"uniqueBody\": {\n      \"$ref\": \"#/$defs/itemBody\",\n      \"description\": \"The part of the body unique to the current message\"\n    }\n  },\n  \"required\"\
  : [\"subject\"],\n  \"$defs\": {\n    \"recipient\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an email recipient\",\n      \"properties\": {\n        \"emailAddress\": {\n          \"$ref\": \"#/$defs/emailAddress\"\n        }\n      }\n    },\n    \"emailAddress\": {\n      \"type\": \"object\",\n      \"description\": \"The name and email address of a person or entity\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the person or entity\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address\"\n        }\n      }\n    },\n    \"itemBody\": {\n      \"type\": \"object\",\n      \"description\": \"Represents the body content\",\n      \"properties\": {\n        \"contentType\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"html\"],\n          \"description\":\
  \ \"The type of the content\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The content of the body\"\n        }\n      }\n    },\n    \"internetMessageHeader\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value pair representing an Internet message header defined by RFC5322\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the message header\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the message header\"\n        }\n      }\n    },\n    \"followupFlag\": {\n      \"type\": \"object\",\n      \"description\": \"Follow-up flag on a message\",\n      \"properties\": {\n        \"completedDateTime\": {\n          \"$ref\": \"#/$defs/dateTimeTimeZone\"\n        },\n        \"dueDateTime\": {\n          \"$ref\": \"#/$defs/dateTimeTimeZone\"\n        },\n        \"startDateTime\"\
  : {\n          \"$ref\": \"#/$defs/dateTimeTimeZone\"\n        },\n        \"flagStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"notFlagged\", \"complete\", \"flagged\"],\n          \"description\": \"The status of the follow-up flag\"\n        }\n      }\n    },\n    \"dateTimeTimeZone\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a date, time, and time zone\",\n      \"properties\": {\n        \"dateTime\": {\n          \"type\": \"string\",\n          \"description\": \"A date and time combined in ISO 8601 format\"\n        },\n        \"timeZone\": {\n          \"type\": \"string\",\n          \"description\": \"A time zone name (e.g. Pacific Standard Time)\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-exchange/refs/heads/main/json-schema/microsoft-exchange-message-schema.json
tags:
- Calendar
- Collaboration
- Contacts
- Email
- Enterprise
title: Microsoft Exchange Message
---
