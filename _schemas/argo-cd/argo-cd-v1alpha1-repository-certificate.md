---
description: v1alpha1RepositoryCertificate schema from Argo CD API
layout: schema
name: v1alpha1RepositoryCertificate
properties_list:
- description: ''
  name: certData
  type: string
- description: ''
  name: certInfo
  type: string
- description: ''
  name: certSubType
  type: string
- description: ''
  name: certType
  type: string
- description: ''
  name: serverName
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-repository-certificate-schema.json
slug: argo-cd-v1alpha1-repository-certificate
source_filename: argo-cd-v1alpha1-repository-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-repository-certificate-schema.json\",\n  \"title\": \"v1alpha1RepositoryCertificate\",\n  \"description\": \"v1alpha1RepositoryCertificate schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certData\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"title\": \"CertData contains the actual certificate data, dependent on the certificate type\"\n    },\n    \"certInfo\": {\n      \"type\": \"string\",\n      \"title\": \"CertInfo will hold additional certificate info, depdendent on the certificate type (e.g. SSH fingerprint, X509 CommonName)\"\n    },\n    \"certSubType\": {\n      \"type\": \"string\",\n      \"title\": \"CertSubType specifies the sub type of the cert, i.e. \\\"ssh-rsa\\\"\"\n    },\n    \"certType\": {\n      \"type\": \"string\"\
  ,\n      \"title\": \"CertType specifies the type of the certificate - currently one of \\\"https\\\" or \\\"ssh\\\"\"\n    },\n    \"serverName\": {\n      \"type\": \"string\",\n      \"title\": \"ServerName specifies the DNS name of the server this certificate is intended for\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-repository-certificate-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1RepositoryCertificate
---
