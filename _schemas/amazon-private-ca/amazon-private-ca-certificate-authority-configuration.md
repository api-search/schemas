---
description: Contains configuration information for your private certificate authority (CA). This includes information about the class of public key algorithm and the key pair that your private CA creates when it issues a certificate. It also includes the signature algorithm that it uses when issuing certificates, and its X.500 distinguished name. You must specify this information when you call the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html">CreateCertificateAuthority</a> action.
layout: schema
name: CertificateAuthorityConfiguration
properties_list:
- description: ''
  name: KeyAlgorithm
  type: object
- description: ''
  name: SigningAlgorithm
  type: object
- description: ''
  name: Subject
  type: object
- description: ''
  name: CsrExtensions
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-certificate-authority-configuration-schema.json
slug: amazon-private-ca-certificate-authority-configuration
source_filename: amazon-private-ca-certificate-authority-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-certificate-authority-configuration-schema.json\",\n  \"title\": \"CertificateAuthorityConfiguration\",\n  \"description\": \"Contains configuration information for your private certificate authority (CA). This includes information about the class of public key algorithm and the key pair that your private CA creates when it issues a certificate. It also includes the signature algorithm that it uses when issuing certificates, and its X.500 distinguished name. You must specify this information when you call the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html\\\">CreateCertificateAuthority</a> action. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KeyAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/KeyAlgorithm\"\n        },\n        {\n          \"description\": \"Type of the public key algorithm and size, in bits, of the key pair that your CA creates when it issues a certificate. When you create a subordinate CA, you must use a key algorithm supported by the parent CA.\"\n        }\n      ]\n    },\n    \"SigningAlgorithm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SigningAlgorithm\"\n        },\n        {\n          \"description\": \"<p>Name of the algorithm your private CA uses to sign certificate requests.</p> <p>This parameter should not be confused with the <code>SigningAlgorithm</code> parameter used to sign certificates when they are issued.</p>\"\n        }\n      ]\n    },\n    \"Subject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ASN1Subject\"\n        },\n        {\n          \"description\": \"Structure that contains X.500 distinguished name information for your private CA.\"\
  \n        }\n      ]\n    },\n    \"CsrExtensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CsrExtensions\"\n        },\n        {\n          \"description\": \"Specifies information to be added to the extension section of the certificate signing request (CSR).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KeyAlgorithm\",\n    \"SigningAlgorithm\",\n    \"Subject\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-certificate-authority-configuration-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CertificateAuthorityConfiguration
---
