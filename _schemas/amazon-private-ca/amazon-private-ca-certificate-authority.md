---
description: Contains information about your private certificate authority (CA). Your private CA can issue and revoke X.509 digital certificates. Digital certificates verify that the entity named in the certificate <b>Subject</b> field owns or controls the public key contained in the <b>Subject Public Key Info</b> field. Call the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html">CreateCertificateAuthority</a> action to create your private CA. You must then call the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_GetCertificateAuthorityCertificate.html">GetCertificateAuthorityCertificate</a> action to retrieve a private CA certificate signing request (CSR). Sign the CSR with your Amazon Web Services Private CA-hosted or on-premises root or subordinate CA certificate. Call the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_ImportCertificateAuthorityCertificate.html">ImportCertificateAuthorityCertificate</a>
  action to import the signed certificate into Certificate Manager (ACM).
layout: schema
name: CertificateAuthority
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: OwnerAccount
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: LastStateChangeAt
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Serial
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: NotBefore
  type: object
- description: ''
  name: NotAfter
  type: object
- description: ''
  name: FailureReason
  type: object
- description: ''
  name: CertificateAuthorityConfiguration
  type: object
- description: ''
  name: RevocationConfiguration
  type: object
- description: ''
  name: RestorableUntil
  type: object
- description: ''
  name: KeyStorageSecurityStandard
  type: object
- description: ''
  name: UsageMode
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-certificate-authority-schema.json
slug: amazon-private-ca-certificate-authority
source_filename: amazon-private-ca-certificate-authority-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-certificate-authority-schema.json\",\n  \"title\": \"CertificateAuthority\",\n  \"description\": \"Contains information about your private certificate authority (CA). Your private CA can issue and revoke X.509 digital certificates. Digital certificates verify that the entity named in the certificate <b>Subject</b> field owns or controls the public key contained in the <b>Subject Public Key Info</b> field. Call the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html\\\">CreateCertificateAuthority</a> action to create your private CA. You must then call the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_GetCertificateAuthorityCertificate.html\\\">GetCertificateAuthorityCertificate</a> action to retrieve a\
  \ private CA certificate signing request (CSR). Sign the CSR with your Amazon Web Services Private CA-hosted or on-premises root or subordinate CA certificate. Call the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_ImportCertificateAuthorityCertificate.html\\\">ImportCertificateAuthorityCertificate</a> action to import the signed certificate into Certificate Manager (ACM). \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) for your private certificate authority (CA). The format is <code> <i>12345678-1234-1234-1234-123456789012</i> </code>.\"\n        }\n      ]\n    },\n    \"OwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID that owns the certificate\
  \ authority.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"Date and time at which your private CA was created.\"\n        }\n      ]\n    },\n    \"LastStateChangeAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"Date and time at which your private CA was last updated.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityType\"\n        },\n        {\n          \"description\": \"Type of your private CA.\"\n        }\n      ]\n    },\n    \"Serial\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Serial number of your private CA.\"\n        }\n      ]\n    },\n    \"Status\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityStatus\"\n        },\n        {\n          \"description\": \"Status of your private CA.\"\n        }\n      ]\n    },\n    \"NotBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"Date and time before which your private CA certificate is not valid.\"\n        }\n      ]\n    },\n    \"NotAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"Date and time after which your private CA certificate is not valid.\"\n        }\n      ]\n    },\n    \"FailureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureReason\"\n        },\n        {\n          \"description\": \"Reason the request to create your private CA failed.\"\n        }\n      ]\n    },\n    \"CertificateAuthorityConfiguration\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityConfiguration\"\n        },\n        {\n          \"description\": \"Your private CA configuration.\"\n        }\n      ]\n    },\n    \"RevocationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevocationConfiguration\"\n        },\n        {\n          \"description\": \"Information about the Online Certificate Status Protocol (OCSP) configuration or certificate revocation list (CRL) created and maintained by your private CA. \"\n        }\n      ]\n    },\n    \"RestorableUntil\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The period during which a deleted CA can be restored. For more information, see the <code>PermanentDeletionTimeInDays</code> parameter of the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_DeleteCertificateAuthorityRequest.html\\\
  \">DeleteCertificateAuthorityRequest</a> action. \"\n        }\n      ]\n    },\n    \"KeyStorageSecurityStandard\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyStorageSecurityStandard\"\n        },\n        {\n          \"description\": \"<p>Defines a cryptographic key management compliance standard used for handling CA keys. </p> <p>Default: FIPS_140_2_LEVEL_3_OR_HIGHER</p> <p>Note: Amazon Web Services Region ap-northeast-3 supports only FIPS_140_2_LEVEL_2_OR_HIGHER. You must explicitly specify this parameter and value when creating a CA in that Region. Specifying a different value (or no value) results in an <code>InvalidArgsException</code> with the message \\\"A certificate authority cannot be created in this region with the specified security standard.\\\"</p>\"\n        }\n      ]\n    },\n    \"UsageMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityUsageMode\"\n        },\n        {\n   \
  \       \"description\": \"<p>Specifies whether the CA issues general-purpose certificates that typically require a revocation mechanism, or short-lived certificates that may optionally omit revocation because they expire quickly. Short-lived certificate validity is limited to seven days.</p> <p>The default value is GENERAL_PURPOSE.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-certificate-authority-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CertificateAuthority
---
