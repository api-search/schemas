---
description: Schema for a Confluence Cloud space resource as returned by the REST API v2. A space is the top-level organizational container in Confluence, holding pages, blog posts, and other content.
layout: schema
name: Confluence Space
properties_list:
- description: The unique identifier of the space.
  name: id
  type: string
- description: The unique key of the space. Used in URLs and as a human-readable identifier. Must be alphanumeric and uppercase.
  name: key
  type: string
- description: The display name of the space.
  name: name
  type: string
- description: The type of space. Global spaces are accessible to all users; personal spaces belong to an individual user.
  name: type
  type: string
- description: The lifecycle status of the space.
  name: status
  type: string
- description: The Atlassian account ID of the user who created the space.
  name: authorId
  type: string
- description: The ISO 8601 date-time when the space was created.
  name: createdAt
  type: string
- description: The ID of the space homepage. Every space has a homepage that serves as the root of the page tree.
  name: homepageId
  type:
  - string
  - 'null'
- description: ''
  name: description
  type: object
- description: ''
  name: icon
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
  name: permissions
  type: object
- description: ''
  name: _links
  type: object
provider_name: Confluence
provider_slug: confluence
schema_file: json-schema/confluence-space-schema.json
slug: confluence-space
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/confluence/space\",\n  \"title\": \"Confluence Space\",\n  \"description\": \"Schema for a Confluence Cloud space resource as returned by the REST API v2. A space is the top-level organizational container in Confluence, holding pages, blog posts, and other content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the space.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique key of the space. Used in URLs and as a human-readable identifier. Must be alphanumeric and uppercase.\",\n      \"pattern\": \"^[A-Z][A-Z0-9]*$\",\n      \"maxLength\": 255\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the space.\",\n      \"maxLength\": 200\n    },\n    \"type\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The type of space. Global spaces are accessible to all users; personal spaces belong to an individual user.\",\n      \"enum\": [\"global\", \"personal\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle status of the space.\",\n      \"enum\": [\"current\", \"archived\"]\n    },\n    \"authorId\": {\n      \"type\": \"string\",\n      \"description\": \"The Atlassian account ID of the user who created the space.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 date-time when the space was created.\"\n    },\n    \"homepageId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of the space homepage. Every space has a homepage that serves as the root of the page tree.\"\n    },\n    \"description\": {\n      \"$ref\": \"#/$defs/SpaceDescription\"\n    },\n    \"icon\": {\n      \"$ref\": \"#/$defs/SpaceIcon\"\
  \n    },\n    \"labels\": {\n      \"$ref\": \"#/$defs/LabelArray\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/$defs/SpacePropertyArray\"\n    },\n    \"operations\": {\n      \"$ref\": \"#/$defs/OperationArray\"\n    },\n    \"permissions\": {\n      \"$ref\": \"#/$defs/SpacePermissionArray\"\n    },\n    \"_links\": {\n      \"$ref\": \"#/$defs/SpaceLinks\"\n    }\n  },\n  \"required\": [\"id\", \"key\", \"name\", \"type\", \"status\", \"authorId\", \"createdAt\"],\n  \"$defs\": {\n    \"SpaceDescription\": {\n      \"type\": \"object\",\n      \"title\": \"Space Description\",\n      \"description\": \"The description of the space in available representation formats.\",\n      \"properties\": {\n        \"plain\": {\n          \"$ref\": \"#/$defs/BodyRepresentation\",\n          \"description\": \"The plain text representation of the space description.\"\n        },\n        \"view\": {\n          \"$ref\": \"#/$defs/BodyRepresentation\",\n          \"description\": \"The rendered\
  \ HTML view of the space description.\"\n        }\n      }\n    },\n    \"SpaceIcon\": {\n      \"type\": \"object\",\n      \"title\": \"Space Icon\",\n      \"description\": \"The icon associated with the space.\",\n      \"properties\": {\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"The relative path to the space icon image.\"\n        },\n        \"apiDownloadLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri-reference\",\n          \"description\": \"The API download link for the space icon.\"\n        }\n      }\n    },\n    \"BodyRepresentation\": {\n      \"type\": \"object\",\n      \"title\": \"Body Representation\",\n      \"description\": \"A single representation of content.\",\n      \"properties\": {\n        \"representation\": {\n          \"type\": \"string\",\n          \"description\": \"The name of this representation format.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n         \
  \ \"description\": \"The content in this representation format.\"\n        }\n      },\n      \"required\": [\"representation\", \"value\"]\n    },\n    \"Label\": {\n      \"type\": \"object\",\n      \"title\": \"Label\",\n      \"description\": \"A label used to categorize and organize content.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the label.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the label.\"\n        },\n        \"prefix\": {\n          \"type\": \"string\",\n          \"description\": \"The prefix indicating the label scope.\",\n          \"enum\": [\"global\", \"my\", \"team\"]\n        }\n      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"LabelArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"items\": {\n    \
  \        \"$ref\": \"#/$defs/Label\"\n          }\n        },\n        \"_links\": {\n          \"$ref\": \"#/$defs/PaginationLinks\"\n        }\n      }\n    },\n    \"SpaceProperty\": {\n      \"type\": \"object\",\n      \"title\": \"Space Property\",\n      \"description\": \"A key-value property stored on a space for custom metadata.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the property.\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the property.\"\n        },\n        \"value\": {\n          \"description\": \"The value of the property. Can be any valid JSON value.\"\n        },\n        \"version\": {\n          \"$ref\": \"#/$defs/Version\"\n        }\n      },\n      \"required\": [\"id\", \"key\"]\n    },\n    \"SpacePropertyArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n        \
  \  \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/SpaceProperty\"\n          }\n        }\n      }\n    },\n    \"Version\": {\n      \"type\": \"object\",\n      \"title\": \"Version\",\n      \"description\": \"Version metadata for a resource.\",\n      \"properties\": {\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The ISO 8601 date-time when this version was created.\"\n        },\n        \"message\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"An optional message describing the changes in this version.\"\n        },\n        \"number\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The version number.\"\n        },\n        \"minorEdit\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version was a minor edit.\"\n        },\n        \"authorId\": {\n         \
  \ \"type\": \"string\",\n          \"description\": \"The Atlassian account ID of the user who created this version.\"\n        }\n      },\n      \"required\": [\"number\", \"createdAt\", \"authorId\"]\n    },\n    \"Operation\": {\n      \"type\": \"object\",\n      \"title\": \"Operation\",\n      \"description\": \"An operation that can be performed on a space.\",\n      \"properties\": {\n        \"operation\": {\n          \"type\": \"string\",\n          \"description\": \"The operation type.\",\n          \"enum\": [\"create\", \"read\", \"update\", \"delete\", \"administer\"]\n        },\n        \"targetType\": {\n          \"type\": \"string\",\n          \"description\": \"The target type for the operation.\"\n        }\n      },\n      \"required\": [\"operation\"]\n    },\n    \"OperationArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Operation\"\
  \n          }\n        }\n      }\n    },\n    \"SpacePermission\": {\n      \"type\": \"object\",\n      \"title\": \"Space Permission\",\n      \"description\": \"A permission entry controlling access to the space.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the permission entry.\"\n        },\n        \"principal\": {\n          \"type\": \"object\",\n          \"description\": \"The user, group, or role that this permission applies to.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"The type of principal.\",\n              \"enum\": [\"user\", \"group\", \"role\"]\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"The identifier of the principal.\"\n            }\n          },\n          \"required\": [\"type\", \"id\"]\n        },\n        \"operation\":\
  \ {\n          \"$ref\": \"#/$defs/Operation\"\n        }\n      },\n      \"required\": [\"id\", \"principal\", \"operation\"]\n    },\n    \"SpacePermissionArray\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"results\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/SpacePermission\"\n          }\n        }\n      }\n    },\n    \"SpaceLinks\": {\n      \"type\": \"object\",\n      \"title\": \"Space Links\",\n      \"description\": \"Hypermedia links associated with the space.\",\n      \"properties\": {\n        \"webui\": {\n          \"type\": \"string\",\n          \"format\": \"uri-reference\",\n          \"description\": \"Relative path to view the space in the Confluence web UI.\"\n        }\n      }\n    },\n    \"PaginationLinks\": {\n      \"type\": \"object\",\n      \"title\": \"Pagination Links\",\n      \"description\": \"Links for cursor-based pagination through result sets.\",\n      \"properties\": {\n\
  \        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for the next page of results.\"\n        },\n        \"base\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The base URL of the Confluence instance.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/confluence/refs/heads/main/json-schema/confluence-space-schema.json
tags:
- Collaboration
- Content Management
- Documentation
- Knowledge Base
- Wiki
title: Confluence Space
---
