---
description: CreateHsmClientCertificateResult schema from Amazon Redshift
layout: schema
name: CreateHsmClientCertificateResult
properties_list:
- description: Returns information about an HSM client certificate. The certificate is stored in a secure Hardware Storage Module (HSM), and used by the Amazon Redshift cluster to encrypt data files.
  name: HsmClientCertificate
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-hsm-client-certificate-result-schema.json
slug: redshift-create-hsm-client-certificate-result
source_filename: redshift-create-hsm-client-certificate-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"HsmClientCertificate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"HsmClientCertificateIdentifier\": {},\n        \"HsmClientCertificatePublicKey\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"Returns information about an HSM client certificate. The certificate is stored in a secure Hardware Storage Module (HSM), and used by the Amazon Redshift cluster to encrypt data files.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-hsm-client-certificate-result-schema.json\",\n  \"title\": \"CreateHsmClientCertificateResult\",\n  \"description\": \"CreateHsmClientCertificateResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-hsm-client-certificate-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateHsmClientCertificateResult
---
