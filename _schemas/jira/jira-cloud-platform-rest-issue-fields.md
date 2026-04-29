---
description: The fields of a Jira issue.
layout: schema
name: IssueFields
properties_list:
- description: The summary (title) of the issue.
  name: summary
  type: string
- description: The description of the issue in Atlassian Document Format (ADF).
  name: description
  type: string
- description: The user assigned to the issue.
  name: assignee
  type: string
- description: Labels applied to the issue.
  name: labels
  type: array
- description: Components associated with the issue.
  name: components
  type: array
- description: Fix versions for the issue.
  name: fixVersions
  type: array
- description: Affected versions for the issue.
  name: versions
  type: array
- description: The resolution of the issue.
  name: resolution
  type: string
- description: The date the issue was resolved.
  name: resolutiondate
  type: '[''string'', ''null'']'
- description: The date and time the issue was created.
  name: created
  type: string
- description: The date and time the issue was last updated.
  name: updated
  type: string
- description: The due date of the issue.
  name: duedate
  type: '[''string'', ''null'']'
- description: Sub-tasks of the issue.
  name: subtasks
  type: array
- description: The parent issue, if this is a sub-task.
  name: parent
  type: string
- description: The environment in which the issue was found in ADF.
  name: environment
  type: string
- description: Attachments on the issue.
  name: attachment
  type: array
- description: Links to other issues.
  name: issuelinks
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-issue-fields-schema.json
slug: jira-cloud-platform-rest-issue-fields
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IssueFields\",\n  \"type\": \"object\",\n  \"description\": \"The fields of a Jira issue.\",\n  \"properties\": {\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"The summary (title) of the issue.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the issue in Atlassian Document Format (ADF).\"\n    },\n    \"assignee\": {\n      \"type\": \"string\",\n      \"description\": \"The user assigned to the issue.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels applied to the issue.\"\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"description\": \"Components associated with the issue.\"\n    },\n    \"fixVersions\": {\n      \"type\": \"array\",\n      \"description\": \"Fix versions for the issue.\"\n    },\n    \"versions\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Affected versions for the issue.\"\n    },\n    \"resolution\": {\n      \"type\": \"string\",\n      \"description\": \"The resolution of the issue.\"\n    },\n    \"resolutiondate\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The date the issue was resolved.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the issue was created.\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the issue was last updated.\"\n    },\n    \"duedate\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The due date of the issue.\"\n    },\n    \"subtasks\": {\n      \"type\": \"array\",\n      \"description\": \"Sub-tasks of the issue.\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"The parent issue, if this is a sub-task.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"The environment in which the issue was found in ADF.\"\n    },\n    \"attachment\": {\n      \"type\": \"array\",\n      \"description\": \"Attachments on the issue.\"\n    },\n    \"issuelinks\": {\n      \"type\": \"array\",\n      \"description\": \"Links to other issues.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-issue-fields-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: IssueFields
---
