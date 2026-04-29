---
description: ''
layout: schema
name: RetrievalRequest
properties_list:
- description: Natural language query string used to retrieve relevant text extracts. Should be a single sentence. Avoid spelling errors in context-rich keywords.
  name: queryString
  type: string
- description: Indicates whether extracts should be retrieved from SharePoint, OneDrive, or Copilot connectors.
  name: dataSource
  type: string
- description: Keyword Query Language (KQL) expression with queryable properties to scope retrieval. Supports AND, OR, NOT, and inequality operators. Supported SharePoint/OneDrive properties include Author, FileExte
  name: filterExpression
  type: string
- description: List of metadata fields to return for each item. Only retrievable metadata properties can be included. By default, no metadata is returned.
  name: resourceMetadata
  type: array
- description: Number of results to return. Must be between 1 and 25. Defaults to 25.
  name: maximumNumberOfResults
  type: integer
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-retrieval-request-schema.json
slug: microsoft-copilot-retrieval-request
source_filename: microsoft-copilot-retrieval-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RetrievalRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queryString\": {\n      \"type\": \"string\",\n      \"description\": \"Natural language query string used to retrieve relevant text extracts. Should be a single sentence. Avoid spelling errors in context-rich keywords.\"\n    },\n    \"dataSource\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether extracts should be retrieved from SharePoint, OneDrive, or Copilot connectors.\"\n    },\n    \"filterExpression\": {\n      \"type\": \"string\",\n      \"description\": \"Keyword Query Language (KQL) expression with queryable properties to scope retrieval. Supports AND, OR, NOT, and inequality operators. Supported SharePoint/OneDrive properties include Author, FileExtension, Filename, FileType, InformationProtectionLabelId, LastModifiedTime, ModifiedBy, Path, SiteID, and Title.\"\n    },\n    \"resourceMetadata\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"List of metadata fields to return for each item. Only retrievable metadata properties can be included. By default, no metadata is returned.\"\n    },\n    \"maximumNumberOfResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of results to return. Must be between 1 and 25. Defaults to 25.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-retrieval-request-schema.json
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft 365
- Productivity
title: RetrievalRequest
---
