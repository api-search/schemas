---
description: A project is a high-level Google Cloud entity. It is a container for ACLs, APIs, App Engine Apps, VMs, and other Google Cloud Platform resources. Projects are the base-level organizing entity and are required to use service-level resources.
layout: schema
name: Project
properties_list:
- description: The unique resource name of the project in the form projects/{project_number}. Output only.
  name: name
  type: string
- description: The resource name of the parent in the form folders/{folder_id} or organizations/{organization_id}. Required when creating a project.
  name: parent
  type: string
- description: The unique, user-assigned identifier of the project. It must be 6 to 30 lowercase ASCII letters, digits, or hyphens. It must start with a letter and cannot end with a hyphen. Project IDs are immutable
  name: projectId
  type: string
- description: The project lifecycle state. Output only.
  name: state
  type: string
- description: A user-assigned display name for the project. This field is optional and has a maximum length of 30 characters. Display names are used for identification purposes and do not need to be unique.
  name: displayName
  type: string
- description: Timestamp of when the project was created. Output only. Uses RFC 3339 format.
  name: createTime
  type: string
- description: Timestamp of when the project was last modified. Output only. Uses RFC 3339 format.
  name: updateTime
  type: string
- description: Timestamp of when the delete request was sent. Only present when the project is in DELETE_REQUESTED state. Output only.
  name: deleteTime
  type: string
- description: A checksum computed by the server based on the current value of the project resource. Used for optimistic concurrency control.
  name: etag
  type: string
- description: User-defined labels associated with the project. Label keys must be between 1 and 63 characters, and label values must be between 0 and 63 characters. Both keys and values can contain lowercase letter
  name: labels
  type: object
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-project-schema.json
slug: cloud-resource-manager-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Project\",\n  \"type\": \"object\",\n  \"description\": \"A project is a high-level Google Cloud entity. It is a container for ACLs, APIs, App Engine Apps, VMs, and other Google Cloud Platform resources. Projects are the base-level organizing entity and are required to use service-level resources.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique resource name of the project in the form projects/{project_number}. Output only.\"\n    },\n    \"parent\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the parent in the form folders/{folder_id} or organizations/{organization_id}. Required when creating a project.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique, user-assigned identifier of the project. It must be 6 to 30 lowercase ASCII letters, digits, or hyphens.\
  \ It must start with a letter and cannot end with a hyphen. Project IDs are immutable and cannot be reused once assigned.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The project lifecycle state. Output only.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-assigned display name for the project. This field is optional and has a maximum length of 30 characters. Display names are used for identification purposes and do not need to be unique.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the project was created. Output only. Uses RFC 3339 format.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the project was last modified. Output only. Uses RFC 3339 format.\"\n    },\n    \"deleteTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of when the delete request was sent.\
  \ Only present when the project is in DELETE_REQUESTED state. Output only.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"A checksum computed by the server based on the current value of the project resource. Used for optimistic concurrency control.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined labels associated with the project. Label keys must be between 1 and 63 characters, and label values must be between 0 and 63 characters. Both keys and values can contain lowercase letters, numeric characters, underscores, and dashes. A maximum of 256 labels can be associated with a project.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-project-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: Project
---
