---
description: An object that represents a local file certificate. The certificate must meet specific requirements and you must have proxy authorization enabled. For more information, see <a href="https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html#virtual-node-tls-prerequisites">Transport Layer Security (TLS)</a>.
layout: schema
name: ListenerTlsFileCertificate
properties_list:
- description: ''
  name: certificateChain
  type: object
- description: ''
  name: privateKey
  type: object
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-listenertlsfilecertificate-schema.json
slug: amazon-app-mesh-listenertlsfilecertificate
source_filename: amazon-app-mesh-listenertlsfilecertificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ListenerTlsFileCertificate\",\n  \"description\": \"An object that represents a local file certificate. The certificate must meet specific requirements and you must have proxy authorization enabled. For more information, see <a href=\\\"https://docs.aws.amazon.com/app-mesh/latest/userguide/tls.html#virtual-node-tls-prerequisites\\\">Transport Layer Security (TLS)</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateChain\": {},\n    \"privateKey\": {}\n  },\n  \"required\": [\n    \"certificateChain\",\n    \"privateKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-listenertlsfilecertificate-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: ListenerTlsFileCertificate
---
