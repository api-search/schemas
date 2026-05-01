---
description: A custom TLS certificate used to terminate TLS traffic for one or more fully qualified domain names on Fastly's edge network. Certificates can be managed via the Custom TLS or Platform TLS APIs.
layout: schema
name: Fastly TLS Certificate
properties_list:
- description: The alphanumeric string identifying the TLS certificate.
  name: id
  type: string
- description: The resource type identifier.
  name: type
  type: string
- description: The certificate attributes.
  name: attributes
  type: object
- description: Related resources for the certificate.
  name: relationships
  type: object
provider_name: fastly
provider_slug: fastly
schema_file: json-schema/fastly-tls-certificate-schema.json
slug: fastly-tls-certificate
source_filename: fastly-tls-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/fastly/tls-certificate.json\",\n  \"title\": \"Fastly TLS Certificate\",\n  \"description\": \"A custom TLS certificate used to terminate TLS traffic for one or more fully qualified domain names on Fastly's edge network. Certificates can be managed via the Custom TLS or Platform TLS APIs.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The alphanumeric string identifying the TLS certificate.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier.\",\n      \"enum\": [\"tls_certificate\"]\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"The certificate attributes.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"A customizable name for the certificate.\"\n        },\n        \"cert_blob\": {\n          \"type\": \"string\",\n          \"description\": \"The PEM-encoded certificate data.\"\n        },\n        \"issued_to\": {\n          \"type\": \"string\",\n          \"description\": \"The common name of the entity the certificate was issued to.\"\n        },\n        \"issuer\": {\n          \"type\": \"string\",\n          \"description\": \"The certificate authority that issued the certificate.\"\n        },\n        \"serial_number\": {\n          \"type\": \"string\",\n          \"description\": \"The serial number of the certificate.\"\n        },\n        \"signature_algorithm\": {\n          \"type\": \"string\",\n          \"description\": \"The algorithm used to sign the certificate.\"\n        },\n        \"not_before\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date the certificate becomes valid.\"\n        },\n\
  \        \"not_after\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date the certificate expires.\"\n        },\n        \"replace\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the certificate is a replacement for another.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the certificate was created.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the certificate was last updated.\"\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Related resources for the certificate.\",\n      \"properties\": {\n        \"tls_domains\": {\n          \"type\": \"object\",\n          \"description\": \"The TLS domains associated with\
  \ the certificate.\",\n          \"properties\": {\n            \"data\": {\n              \"type\": \"array\",\n              \"description\": \"A list of TLS domain references.\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"description\": \"The domain name.\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"description\": \"The resource type.\",\n                    \"enum\": [\"tls_domain\"]\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/json-schema/fastly-tls-certificate-schema.json
tags: []
title: Fastly TLS Certificate
---
