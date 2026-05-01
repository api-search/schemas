---
description: Schema for a Certificate Manager certificate resource, representing a TLS certificate managed or uploaded for use with Google Cloud services.
layout: schema
name: Google Cloud Certificate Manager Certificate
properties_list:
- description: The resource name of the certificate
  name: name
  type: string
- description: A human-readable description of the certificate
  name: description
  type: string
- description: Labels associated with the certificate
  name: labels
  type: object
- description: Configuration for a Google-managed certificate
  name: managed
  type: object
- description: Configuration for a self-managed certificate
  name: selfManaged
  type: object
- description: Subject Alternative Names of the certificate
  name: sanDnsnames
  type: array
- description: The PEM-encoded certificate chain
  name: pemCertificate
  type: string
- description: The expiration time of the certificate
  name: expireTime
  type: string
- description: The creation time of the certificate
  name: createTime
  type: string
- description: The last update time of the certificate
  name: updateTime
  type: string
- description: The scope of the certificate
  name: scope
  type: string
provider_name: Google Cloud Certificate Manager
provider_slug: google-cloud-certificate-manager
schema_file: json-schema/google-cloud-certificate-manager-certificate-schema.json
slug: google-cloud-certificate-manager-certificate
source_filename: google-cloud-certificate-manager-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/certificatemanager/certificate.json\",\n  \"title\": \"Google Cloud Certificate Manager Certificate\",\n  \"description\": \"Schema for a Certificate Manager certificate resource, representing a TLS certificate managed or uploaded for use with Google Cloud services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the certificate\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the certificate\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Labels associated with the certificate\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"managed\": {\n      \"$ref\": \"#/$defs/ManagedCertificate\",\n      \"description\": \"Configuration\
  \ for a Google-managed certificate\"\n    },\n    \"selfManaged\": {\n      \"$ref\": \"#/$defs/SelfManagedCertificate\",\n      \"description\": \"Configuration for a self-managed certificate\"\n    },\n    \"sanDnsnames\": {\n      \"type\": \"array\",\n      \"description\": \"Subject Alternative Names of the certificate\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pemCertificate\": {\n      \"type\": \"string\",\n      \"description\": \"The PEM-encoded certificate chain\"\n    },\n    \"expireTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The expiration time of the certificate\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation time of the certificate\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The last update time of the certificate\"\n  \
  \  },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope of the certificate\",\n      \"enum\": [\"DEFAULT\", \"EDGE_CACHE\", \"ALL_REGIONS\"]\n    }\n  },\n  \"$defs\": {\n    \"ManagedCertificate\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for a Google-managed certificate\",\n      \"properties\": {\n        \"domains\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The domains for which the certificate should be provisioned\"\n        },\n        \"dnsAuthorizations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Resource names of DNS authorizations for the certificate\"\n        },\n        \"issuanceConfig\": {\n          \"type\": \"string\",\n          \"description\": \"The resource name of the issuance configuration\"\n        },\n      \
  \  \"state\": {\n          \"type\": \"string\",\n          \"description\": \"The provisioning state of the managed certificate\",\n          \"enum\": [\"PROVISIONING\", \"FAILED\", \"ACTIVE\"]\n        },\n        \"provisioningIssue\": {\n          \"type\": \"object\",\n          \"description\": \"Information about provisioning issues\",\n          \"properties\": {\n            \"reason\": {\n              \"type\": \"string\",\n              \"enum\": [\"AUTHORIZATION_ISSUE\", \"RATE_LIMITED\"]\n            },\n            \"details\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"SelfManagedCertificate\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for a self-managed certificate\",\n      \"properties\": {\n        \"pemCertificate\": {\n          \"type\": \"string\",\n          \"description\": \"PEM-encoded certificate chain\"\n        },\n        \"pemPrivateKey\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"PEM-encoded private key\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-certificate-manager/refs/heads/main/json-schema/google-cloud-certificate-manager-certificate-schema.json
tags:
- Certificate Management
- Certificates
- Load Balancing
- Security
- SSL
- TLS
title: Google Cloud Certificate Manager Certificate
---
