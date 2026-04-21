---
description: A File represents a stored file in the Appmixer file management system, which can be used by flows and components.
layout: schema
name: Appmixer File
properties_list:
- description: Unique identifier for the file.
  name: fileId
  type: string
- description: Original filename of the uploaded file.
  name: filename
  type: string
- description: File size in bytes.
  name: length
  type: integer
- description: MIME type of the file.
  name: contentType
  type: string
- description: Timestamp when the file was uploaded.
  name: createdAt
  type: string
provider_name: Appmixer
provider_slug: appmixer
schema_file: json-schema/file.json
slug: file
tags:
- Agentic
- Automation
- Embedded iPaaS
- Integrations
- Low-Code
- Workflows
title: Appmixer File
---
