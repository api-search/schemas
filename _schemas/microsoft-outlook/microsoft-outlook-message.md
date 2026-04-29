---
description: JSON Schema for a Microsoft Graph message resource representing an email message in a user's mailbox. Based on the microsoft.graph.message resource type from the Microsoft Graph v1.0 API.
layout: schema
name: Microsoft Outlook Message
properties_list:
- description: 'Unique identifier for the message. By default, this value changes when the item is moved from one container to another. Use the Prefer: IdType="ImmutableId" header for immutable identifiers.'
  name: id
  type: string
- description: The date and time the message was created. Uses ISO 8601 format in UTC time (e.g., 2014-01-01T00:00:00Z).
  name: createdDateTime
  type: string
- description: The date and time the message was last changed. Uses ISO 8601 format in UTC time.
  name: lastModifiedDateTime
  type: string
- description: The version of the message.
  name: changeKey
  type: string
- description: The categories associated with the message.
  name: categories
  type: array
- description: The date and time the message was received. Uses ISO 8601 format in UTC time.
  name: receivedDateTime
  type: string
- description: The date and time the message was sent. Uses ISO 8601 format in UTC time.
  name: sentDateTime
  type: string
- description: Indicates whether the message has attachments. This property does not include inline attachments. To verify inline attachments, parse the body property for a src attribute.
  name: hasAttachments
  type: boolean
- description: The message ID in the format specified by RFC 2822.
  name: internetMessageId
  type: string
- description: A collection of message headers defined by RFC 5322. Includes custom message headers starting with 'x-'. Returned only on applying a $select query option.
  name: internetMessageHeaders
  type: array
- description: The subject of the message.
  name: subject
  type: string
- description: The body of the message. Can be in HTML or text format.
  name: body
  type: object
- description: The first 255 characters of the message body in text format.
  name: bodyPreview
  type: string
- description: The importance of the message.
  name: importance
  type: string
- description: The unique identifier for the message's parent mailFolder.
  name: parentFolderId
  type: string
- description: The ID of the conversation the email belongs to.
  name: conversationId
  type: string
- description: Indicates the position of the message within the conversation. Binary value encoded as base64.
  name: conversationIndex
  type: string
- description: Indicates whether a delivery receipt is requested for the message.
  name: isDeliveryReceiptRequested
  type:
  - boolean
  - 'null'
- description: Indicates whether a read receipt is requested for the message.
  name: isReadReceiptRequested
  type: boolean
- description: Indicates whether the message has been read.
  name: isRead
  type: boolean
- description: Indicates whether the message is a draft. A message is a draft if it has not been sent yet.
  name: isDraft
  type: boolean
- description: The URL to open the message in Outlook on the web. Append ispopout=0 to show in the review pane instead of a popout window.
  name: webLink
  type: string
- description: The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.
  name: inferenceClassification
  type: string
- description: The follow-up flag value indicating the status, start date, due date, or completion date for the message.
  name: flag
  type: object
- description: The owner of the mailbox from which the message is sent. In most cases, this is the same as the sender property, except for sharing or delegation scenarios.
  name: from
  type: object
- description: The account that is used to generate the message. In most cases, this is the same as the from property. Can differ when sending from a shared mailbox or as a delegate.
  name: sender
  type: object
- description: 'The To: recipients for the message.'
  name: toRecipients
  type: array
- description: 'The Cc: recipients for the message.'
  name: ccRecipients
  type: array
- description: 'The Bcc: recipients for the message.'
  name: bccRecipients
  type: array
- description: The email addresses to use when replying.
  name: replyTo
  type: array
- description: The part of the body of the message that is unique to the current message. Not returned by default; use $select=uniqueBody.
  name: uniqueBody
  type: object
- description: The fileAttachment and itemAttachment attachments for the message.
  name: attachments
  type: array
provider_name: Microsoft Outlook
provider_slug: microsoft-outlook
schema_file: json-schema/microsoft-outlook-message-schema.json
slug: microsoft-outlook-message
source_filename: microsoft-outlook-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-outlook/message\",\n  \"title\": \"Microsoft Outlook Message\",\n  \"description\": \"JSON Schema for a Microsoft Graph message resource representing an email message in a user's mailbox. Based on the microsoft.graph.message resource type from the Microsoft Graph v1.0 API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the message. By default, this value changes when the item is moved from one container to another. Use the Prefer: IdType=\\\"ImmutableId\\\" header for immutable identifiers.\",\n      \"readOnly\": true\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was created. Uses ISO 8601 format in UTC time (e.g., 2014-01-01T00:00:00Z).\",\n      \"readOnly\"\
  : true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was last changed. Uses ISO 8601 format in UTC time.\",\n      \"readOnly\": true\n    },\n    \"changeKey\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the message.\",\n      \"readOnly\": true\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The categories associated with the message.\"\n    },\n    \"receivedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was received. Uses ISO 8601 format in UTC time.\"\n    },\n    \"sentDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the message was sent. Uses ISO 8601 format in UTC time.\"\n    },\n    \"\
  hasAttachments\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message has attachments. This property does not include inline attachments. To verify inline attachments, parse the body property for a src attribute.\"\n    },\n    \"internetMessageId\": {\n      \"type\": \"string\",\n      \"description\": \"The message ID in the format specified by RFC 2822.\"\n    },\n    \"internetMessageHeaders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InternetMessageHeader\"\n      },\n      \"description\": \"A collection of message headers defined by RFC 5322. Includes custom message headers starting with 'x-'. Returned only on applying a $select query option.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject of the message.\"\n    },\n    \"body\": {\n      \"$ref\": \"#/$defs/ItemBody\",\n      \"description\": \"The body of the message. Can be in HTML or text format.\"\n  \
  \  },\n    \"bodyPreview\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"The first 255 characters of the message body in text format.\",\n      \"readOnly\": true\n    },\n    \"importance\": {\n      \"type\": \"string\",\n      \"enum\": [\"low\", \"normal\", \"high\"],\n      \"description\": \"The importance of the message.\"\n    },\n    \"parentFolderId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the message's parent mailFolder.\"\n    },\n    \"conversationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the conversation the email belongs to.\"\n    },\n    \"conversationIndex\": {\n      \"type\": \"string\",\n      \"contentEncoding\": \"base64\",\n      \"description\": \"Indicates the position of the message within the conversation. Binary value encoded as base64.\"\n    },\n    \"isDeliveryReceiptRequested\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\"\
  : \"Indicates whether a delivery receipt is requested for the message.\"\n    },\n    \"isReadReceiptRequested\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether a read receipt is requested for the message.\"\n    },\n    \"isRead\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message has been read.\"\n    },\n    \"isDraft\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the message is a draft. A message is a draft if it has not been sent yet.\"\n    },\n    \"webLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to open the message in Outlook on the web. Append ispopout=0 to show in the review pane instead of a popout window.\",\n      \"readOnly\": true\n    },\n    \"inferenceClassification\": {\n      \"type\": \"string\",\n      \"enum\": [\"focused\", \"other\"],\n      \"description\": \"The classification of the message for the user, based\
  \ on inferred relevance or importance, or on an explicit override.\"\n    },\n    \"flag\": {\n      \"$ref\": \"#/$defs/FollowupFlag\",\n      \"description\": \"The follow-up flag value indicating the status, start date, due date, or completion date for the message.\"\n    },\n    \"from\": {\n      \"$ref\": \"#/$defs/Recipient\",\n      \"description\": \"The owner of the mailbox from which the message is sent. In most cases, this is the same as the sender property, except for sharing or delegation scenarios.\"\n    },\n    \"sender\": {\n      \"$ref\": \"#/$defs/Recipient\",\n      \"description\": \"The account that is used to generate the message. In most cases, this is the same as the from property. Can differ when sending from a shared mailbox or as a delegate.\"\n    },\n    \"toRecipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Recipient\"\n      },\n      \"description\": \"The To: recipients for the message.\"\n    },\n    \"ccRecipients\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Recipient\"\n      },\n      \"description\": \"The Cc: recipients for the message.\"\n    },\n    \"bccRecipients\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Recipient\"\n      },\n      \"description\": \"The Bcc: recipients for the message.\"\n    },\n    \"replyTo\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Recipient\"\n      },\n      \"description\": \"The email addresses to use when replying.\"\n    },\n    \"uniqueBody\": {\n      \"$ref\": \"#/$defs/ItemBody\",\n      \"description\": \"The part of the body of the message that is unique to the current message. Not returned by default; use $select=uniqueBody.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Attachment\"\n      },\n      \"description\": \"The fileAttachment and itemAttachment attachments for the\
  \ message.\"\n    }\n  },\n  \"$defs\": {\n    \"Recipient\": {\n      \"type\": \"object\",\n      \"title\": \"Recipient\",\n      \"description\": \"Represents information about a user in the context of a message (sender, from, to, cc, bcc, replyTo).\",\n      \"properties\": {\n        \"emailAddress\": {\n          \"$ref\": \"#/$defs/EmailAddress\"\n        }\n      },\n      \"required\": [\"emailAddress\"]\n    },\n    \"EmailAddress\": {\n      \"type\": \"object\",\n      \"title\": \"Email Address\",\n      \"description\": \"Represents the name and email address of a person or entity.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the person or entity.\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the person or entity.\"\n        }\n      },\n      \"required\": [\"address\"]\n    },\n\
  \    \"ItemBody\": {\n      \"type\": \"object\",\n      \"title\": \"Item Body\",\n      \"description\": \"Represents the body content of a message, event, or other item.\",\n      \"properties\": {\n        \"contentType\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"html\"],\n          \"description\": \"The type of the content. Possible values are text and html.\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The content of the item body.\"\n        }\n      },\n      \"required\": [\"contentType\", \"content\"]\n    },\n    \"InternetMessageHeader\": {\n      \"type\": \"object\",\n      \"title\": \"Internet Message Header\",\n      \"description\": \"A key-value pair representing an Internet message header as defined by RFC 5322. Custom headers should start with 'x-'.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the message\
  \ header.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value for the message header.\"\n        }\n      },\n      \"required\": [\"name\", \"value\"]\n    },\n    \"FollowupFlag\": {\n      \"type\": \"object\",\n      \"title\": \"Follow-up Flag\",\n      \"description\": \"Represents the follow-up flag status, start date, due date, or completion date for a message.\",\n      \"properties\": {\n        \"flagStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"notFlagged\", \"complete\", \"flagged\"],\n          \"description\": \"The follow-up status for the message.\"\n        },\n        \"startDateTime\": {\n          \"$ref\": \"#/$defs/DateTimeTimeZone\",\n          \"description\": \"The date and time to start the follow up.\"\n        },\n        \"dueDateTime\": {\n          \"$ref\": \"#/$defs/DateTimeTimeZone\",\n          \"description\": \"The date and time the follow up is due.\"\n        },\n   \
  \     \"completedDateTime\": {\n          \"$ref\": \"#/$defs/DateTimeTimeZone\",\n          \"description\": \"The date and time the follow up was completed.\"\n        }\n      },\n      \"required\": [\"flagStatus\"]\n    },\n    \"DateTimeTimeZone\": {\n      \"type\": \"object\",\n      \"title\": \"DateTime with Time Zone\",\n      \"description\": \"Describes the date, time, and time zone of a point in time.\",\n      \"properties\": {\n        \"dateTime\": {\n          \"type\": \"string\",\n          \"description\": \"A single point of time in a combined date and time representation (e.g., 2017-08-29T04:00:00.0000000).\"\n        },\n        \"timeZone\": {\n          \"type\": \"string\",\n          \"description\": \"Represents a time zone (e.g., Pacific Standard Time). See supported time zones.\"\n        }\n      },\n      \"required\": [\"dateTime\", \"timeZone\"]\n    },\n    \"Attachment\": {\n      \"type\": \"object\",\n      \"title\": \"Attachment\",\n      \"description\"\
  : \"Base type for file, item, and reference attachments on a message. Use @odata.type to distinguish between types.\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"#microsoft.graph.fileAttachment\",\n            \"#microsoft.graph.itemAttachment\",\n            \"#microsoft.graph.referenceAttachment\"\n          ],\n          \"description\": \"The OData type discriminator for the attachment.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the attachment.\",\n          \"readOnly\": true\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the attachment. Does not need to be the actual file name.\"\n        },\n        \"contentType\": {\n          \"type\": \"string\",\n          \"description\": \"The MIME type of the attachment.\"\n        },\n        \"size\": {\n      \
  \    \"type\": \"integer\",\n          \"description\": \"The length of the attachment in bytes.\"\n        },\n        \"isInline\": {\n          \"type\": \"boolean\",\n          \"description\": \"True if the attachment is an inline attachment; otherwise, false.\"\n        },\n        \"lastModifiedDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the attachment was last modified in UTC (ISO 8601).\"\n        },\n        \"contentBytes\": {\n          \"type\": \"string\",\n          \"contentEncoding\": \"base64\",\n          \"description\": \"The base64-encoded contents of the file. Only for fileAttachment type.\"\n        },\n        \"contentId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID of the attachment in the Exchange store. Only for fileAttachment type.\"\n        },\n        \"contentLocation\": {\n          \"type\": [\"string\", \"null\"],\n     \
  \     \"description\": \"The URI corresponding to the location of the content of the attachment.\"\n        }\n      },\n      \"required\": [\"@odata.type\"]\n    },\n    \"MailFolder\": {\n      \"type\": \"object\",\n      \"title\": \"Mail Folder\",\n      \"description\": \"A mail folder in a user's mailbox, such as Inbox and Drafts. Mail folders can contain messages, other Outlook items, and child mail folders.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the mail folder.\",\n          \"readOnly\": true\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"The mail folder's display name.\"\n        },\n        \"parentFolderId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the parent mail folder.\"\n        },\n        \"childFolderCount\": {\n          \"type\": \"integer\",\n          \"minimum\"\
  : 0,\n          \"description\": \"The number of immediate child mail folders.\"\n        },\n        \"unreadItemCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of items marked as unread in the folder.\"\n        },\n        \"totalItemCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of items in the folder.\"\n        },\n        \"isHidden\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the mail folder is hidden. Can only be set when creating the folder.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-outlook/refs/heads/main/json-schema/microsoft-outlook-message-schema.json
tags:
- Calendar
- Contacts
- Email
- Enterprise
- Microsoft
- Office 365
- Productivity
title: Microsoft Outlook Message
---
