---
description: Represents a published version of managed CMS content delivered through Experience Cloud channels.
layout: schema
name: Managed Content Version
properties_list:
- description: Salesforce record ID of the managed content item
  name: managedContentId
  type: string
- description: Unique content key used for content retrieval and referencing
  name: contentKey
  type: string
- description: URL-friendly name for the content, used in page URLs
  name: contentUrlName
  type: string
- description: Display title of the content item
  name: title
  type: string
- description: Developer name of the content type (e.g., news, cms_image, cms_document)
  name: type
  type: string
- description: Human-readable label for the content type
  name: typeLabel
  type: string
- description: Language code of this content version (e.g., en_US)
  name: language
  type: string
- description: ISO 8601 timestamp when this content version was published
  name: publishedDate
  type: string
- description: Current publication status of the content
  name: status
  type: string
- description: Content field values organized as typed nodes, keyed by field name
  name: contentNodes
  type: object
- description: Public URL for accessing this content without authentication
  name: unauthenticatedUrl
  type: string
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
schema_file: json-schema/salesforce-experience-cloud-managed-content-schema.json
slug: salesforce-experience-cloud-managed-content
source_filename: salesforce-experience-cloud-managed-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/experience-cloud/managed-content.json\",\n  \"title\": \"Managed Content Version\",\n  \"description\": \"Represents a published version of managed CMS content delivered through Experience Cloud channels.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"managedContentId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce record ID of the managed content item\"\n    },\n    \"contentKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique content key used for content retrieval and referencing\"\n    },\n    \"contentUrlName\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly name for the content, used in page URLs\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title of the content item\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Developer name of the content type (e.g., news, cms_image, cms_document)\"\n    },\n    \"typeLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable label for the content type\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code of this content version (e.g., en_US)\",\n      \"pattern\": \"^[a-z]{2}(_[A-Z]{2})?$\"\n    },\n    \"publishedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when this content version was published\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current publication status of the content\",\n      \"enum\": [\"Draft\", \"Published\", \"Archived\"]\n    },\n    \"contentNodes\": {\n      \"type\": \"object\",\n      \"description\": \"Content field values organized as typed nodes, keyed by field name\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/ContentNode\"\
  \n      }\n    },\n    \"unauthenticatedUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Public URL for accessing this content without authentication\"\n    }\n  },\n  \"required\": [\"managedContentId\", \"contentKey\", \"title\", \"type\"],\n  \"$defs\": {\n    \"ContentNode\": {\n      \"type\": \"object\",\n      \"description\": \"A typed content node representing a field value within managed content\",\n      \"properties\": {\n        \"nodeType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of the content node determining how the value should be interpreted\",\n          \"enum\": [\"Media\", \"MediaSource\", \"MultilineText\", \"NameField\", \"RichText\", \"Text\", \"Url\", \"DateTime\"]\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Text or scalar value of the node\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\
  ,\n          \"description\": \"URL value for Media and Url node types\"\n        },\n        \"altText\": {\n          \"type\": \"string\",\n          \"description\": \"Alternative text for accessibility (Media node type)\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"Title of the content node\"\n        },\n        \"fileName\": {\n          \"type\": \"string\",\n          \"description\": \"Original file name for media content\"\n        },\n        \"mediaType\": {\n          \"type\": \"string\",\n          \"description\": \"Classification of media content (e.g., Image, Document, Video)\"\n        },\n        \"mimeType\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the content (e.g., image/png, application/pdf)\"\n        },\n        \"referenceId\": {\n          \"type\": \"string\",\n          \"description\": \"Reference identifier for the content\"\n        },\n        \"contentKey\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Content key for referenced content items\"\n        },\n        \"unauthenticatedUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Public URL for unauthenticated access to the content\"\n        }\n      },\n      \"required\": [\"nodeType\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/json-schema/salesforce-experience-cloud-managed-content-schema.json
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
title: Managed Content Version
---
