---
description: Returns information about an HSM client certificate. The certificate is stored in a secure Hardware Storage Module (HSM), and used by the Amazon Redshift cluster to encrypt data files.
layout: schema
name: HsmClientCertificate
properties_list:
- description: ''
  name: HsmClientCertificateIdentifier
  type: object
- description: ''
  name: HsmClientCertificatePublicKey
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-hsm-client-certificate-schema.json
slug: redshift-hsm-client-certificate
source_filename: redshift-hsm-client-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"HsmClientCertificateIdentifier\": {},\n    \"HsmClientCertificatePublicKey\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"Returns information about an HSM client certificate. The certificate is stored in a secure Hardware Storage Module (HSM), and used by the Amazon Redshift cluster to encrypt data files.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-hsm-client-certificate-schema.json\",\n  \"title\": \"HsmClientCertificate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-hsm-client-certificate-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: HsmClientCertificate
---
