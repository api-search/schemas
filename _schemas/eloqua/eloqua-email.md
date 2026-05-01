---
description: An email asset in Oracle Eloqua used for marketing communications, including subject line, sender information, HTML/plain text content, tracking configuration, and associated forms and images.
layout: schema
name: Eloqua Email
properties_list:
- description: Unique identifier for the email
  name: id
  type: string
- description: Asset type in Eloqua
  name: type
  type: string
- description: Email name
  name: name
  type: string
- description: Email description
  name: description
  type: string
- description: Email subject line
  name: subject
  type: string
- description: Sender name displayed to recipients
  name: senderName
  type: string
- description: Sender email address displayed to recipients
  name: senderEmail
  type: string
- description: Reply-to email address
  name: replyToEmail
  type: string
- description: Reply-to display name
  name: replyToName
  type: string
- description: Preheader text shown in email clients
  name: previewText
  type: string
- description: ''
  name: htmlContent
  type: object
- description: Plain text version of the email
  name: plainText
  type: string
- description: Whether to send as plain text only
  name: sendPlainTextOnly
  type: boolean
- description: Whether Eloqua tracks opens and clicks
  name: isTracked
  type: string
- description: Whether the email is private to the creator
  name: isPrivate
  type: string
- description: Whether the email is in content protection mode
  name: isContentProtected
  type: string
- description: Current email status
  name: currentStatus
  type: string
- description: Email main layout template
  name: layout
  type: string
- description: Email layout style
  name: style
  type: string
- description: Email layout rendering mode
  name: renderMode
  type: string
- description: Whether the email is archived
  name: archived
  type: boolean
- description: Associated email header identifier
  name: emailHeaderId
  type: string
- description: Associated email footer identifier
  name: emailFooterId
  type: string
- description: Associated email group identifier
  name: emailGroupId
  type: string
- description: Forms embedded in the email
  name: forms
  type: array
- description: Images used in the email
  name: images
  type: array
- description: Hyperlinks in the email
  name: hyperlinks
  type: array
- description: Content sections in the email
  name: contentSections
  type: array
- description: Dynamic content blocks in the email
  name: dynamicContents
  type: array
- description: Field merge tokens in the email
  name: fieldMerges
  type: array
- description: Containing folder identifier
  name: folderId
  type: string
- description: Level of detail returned for the email
  name: depth
  type: string
- description: Granted permissions on this email
  name: permissions
  type: array
- description: Creation timestamp (Unix time)
  name: createdAt
  type: string
- description: User login who created the email
  name: createdBy
  type: string
- description: Display name of the user who created the email
  name: createdByName
  type: string
- description: Last update timestamp (Unix time)
  name: updatedAt
  type: string
- description: User login who last updated the email
  name: updatedBy
  type: string
- description: Display name of the user who last updated the email
  name: updatedByName
  type: string
provider_name: Oracle Eloqua
provider_slug: eloqua
schema_file: json-schema/eloqua-email-schema.json
slug: eloqua-email
source_filename: eloqua-email-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/en/cloud/saas/marketing/eloqua-rest-api/schemas/email.json\",\n  \"title\": \"Eloqua Email\",\n  \"description\": \"An email asset in Oracle Eloqua used for marketing communications, including subject line, sender information, HTML/plain text content, tracking configuration, and associated forms and images.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the email\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Asset type in Eloqua\",\n      \"const\": \"Email\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Email name\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Email description\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Email subject line\"\n    },\n    \"senderName\": {\n      \"type\": \"string\",\n      \"description\": \"Sender name displayed to recipients\"\n    },\n    \"senderEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Sender email address displayed to recipients\"\n    },\n    \"replyToEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Reply-to email address\"\n    },\n    \"replyToName\": {\n      \"type\": \"string\",\n      \"description\": \"Reply-to display name\"\n    },\n    \"previewText\": {\n      \"type\": \"string\",\n      \"description\": \"Preheader text shown in email clients\",\n      \"maxLength\": 500\n    },\n    \"htmlContent\": {\n      \"$ref\": \"#/$defs/HtmlContent\"\n    },\n    \"plainText\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text version of\
  \ the email\"\n    },\n    \"sendPlainTextOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to send as plain text only\"\n    },\n    \"isTracked\": {\n      \"type\": \"string\",\n      \"description\": \"Whether Eloqua tracks opens and clicks\"\n    },\n    \"isPrivate\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the email is private to the creator\"\n    },\n    \"isContentProtected\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the email is in content protection mode\"\n    },\n    \"currentStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current email status\",\n      \"readOnly\": true\n    },\n    \"layout\": {\n      \"type\": \"string\",\n      \"description\": \"Email main layout template\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"Email layout style\"\n    },\n    \"renderMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"fixed\", \"flow\"],\n\
  \      \"description\": \"Email layout rendering mode\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email is archived\"\n    },\n    \"emailHeaderId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated email header identifier\"\n    },\n    \"emailFooterId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated email footer identifier\"\n    },\n    \"emailGroupId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated email group identifier\"\n    },\n    \"forms\": {\n      \"type\": \"array\",\n      \"description\": \"Forms embedded in the email\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssetReference\"\n      },\n      \"readOnly\": true\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"description\": \"Images used in the email\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssetReference\"\n      },\n      \"readOnly\": true\n    },\n    \"hyperlinks\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Hyperlinks in the email\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Hyperlink\"\n      },\n      \"readOnly\": true\n    },\n    \"contentSections\": {\n      \"type\": \"array\",\n      \"description\": \"Content sections in the email\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssetReference\"\n      },\n      \"readOnly\": true\n    },\n    \"dynamicContents\": {\n      \"type\": \"array\",\n      \"description\": \"Dynamic content blocks in the email\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssetReference\"\n      },\n      \"readOnly\": true\n    },\n    \"fieldMerges\": {\n      \"type\": \"array\",\n      \"description\": \"Field merge tokens in the email\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AssetReference\"\n      },\n      \"readOnly\": true\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"Containing folder identifier\",\n      \"readOnly\": true\n\
  \    },\n    \"depth\": {\n      \"type\": \"string\",\n      \"enum\": [\"minimal\", \"partial\", \"complete\"],\n      \"description\": \"Level of detail returned for the email\",\n      \"readOnly\": true\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"Granted permissions on this email\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Creation timestamp (Unix time)\",\n      \"readOnly\": true\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User login who created the email\",\n      \"readOnly\": true\n    },\n    \"createdByName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user who created the email\",\n      \"readOnly\": true\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Last update timestamp (Unix time)\",\n  \
  \    \"readOnly\": true\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"User login who last updated the email\",\n      \"readOnly\": true\n    },\n    \"updatedByName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user who last updated the email\",\n      \"readOnly\": true\n    }\n  },\n  \"$defs\": {\n    \"HtmlContent\": {\n      \"type\": \"object\",\n      \"description\": \"HTML content container for the email\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Content type identifier\"\n        },\n        \"contentSource\": {\n          \"type\": \"string\",\n          \"description\": \"HTML source content of the email\"\n        }\n      }\n    },\n    \"AssetReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to an associated asset\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n      \
  \    \"description\": \"Asset identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Asset name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Asset type\"\n        }\n      }\n    },\n    \"Hyperlink\": {\n      \"type\": \"object\",\n      \"description\": \"A hyperlink in the email content\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Hyperlink identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Hyperlink name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Hyperlink type\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Hyperlink URL\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/json-schema/eloqua-email-schema.json
tags:
- CRM
- Email Marketing
- Lead Management
- Marketing Automation
title: Eloqua Email
---
