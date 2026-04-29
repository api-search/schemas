---
description: CreateCertificateAuthorityRequest schema from Amazon Private CA API
layout: schema
name: CreateCertificateAuthorityRequest
properties_list:
- description: ''
  name: CertificateAuthorityConfiguration
  type: object
- description: ''
  name: RevocationConfiguration
  type: object
- description: ''
  name: CertificateAuthorityType
  type: object
- description: ''
  name: IdempotencyToken
  type: object
- description: ''
  name: KeyStorageSecurityStandard
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: UsageMode
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-create-certificate-authority-request-schema.json
slug: amazon-private-ca-create-certificate-authority-request
source_filename: amazon-private-ca-create-certificate-authority-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-certificate-authority-request-schema.json\",\n  \"title\": \"CreateCertificateAuthorityRequest\",\n  \"description\": \"CreateCertificateAuthorityRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityConfiguration\"\n        },\n        {\n          \"description\": \"Name and bit size of the private key algorithm, the name of the signing algorithm, and X.500 certificate subject information.\"\n        }\n      ]\n    },\n    \"RevocationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevocationConfiguration\"\n        },\n        {\n          \"description\"\
  : \"<p>Contains information to enable Online Certificate Status Protocol (OCSP) support, to enable a certificate revocation list (CRL), to enable both, or to enable neither. The default is for both certificate validation mechanisms to be disabled. </p> <note> <p>The following requirements apply to revocation configurations.</p> <ul> <li> <p>A configuration disabling CRLs or OCSP must contain only the <code>Enabled=False</code> parameter, and will fail if other parameters such as <code>CustomCname</code> or <code>ExpirationInDays</code> are included.</p> </li> <li> <p>In a CRL configuration, the <code>S3BucketName</code> parameter must conform to <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html\\\">Amazon S3 bucket naming rules</a>.</p> </li> <li> <p>A configuration containing a custom Canonical Name (CNAME) parameter for CRLs or OCSP must conform to <a href=\\\"https://www.ietf.org/rfc/rfc2396.txt\\\">RFC2396</a> restrictions on the use of special\
  \ characters in a CNAME. </p> </li> <li> <p>In a CRL or OCSP configuration, the value of a CNAME parameter must not include a protocol prefix such as \\\"http://\\\" or \\\"https://\\\".</p> </li> </ul> </note> <p> For more information, see the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_OcspConfiguration.html\\\">OcspConfiguration</a> and <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CrlConfiguration.html\\\">CrlConfiguration</a> types.</p>\"\n        }\n      ]\n    },\n    \"CertificateAuthorityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityType\"\n        },\n        {\n          \"description\": \"The type of the certificate authority.\"\n        }\n      ]\n    },\n    \"IdempotencyToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"Custom string that can be used\
  \ to distinguish between calls to the <b>CreateCertificateAuthority</b> action. Idempotency tokens for <b>CreateCertificateAuthority</b> time out after five minutes. Therefore, if you call <b>CreateCertificateAuthority</b> multiple times with the same idempotency token within five minutes, Amazon Web Services Private CA recognizes that you are requesting only certificate authority and will issue only one. If you change the idempotency token for each call, Amazon Web Services Private CA recognizes that you are requesting multiple certificate authorities.\"\n        }\n      ]\n    },\n    \"KeyStorageSecurityStandard\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyStorageSecurityStandard\"\n        },\n        {\n          \"description\": \"<p>Specifies a cryptographic key management compliance standard used for handling CA keys.</p> <p>Default: FIPS_140_2_LEVEL_3_OR_HIGHER</p> <p> <i>Note:</i> <code>FIPS_140_2_LEVEL_3_OR_HIGHER</code> is not supported\
  \ in the following Regions:</p> <ul> <li> <p>ap-northeast-3</p> </li> <li> <p>ap-southeast-3</p> </li> </ul> <p>When creating a CA in these Regions, you must provide <code>FIPS_140_2_LEVEL_2_OR_HIGHER</code> as the argument for <code>KeyStorageSecurityStandard</code>. Failure to do this results in an <code>InvalidArgsException</code> with the message, \\\"A certificate authority cannot be created in this region with the specified security standard.\\\"</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Key-value pairs that will be attached to the new private CA. You can associate up to 50 tags with a private CA. For information using tags with IAM to manage permissions, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_iam-tags.html\\\">Controlling Access Using IAM Tags</a>.\"\n        }\n      ]\n    },\n    \"UsageMode\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityUsageMode\"\n        },\n        {\n          \"description\": \"<p>Specifies whether the CA issues general-purpose certificates that typically require a revocation mechanism, or short-lived certificates that may optionally omit revocation because they expire quickly. Short-lived certificate validity is limited to seven days.</p> <p>The default value is GENERAL_PURPOSE.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityConfiguration\",\n    \"CertificateAuthorityType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-create-certificate-authority-request-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: CreateCertificateAuthorityRequest
---
