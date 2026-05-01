---
description: Schema representing a Drupal content node entity with its system metadata, publication status, revision tracking, language, and field values. Nodes are the primary content entities in Drupal and may belong to any configured content type (bundle) such as article or page.
layout: schema
name: Drupal Node
properties_list:
- description: The unique numeric node ID assigned by Drupal upon creation. Used in internal references and REST API paths.
  name: nid
  type: integer
- description: The universally unique identifier of the node. Used as the primary identifier in the JSON:API module.
  name: uuid
  type: string
- description: The current revision ID. Increments each time a new revision is saved.
  name: vid
  type: integer
- description: The language code for this node translation (e.g., en, fr, de). Follows BCP 47 format.
  name: langcode
  type: string
- description: The machine name of the content type (bundle) this node belongs to, such as article or page.
  name: type
  type: string
- description: The title of the content node. Required for all node types.
  name: title
  type: string
- description: Publication status of the node. True means the node is published and publicly accessible. False means it is unpublished and only visible to privileged users.
  name: status
  type: boolean
- description: Whether the node is promoted to the front page of the Drupal site.
  name: promote
  type: boolean
- description: Whether the node is displayed at the top of content lists regardless of sort order.
  name: sticky
  type: boolean
- description: Unix timestamp of when the current revision was created.
  name: revision_timestamp
  type: integer
- description: The numeric user ID of the user who created the current revision.
  name: revision_uid
  type: integer
- description: Optional log message describing the changes made in the current revision.
  name: revision_log
  type:
  - string
  - 'null'
- description: Whether this revision reflects a translation change. True if this revision was created due to a change in a translated version.
  name: revision_translation_affected
  type:
  - boolean
  - 'null'
- description: The numeric user ID of the user who originally authored the node.
  name: uid
  type: integer
- description: Unix timestamp of when the node was originally created.
  name: created
  type: integer
- description: Unix timestamp of when the node was last modified.
  name: changed
  type: integer
- description: Comment status for this node. 0 = comments hidden, 1 = comments closed, 2 = comments open.
  name: comment
  type: integer
- description: The main body field of the node. Contains text value, optional summary, and the text format applied.
  name: body
  type: object
- description: The URL alias configuration for the node's canonical path.
  name: path
  type: object
- description: Array of taxonomy term references used to tag or categorize this node. Available when the tags field is configured on the content type.
  name: field_tags
  type: array
- description: Image field reference to a file entity. Available when an image field is configured on the content type.
  name: field_image
  type: object
- description: Meta tag values for SEO and social sharing, available when the Metatag module is installed.
  name: metatag
  type: object
provider_name: drupal
provider_slug: drupal
schema_file: json-schema/drupal-node-schema.json
slug: drupal-node
source_filename: drupal-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://drupal.org/schemas/drupal/node.json\",\n  \"title\": \"Drupal Node\",\n  \"description\": \"Schema representing a Drupal content node entity with its system metadata, publication status, revision tracking, language, and field values. Nodes are the primary content entities in Drupal and may belong to any configured content type (bundle) such as article or page.\",\n  \"type\": \"object\",\n  \"required\": [\"nid\", \"uuid\", \"type\", \"title\", \"status\", \"langcode\"],\n  \"properties\": {\n    \"nid\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique numeric node ID assigned by Drupal upon creation. Used in internal references and REST API paths.\",\n      \"minimum\": 1\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The universally unique identifier of the node. Used as the primary identifier in the JSON:API\
  \ module.\"\n    },\n    \"vid\": {\n      \"type\": \"integer\",\n      \"description\": \"The current revision ID. Increments each time a new revision is saved.\",\n      \"minimum\": 1\n    },\n    \"langcode\": {\n      \"type\": \"string\",\n      \"description\": \"The language code for this node translation (e.g., en, fr, de). Follows BCP 47 format.\",\n      \"pattern\": \"^[a-z]{2}(-[A-Z]{2})?$\",\n      \"examples\": [\"en\", \"fr\", \"de\", \"es\", \"ja\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The machine name of the content type (bundle) this node belongs to, such as article or page.\",\n      \"pattern\": \"^[a-z][a-z0-9_]*$\",\n      \"examples\": [\"article\", \"page\", \"blog_post\", \"landing_page\"]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the content node. Required for all node types.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"status\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Publication status of the node. True means the node is published and publicly accessible. False means it is unpublished and only visible to privileged users.\"\n    },\n    \"promote\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the node is promoted to the front page of the Drupal site.\"\n    },\n    \"sticky\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the node is displayed at the top of content lists regardless of sort order.\"\n    },\n    \"revision_timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the current revision was created.\",\n      \"minimum\": 0\n    },\n    \"revision_uid\": {\n      \"type\": \"integer\",\n      \"description\": \"The numeric user ID of the user who created the current revision.\",\n      \"minimum\": 0\n    },\n    \"revision_log\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Optional log message\
  \ describing the changes made in the current revision.\",\n      \"maxLength\": 255\n    },\n    \"revision_translation_affected\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"Whether this revision reflects a translation change. True if this revision was created due to a change in a translated version.\"\n    },\n    \"uid\": {\n      \"type\": \"integer\",\n      \"description\": \"The numeric user ID of the user who originally authored the node.\",\n      \"minimum\": 0\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the node was originally created.\",\n      \"minimum\": 0\n    },\n    \"changed\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the node was last modified.\",\n      \"minimum\": 0\n    },\n    \"comment\": {\n      \"type\": \"integer\",\n      \"description\": \"Comment status for this node. 0 = comments hidden, 1 = comments closed, 2 = comments open.\"\
  ,\n      \"enum\": [0, 1, 2]\n    },\n    \"body\": {\n      \"$ref\": \"#/$defs/TextItem\",\n      \"description\": \"The main body field of the node. Contains text value, optional summary, and the text format applied.\"\n    },\n    \"path\": {\n      \"$ref\": \"#/$defs/PathAlias\",\n      \"description\": \"The URL alias configuration for the node's canonical path.\"\n    },\n    \"field_tags\": {\n      \"type\": \"array\",\n      \"description\": \"Array of taxonomy term references used to tag or categorize this node. Available when the tags field is configured on the content type.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EntityReference\"\n      }\n    },\n    \"field_image\": {\n      \"description\": \"Image field reference to a file entity. Available when an image field is configured on the content type.\",\n      \"$ref\": \"#/$defs/ImageItem\"\n    },\n    \"metatag\": {\n      \"type\": \"object\",\n      \"description\": \"Meta tag values for SEO and social sharing,\
  \ available when the Metatag module is installed.\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value pairs of meta tag names and their values.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"TextItem\": {\n      \"type\": \"object\",\n      \"description\": \"A Drupal formatted text field value with optional summary and format specification.\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The full text content. May contain HTML markup depending on the configured text format.\"\n        },\n        \"summary\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Optional trimmed summary of the text. Used for teaser views if provided.\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"description\": \"The machine name of the text format applied to this field (e.g., basic_html, full_html,\
  \ plain_text, restricted_html).\",\n          \"examples\": [\"basic_html\", \"full_html\", \"plain_text\", \"restricted_html\"]\n        },\n        \"processed\": {\n          \"type\": \"string\",\n          \"description\": \"The text value after applying the text format filters. Read-only, computed by Drupal.\"\n        }\n      }\n    },\n    \"EntityReference\": {\n      \"type\": \"object\",\n      \"description\": \"A Drupal entity reference field value pointing to another entity.\",\n      \"required\": [\"target_id\"],\n      \"properties\": {\n        \"target_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The numeric ID of the referenced entity.\",\n          \"minimum\": 1\n        },\n        \"target_type\": {\n          \"type\": \"string\",\n          \"description\": \"The entity type of the referenced entity (e.g., taxonomy_term, node, user).\"\n        },\n        \"target_uuid\": {\n          \"type\": \"string\",\n          \"format\": \"\
  uuid\",\n          \"description\": \"The UUID of the referenced entity.\"\n        }\n      }\n    },\n    \"ImageItem\": {\n      \"type\": \"object\",\n      \"description\": \"A Drupal image field value with file reference and display metadata.\",\n      \"required\": [\"target_id\"],\n      \"properties\": {\n        \"target_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The numeric file entity ID of the referenced image.\",\n          \"minimum\": 1\n        },\n        \"alt\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Alternative text for the image, used for accessibility and SEO.\",\n          \"maxLength\": 512\n        },\n        \"title\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Optional title attribute for the image, shown as tooltip on hover.\",\n          \"maxLength\": 1024\n        },\n        \"width\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\"\
  : \"The pixel width of the image.\",\n          \"minimum\": 1\n        },\n        \"height\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The pixel height of the image.\",\n          \"minimum\": 1\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The absolute URL to the image file. Computed field, read-only.\"\n        }\n      }\n    },\n    \"PathAlias\": {\n      \"type\": \"object\",\n      \"description\": \"A Drupal URL alias configuration for an entity's canonical path.\",\n      \"properties\": {\n        \"alias\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The URL alias path starting with a forward slash (e.g., /my-article-title). Null if no alias is configured.\",\n          \"pattern\": \"^\\\\/.*\"\n        },\n        \"pid\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"The numeric path ID for\
  \ this alias. Null if no alias exists.\",\n          \"minimum\": 1\n        },\n        \"langcode\": {\n          \"type\": \"string\",\n          \"description\": \"The language code for this path alias.\",\n          \"pattern\": \"^[a-z]{2}(-[A-Z]{2})?$\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/drupal/refs/heads/main/json-schema/drupal-node-schema.json
tags: []
title: Drupal Node
---
