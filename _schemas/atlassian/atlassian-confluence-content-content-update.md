---
description: ''
layout: schema
name: ContentUpdate
properties_list:
- description: The new version for the updated content. Set this to the current version number incremented by one, unless you are changing the status to 'draft' which must have a version number of 1. To get the curr
  name: version
  type: object
- description: The updated title of the content. If you are updating a non-draft `page` or `blogpost`, title is required. If you are not changing the title, set this field to the the current title.
  name: title
  type: string
- description: The type of content. Set this to the current type of the content. For example, - page - blogpost - comment - attachment
  name: type
  type: string
- description: The updated status of the content. Note, if you change the status of a page from 'current' to 'draft' and it has an existing draft, the existing draft will be deleted in favor of the updated page.
  name: status
  type: string
- description: The new parent for the content. Only one parent content 'id' can be specified.
  name: ancestors
  type: array
- description: 'The updated body of the content. Does not apply to attachments. If you are not sure how to generate these formats, you can create a page in the Confluence application, retrieve the content using [Get '
  name: body
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-update-schema.json
slug: atlassian-confluence-content-content-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"object\",\n      \"description\": \"The new version for the updated content. Set this to the current version number incremented by one, unless you are changing the status to 'draft' which must have a version number of 1.\\n\\nTo get the current version number, use [Get content by ID](#api-content-id-get) and retrieve `version.number`.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The updated title of the content. If you are updating a non-draft `page` or `blogpost`, title is required. If you are not changing the title, set this field to the the current title.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of content. Set this to the current type of the content. For example, - page - blogpost - comment - attachment\"\
  \n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The updated status of the content. Note, if you change the status of a page from\\n'current' to 'draft' and it has an existing draft, the existing draft will be deleted\\nin favor of the updated page.\"\n    },\n    \"ancestors\": {\n      \"type\": \"array\",\n      \"description\": \"The new parent for the content. Only one parent content 'id' can be specified.\"\n    },\n    \"body\": {\n      \"type\": \"object\",\n      \"description\": \"The updated body of the content. Does not apply to attachments.\\nIf you are not sure how to generate these formats, you can create a page in the\\nConfluence application, retrieve the content using [Get content](#api-content-get),\\nand expand the desired content format, e.g. `expand=body.storage`.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-update-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentUpdate
---
