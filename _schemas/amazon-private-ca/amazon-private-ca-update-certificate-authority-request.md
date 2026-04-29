---
description: UpdateCertificateAuthorityRequest schema from Amazon Private CA API
layout: schema
name: UpdateCertificateAuthorityRequest
properties_list:
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: RevocationConfiguration
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-update-certificate-authority-request-schema.json
slug: amazon-private-ca-update-certificate-authority-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-update-certificate-authority-request-schema.json\",\n  \"title\": \"UpdateCertificateAuthorityRequest\",\n  \"description\": \"UpdateCertificateAuthorityRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>Amazon Resource Name (ARN) of the private CA that issued the certificate to be revoked. This must be of the form:</p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i> </code> </p>\"\n        }\n      ]\n    },\n    \"RevocationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevocationConfiguration\"\
  \n        },\n        {\n          \"description\": \"<p>Contains information to enable Online Certificate Status Protocol (OCSP) support, to enable a certificate revocation list (CRL), to enable both, or to enable neither. If this parameter is not supplied, existing capibilites remain unchanged. For more information, see the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_OcspConfiguration.html\\\">OcspConfiguration</a> and <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CrlConfiguration.html\\\">CrlConfiguration</a> types.</p> <note> <p>The following requirements apply to revocation configurations.</p> <ul> <li> <p>A configuration disabling CRLs or OCSP must contain only the <code>Enabled=False</code> parameter, and will fail if other parameters such as <code>CustomCname</code> or <code>ExpirationInDays</code> are included.</p> </li> <li> <p>In a CRL configuration, the <code>S3BucketName</code> parameter must conform to <a href=\\\"\
  https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html\\\">Amazon S3 bucket naming rules</a>.</p> </li> <li> <p>A configuration containing a custom Canonical Name (CNAME) parameter for CRLs or OCSP must conform to <a href=\\\"https://www.ietf.org/rfc/rfc2396.txt\\\">RFC2396</a> restrictions on the use of special characters in a CNAME. </p> </li> <li> <p>In a CRL or OCSP configuration, the value of a CNAME parameter must not include a protocol prefix such as \\\"http://\\\" or \\\"https://\\\".</p> </li> </ul> </note>\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityStatus\"\n        },\n        {\n          \"description\": \"Status of your private CA.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-update-certificate-authority-request-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: UpdateCertificateAuthorityRequest
---
