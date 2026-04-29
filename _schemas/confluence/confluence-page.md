---
description: Schema for a Confluence Cloud page resource as returned by the REST API v2. A page is the primary content type in Confluence, representing a wiki-style document within a space.
layout: schema
name: Confluence Page
properties_list:
- description: The unique identifier of the page. Represented as a string in the v2 API.
  name: id
  type: string
- description: The current lifecycle status of the page.
  name: status
  type: string
- description: The title of the page. Must be unique within the space for current pages.
  name: title
  type: string
- description: The ID of the space this page belongs to.
  name: spaceId
  type: string
- description: The ID of the parent page. Null for top-level pages in a space.
  name: parentId
  type:
  - string
  - 'null'
- description: The type of the parent entity.
  name: parentType
  type: string
- description: The ordinal position of this page among its siblings in the page tree.
  name: position
  type:
  - integer
  - 'null'
- description: The Atlassian account ID of the user who originally created the page.
  name: authorId
  type: string
- description: The Atlassian account ID of the current page owner.
  name: ownerId
  type: string
- description: The Atlassian account ID of the previous page owner.
  name: lastOwnerId
  type:
  - string
  - 'null'
- description: The ISO 8601 date-time when the page was originally created.
  name: createdAt
  type: string
- description: ''
  name: version
  type: object
- description: ''
  name: body
  type: object
- description: ''
  name: labels
  type: object
- description: ''
  name: properties
  type: object
- description: ''
  name: operations
  type: object
- description: ''
  name: likes
  type: object
- description: ''
  name: versions
  type: object
- description: ''
  name: _links
  type: object
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-page-schema.json
slug: confluence-page
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/confluence/page\",\n  \"title\": \"Confluence Page\",\n  \"description\": \"Schema for a Confluence Cloud page resource as returned by the REST API v2. A page is the primary content type in Confluence, representing a wiki-style document within a space.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the page. Represented as a string in the v2 API.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current lifecycle status of the page.\",\n      \"enum\": [\"current\", \"draft\", \"archived\", \"trashed\"]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the page. Must be unique within the space for current pages.\",\n      \"maxLength\": 255\n    },\n    \"spaceId\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The ID of the space this page belongs to.\"\n    },\n    \"parentId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the parent page. Null for top-level pages in a space.\"\n    },\n    \"parentType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the parent entity.\",\n      \"enum\": [\"page\", \"space\"]\n    },\n    \"position\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The ordinal position of this page among its siblings in the page tree.\"\n    },\n    \"authorId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the user who originally created the page.\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the current page owner.\"\n    },\n    \"lastOwnerId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The Atlassian account ID of the previous\
  \ page owner.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 date-time when the page was originally created.\"\n    },\n    \"version\": {\n      \"$ref\": \"#/$defs/Version\"\n    },\n    \"body\": {\n      \"$ref\": \"#/$defs/Body\"\n    },\n    \"labels\": {\n      \"$ref\": \"#/$defs/LabelArray\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/$defs/ContentPropertyArray\"\n    },\n    \"operations\": {\n      \"$ref\": \"#/$defs/OperationArray\"\n    },\n    \"likes\": {\n      \"$ref\": \"#/$defs/LikeArray\"\n    },\n    \"versions\": {\n      \"$ref\": \"#/$defs/VersionArray\"\n    },\n    \"_links\": {\n      \"$ref\": \"#/$defs/PageLinks\"\n    }\n  },\n  \"required\": [\"id\", \"status\", \"title\", \"spaceId\", \"authorId\", \"createdAt\", \"version\"],\n  \"$defs\": {\n    \"Version\": {\n      \"type\": \"object\",\n      \"title\": \"Version\",\n      \"description\": \"Version metadata\
  \ for the content. Each edit creates a new version.\",\n      \"properties\": {\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The ISO 8601 date-time when this version was created.\"\n        },\n        \"message\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"An optional message describing the changes in this version.\"\n        },\n        \"number\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The version number. Starts at 1 and increments with each update.\"\n        },\n        \"minorEdit\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version was saved as a minor edit. Minor edits do not trigger notifications.\"\n        },\n        \"authorId\": {\n          \"type\": \"string\",\n          \"description\": \"The Atlassian account ID of the user who created this version.\"\n        }\n\
  \      },\n      \"required\": [\"number\", \"createdAt\", \"authorId\"]\n    },\n    \"VersionArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Version\"\n          }\n        },\n        \"_links\": {\n          \"$ref\": \"#/$defs/PaginationLinks\"\n        }\n      }\n    },\n    \"Body\": {\n      \"type\": \"object\",\n      \"title\": \"Body\",\n      \"description\": \"The content body in one or more representation formats.\",\n      \"properties\": {\n        \"storage\": {\n          \"$ref\": \"#/$defs/BodyRepresentation\",\n          \"description\": \"The storage format representation (XHTML-based).\"\n        },\n        \"atlas_doc_format\": {\n          \"$ref\": \"#/$defs/BodyRepresentation\",\n          \"description\": \"The Atlassian Document Format (ADF) representation.\"\n        },\n        \"view\": {\n          \"$ref\": \"#/$defs/BodyRepresentation\"\
  ,\n          \"description\": \"The rendered HTML view representation.\"\n        }\n      }\n    },\n    \"BodyRepresentation\": {\n      \"type\": \"object\",\n      \"title\": \"Body Representation\",\n      \"description\": \"A single representation of the content body.\",\n      \"properties\": {\n        \"representation\": {\n          \"type\": \"string\",\n          \"description\": \"The name of this representation format.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The content body in this representation format.\"\n        }\n      },\n      \"required\": [\"representation\", \"value\"]\n    },\n    \"Label\": {\n      \"type\": \"object\",\n      \"title\": \"Label\",\n      \"description\": \"A label used to categorize and organize content in Confluence.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the label.\"\n        },\n     \
  \   \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the label.\"\n        },\n        \"prefix\": {\n          \"type\": \"string\",\n          \"description\": \"The prefix indicating the label scope.\",\n          \"enum\": [\"global\", \"my\", \"team\"]\n        }\n      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"LabelArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Label\"\n          }\n        },\n        \"_links\": {\n          \"$ref\": \"#/$defs/PaginationLinks\"\n        }\n      }\n    },\n    \"ContentProperty\": {\n      \"type\": \"object\",\n      \"title\": \"Content Property\",\n      \"description\": \"A key-value property stored on content for app-specific or custom metadata.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The unique identifier of the property.\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the property.\"\n        },\n        \"value\": {\n          \"description\": \"The value of the property. Can be any valid JSON value.\"\n        },\n        \"version\": {\n          \"$ref\": \"#/$defs/Version\"\n        }\n      },\n      \"required\": [\"id\", \"key\"]\n    },\n    \"ContentPropertyArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ContentProperty\"\n          }\n        }\n      }\n    },\n    \"Operation\": {\n      \"type\": \"object\",\n      \"title\": \"Operation\",\n      \"description\": \"An operation that can be performed on content.\",\n      \"properties\": {\n        \"operation\": {\n          \"type\": \"string\",\n          \"description\": \"The operation type.\",\n        \
  \  \"enum\": [\"create\", \"read\", \"update\", \"delete\", \"administer\"]\n        },\n        \"targetType\": {\n          \"type\": \"string\",\n          \"description\": \"The target type for the operation.\"\n        }\n      },\n      \"required\": [\"operation\"]\n    },\n    \"OperationArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Operation\"\n          }\n        }\n      }\n    },\n    \"Like\": {\n      \"type\": \"object\",\n      \"title\": \"Like\",\n      \"description\": \"A like on the content by a specific user.\",\n      \"properties\": {\n        \"accountId\": {\n          \"type\": \"string\",\n          \"description\": \"The Atlassian account ID of the user who liked the content.\"\n        }\n      },\n      \"required\": [\"accountId\"]\n    },\n    \"LikeArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n       \
  \ \"results\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Like\"\n          }\n        }\n      }\n    },\n    \"PageLinks\": {\n      \"type\": \"object\",\n      \"title\": \"Page Links\",\n      \"description\": \"Hypermedia links associated with the page.\",\n      \"properties\": {\n        \"webui\": {\n          \"type\": \"string\",\n          \"format\": \"uri-reference\",\n          \"description\": \"Relative path to view the page in the Confluence web UI.\"\n        },\n        \"editui\": {\n          \"type\": \"string\",\n          \"format\": \"uri-reference\",\n          \"description\": \"Relative path to edit the page in the Confluence editor.\"\n        },\n        \"tinyui\": {\n          \"type\": \"string\",\n          \"format\": \"uri-reference\",\n          \"description\": \"Shortened relative path for sharing the page.\"\n        }\n      }\n    },\n    \"PaginationLinks\": {\n      \"type\": \"object\",\n    \
  \  \"title\": \"Pagination Links\",\n      \"description\": \"Links for cursor-based pagination through result sets.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the next page of results, including the cursor parameter.\"\n        },\n        \"base\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The base URL of the Confluence instance.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-page-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Confluence Page
---
