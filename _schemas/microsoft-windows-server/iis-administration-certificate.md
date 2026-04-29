---
description: An SSL/TLS certificate associated with an HTTPS binding.
layout: schema
name: Certificate
properties_list:
- description: The friendly name of the certificate.
  name: name
  type: string
- description: The unique identifier of the certificate resource.
  name: id
  type: string
- description: The certificate issuer distinguished name.
  name: issued_by
  type: string
- description: The certificate subject distinguished name.
  name: subject
  type: string
- description: The SHA-1 thumbprint of the certificate.
  name: thumbprint
  type: string
- description: The expiration date of the certificate.
  name: valid_to
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-certificate-schema.json
slug: iis-administration-certificate
source_filename: iis-administration-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Certificate\",\n  \"type\": \"object\",\n  \"description\": \"An SSL/TLS certificate associated with an HTTPS binding.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name of the certificate.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the certificate resource.\"\n    },\n    \"issued_by\": {\n      \"type\": \"string\",\n      \"description\": \"The certificate issuer distinguished name.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The certificate subject distinguished name.\"\n    },\n    \"thumbprint\": {\n      \"type\": \"string\",\n      \"description\": \"The SHA-1 thumbprint of the certificate.\"\n    },\n    \"valid_to\": {\n      \"type\": \"string\",\n      \"description\": \"The expiration date of the certificate.\"\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-certificate-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: Certificate
---
