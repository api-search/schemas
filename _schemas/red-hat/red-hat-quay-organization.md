---
description: A Quay organization.
layout: schema
name: Organization
properties_list:
- description: The name of the organization.
  name: name
  type: string
- description: The organization contact email.
  name: email
  type: string
- description: Whether invoices are sent to the organization email.
  name: invoice_email
  type: boolean
- description: Whether the current user is an admin of this organization.
  name: is_admin
  type: boolean
- description: Whether the current user is a member of this organization.
  name: is_member
  type: boolean
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-quay-organization-schema.json
slug: red-hat-quay-organization
source_filename: red-hat-quay-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Organization\",\n  \"type\": \"object\",\n  \"description\": \"A Quay organization.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the organization.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The organization contact email.\"\n    },\n    \"invoice_email\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether invoices are sent to the organization email.\"\n    },\n    \"is_admin\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current user is an admin of this organization.\"\n    },\n    \"is_member\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the current user is a member of this organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-quay-organization-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Organization
---
