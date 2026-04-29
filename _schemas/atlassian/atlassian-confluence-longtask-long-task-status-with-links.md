---
description: 'Same as LongTaskStatus but with `_links` property. Status keys: - `ERROR_UNKNOWN` - Generic error - `ERROR_LOCK_FAILED` - Could not get the lock on destination space - `ERROR_RELINK` - Error when relink pages/attachments - `ERROR_COPY_PAGE` - Error while copying 1 page - `WARN_RENAME_PAGE` - Warning page is rename during copy - `WARN_IGNORE_COPY_PERMISSION` - Warning could not copy permission - `WARN_IGNORE_COPY_ATTACHMENT` - Warning could not copy attachment - `WARN_IGNORE_DELETE_PAGE` - Warning ignoring delete of a non agreed on page - `STATUS_COPIED_PAGES` - Message total pages are copied - `STATUS_COPYING_PAGES` - Message copy pages - `STATUS_RELINK_PAGES` - Message relink pages/attachments - `STATUS_DELETING_PAGES` - Message delete pages - `STATUS_DELETED_PAGES` - Message total pages are deleted - `STATUS_MOVING_PAGES` - Message move pages - `WARN_IGNORE_VIEW_RESTRICTED` - Permission changed - view restricted - `WARN_IGNORE_EDIT_RESTRICTED` - Permission changed - edit
  restricted - `INITIALIZING_TASK` - Message when initializing task - `UNKNOWN_STATUS` - Message when status is unknown'
layout: schema
name: LongTaskStatusWithLinks
properties_list:
- description: the ARI for the long task, based on its ID
  name: ari
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: object
- description: ''
  name: elapsedTime
  type: integer
- description: ''
  name: percentageComplete
  type: integer
- description: ''
  name: successful
  type: boolean
- description: ''
  name: finished
  type: boolean
- description: ''
  name: messages
  type: array
- description: ''
  name: status
  type: string
- description: ''
  name: errors
  type: array
- description: ''
  name: additionalDetails
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-longtask-long-task-status-with-links-schema.json
slug: atlassian-confluence-longtask-long-task-status-with-links
source_filename: atlassian-confluence-longtask-long-task-status-with-links-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LongTaskStatusWithLinks\",\n  \"type\": \"object\",\n  \"description\": \"Same as LongTaskStatus but with `_links` property.\\n\\nStatus keys:\\n\\n- `ERROR_UNKNOWN` - Generic error\\n- `ERROR_LOCK_FAILED` - Could not get the lock on destination space\\n- `ERROR_RELINK` - Error when relink pages/attachments\\n- `ERROR_COPY_PAGE` - Error while copying 1 page\\n- `WARN_RENAME_PAGE` - Warning page is rename during copy\\n- `WARN_IGNORE_COPY_PERMISSION` - Warning could not copy permission\\n- `WARN_IGNORE_COPY_ATTACHMENT` - Warning could not copy attachment\\n- `WARN_IGNORE_DELETE_PAGE` - Warning ignoring delete of a non agreed on page\\n- `STATUS_COPIED_PAGES` - Message total pages are copied\\n- `STATUS_COPYING_PAGES` - Message copy pages\\n- `STATUS_RELINK_PAGES` - Message relink pages/attachments\\n- `STATUS_DELETING_PAGES` - Message delete pages\\n- `STATUS_DELETED_PAGES` - Message total pages\
  \ are deleted\\n- `STATUS_MOVING_PAGES` - Message move pages\\n- `WARN_IGNORE_VIEW_RESTRICTED` - Permission changed - view restricted\\n- `WARN_IGNORE_EDIT_RESTRICTED` - Permission changed - edit restricted\\n- `INITIALIZING_TASK` - Message when initializing task\\n- `UNKNOWN_STATUS` - Message when status is unknown\",\n  \"properties\": {\n    \"ari\": {\n      \"type\": \"string\",\n      \"description\": \"the ARI for the long task, based on its ID\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"object\"\n    },\n    \"elapsedTime\": {\n      \"type\": \"integer\"\n    },\n    \"percentageComplete\": {\n      \"type\": \"integer\"\n    },\n    \"successful\": {\n      \"type\": \"boolean\"\n    },\n    \"finished\": {\n      \"type\": \"boolean\"\n    },\n    \"messages\": {\n      \"type\": \"array\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"errors\": {\n      \"type\": \"array\"\n    },\n    \"additionalDetails\"\
  : {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-longtask-long-task-status-with-links-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: LongTaskStatusWithLinks
---
