---
description: An access-control entry for an object.
layout: schema
name: ObjectAccessControl
properties_list:
- description: The kind of item this is.
  name: kind
  type: string
- description: The ID of the access-control entry.
  name: id
  type: string
- description: The link to this access-control entry.
  name: selfLink
  type: string
- description: The name of the bucket.
  name: bucket
  type: string
- description: The name of the object.
  name: object
  type: string
- description: The content generation of the object.
  name: generation
  type: string
- description: 'The entity holding the permission, in one of the following forms: user-userId, user-email, group-groupId, group-email, domain-domain, project-team-projectId, allUsers, or allAuthenticatedUsers.'
  name: entity
  type: string
- description: The access permission for the entity.
  name: role
  type: string
- description: The email address associated with the entity, if any.
  name: email
  type: string
- description: The domain associated with the entity, if any.
  name: domain
  type: string
- description: The ID for the entity, if any.
  name: entityId
  type: string
- description: HTTP 1.1 Entity tag for the access-control entry.
  name: etag
  type: string
- description: The project team associated with the entity, if any.
  name: projectTeam
  type: object
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
schema_file: json-schema/gcp-cloud-storage-json-object-access-control-schema.json
slug: gcp-cloud-storage-json-object-access-control
source_filename: gcp-cloud-storage-json-object-access-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectAccessControl\",\n  \"type\": \"object\",\n  \"description\": \"An access-control entry for an object.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of item this is.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the access-control entry.\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"description\": \"The link to this access-control entry.\"\n    },\n    \"bucket\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\"\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the object.\"\n    },\n    \"generation\": {\n      \"type\": \"string\",\n      \"description\": \"The content generation of the object.\"\n    },\n    \"entity\": {\n      \"type\": \"string\",\n      \"description\": \"The entity\
  \ holding the permission, in one of the following forms: user-userId, user-email, group-groupId, group-email, domain-domain, project-team-projectId, allUsers, or allAuthenticatedUsers.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The access permission for the entity.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address associated with the entity, if any.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain associated with the entity, if any.\"\n    },\n    \"entityId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID for the entity, if any.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP 1.1 Entity tag for the access-control entry.\"\n    },\n    \"projectTeam\": {\n      \"type\": \"object\",\n      \"description\": \"The project team associated with the entity, if any.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/json-schema/gcp-cloud-storage-json-object-access-control-schema.json
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
title: ObjectAccessControl
---
