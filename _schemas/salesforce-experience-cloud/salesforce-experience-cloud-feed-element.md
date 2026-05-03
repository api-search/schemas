---
description: Represents a feed element (post, announcement, or bundle) in an Experience Cloud site community feed.
layout: schema
name: Feed Element
properties_list:
- description: Unique identifier of the feed element
  name: id
  type: string
- description: Type of the feed element
  name: feedElementType
  type: string
- description: When the feed element was created
  name: createdDate
  type: string
- description: When the feed element was last modified
  name: modifiedDate
  type: string
- description: The user who created the feed element
  name: actor
  type: object
- description: The parent record or user of the feed element
  name: parent
  type: object
- description: The rich text body of the feed element
  name: body
  type: object
- description: The header text of the feed element
  name: header
  type: object
- description: Capabilities available on this feed element (comments, likes, etc.)
  name: capabilities
  type: object
- description: API resource URL for this feed element
  name: url
  type: string
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
schema_file: json-schema/salesforce-experience-cloud-feed-element-schema.json
slug: salesforce-experience-cloud-feed-element
source_filename: salesforce-experience-cloud-feed-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/experience-cloud/feed-element.json\",\n  \"title\": \"Feed Element\",\n  \"description\": \"Represents a feed element (post, announcement, or bundle) in an Experience Cloud site community feed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the feed element\"\n    },\n    \"feedElementType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the feed element\",\n      \"enum\": [\"FeedItem\", \"Bundle\", \"Recommendation\"]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the feed element was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the feed element was last modified\"\n    },\n\
  \    \"actor\": {\n      \"$ref\": \"#/$defs/ActorReference\",\n      \"description\": \"The user who created the feed element\"\n    },\n    \"parent\": {\n      \"$ref\": \"#/$defs/ActorReference\",\n      \"description\": \"The parent record or user of the feed element\"\n    },\n    \"body\": {\n      \"$ref\": \"#/$defs/MessageBody\",\n      \"description\": \"The rich text body of the feed element\"\n    },\n    \"header\": {\n      \"$ref\": \"#/$defs/MessageBody\",\n      \"description\": \"The header text of the feed element\"\n    },\n    \"capabilities\": {\n      \"type\": \"object\",\n      \"description\": \"Capabilities available on this feed element (comments, likes, etc.)\",\n      \"properties\": {\n        \"comments\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"page\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"currentPageToken\": { \"type\": \"string\" },\n                \"currentPageUrl\"\
  : { \"type\": \"string\", \"format\": \"uri\" },\n                \"nextPageToken\": { \"type\": \"string\" },\n                \"nextPageUrl\": { \"type\": \"string\", \"format\": \"uri\" },\n                \"total\": { \"type\": \"integer\" },\n                \"comments\": {\n                  \"type\": \"array\",\n                  \"items\": { \"$ref\": \"#/$defs/Comment\" }\n                }\n              }\n            }\n          }\n        },\n        \"chatterLikes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"page\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"total\": { \"type\": \"integer\" },\n                \"likes\": {\n                  \"type\": \"array\",\n                  \"items\": { \"$ref\": \"#/$defs/Like\" }\n                }\n              }\n            },\n            \"myLike\": {\n              \"$ref\": \"#/$defs/Like\"\n            }\n          }\n        },\n     \
  \   \"topics\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"items\": {\n              \"type\": \"array\",\n              \"items\": { \"$ref\": \"#/$defs/TopicReference\" }\n            }\n          }\n        },\n        \"bookmarks\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isBookmarkedByCurrentUser\": { \"type\": \"boolean\" }\n          }\n        }\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API resource URL for this feed element\"\n    }\n  },\n  \"required\": [\"id\", \"feedElementType\"],\n  \"$defs\": {\n    \"ActorReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a user or record that acts as an actor\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"type\": { \"type\": \"string\" },\n        \"url\": { \"type\": \"string\"\
  , \"format\": \"uri\" }\n      },\n      \"required\": [\"id\"]\n    },\n    \"MessageBody\": {\n      \"type\": \"object\",\n      \"description\": \"Rich text message body composed of typed segments\",\n      \"properties\": {\n        \"isRichText\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the body contains rich text formatting\"\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Plain text representation of the body\"\n        },\n        \"messageSegments\": {\n          \"type\": \"array\",\n          \"description\": \"Typed segments composing the message body\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"Text\", \"Mention\", \"Hashtag\", \"Link\", \"MarkupBegin\", \"MarkupEnd\", \"InlineImage\", \"EntityLink\"]\n              },\n              \"text\": { \"type\"\
  : \"string\" },\n              \"name\": { \"type\": \"string\" },\n              \"id\": { \"type\": \"string\" },\n              \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n            },\n            \"required\": [\"type\"]\n          }\n        }\n      }\n    },\n    \"Comment\": {\n      \"type\": \"object\",\n      \"description\": \"A comment on a feed element\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"body\": { \"$ref\": \"#/$defs/MessageBody\" },\n        \"createdDate\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"user\": { \"$ref\": \"#/$defs/ActorReference\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n      },\n      \"required\": [\"id\"]\n    },\n    \"Like\": {\n      \"type\": \"object\",\n      \"description\": \"A like on a feed element or comment\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"createdDate\": { \"type\": \"string\", \"format\"\
  : \"date-time\" },\n        \"user\": { \"$ref\": \"#/$defs/ActorReference\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    },\n    \"TopicReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a topic associated with the feed element\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/json-schema/salesforce-experience-cloud-feed-element-schema.json
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
title: Feed Element
---
