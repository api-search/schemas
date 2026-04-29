---
description: Certificate revocation information used by the <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html">CreateCertificateAuthority</a> and <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_UpdateCertificateAuthority.html">UpdateCertificateAuthority</a> actions. Your private certificate authority (CA) can configure Online Certificate Status Protocol (OCSP) support and/or maintain a certificate revocation list (CRL). OCSP returns validation information about certificates as requested by clients, and a CRL contains an updated list of certificates revoked by your CA. For more information, see <a href="https://docs.aws.amazon.com/privateca/latest/APIReference/API_RevokeCertificate.html">RevokeCertificate</a> and <a href="https://docs.aws.amazon.com/privateca/latest/userguide/revocation-setup.html">Setting up a certificate revocation method</a> in the <i>Amazon Web Services Private Certificate Authority User Guide</i>.
layout: schema
name: RevocationConfiguration
properties_list:
- description: ''
  name: CrlConfiguration
  type: object
- description: ''
  name: OcspConfiguration
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-revocation-configuration-schema.json
slug: amazon-private-ca-revocation-configuration
source_filename: amazon-private-ca-revocation-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-revocation-configuration-schema.json\",\n  \"title\": \"RevocationConfiguration\",\n  \"description\": \"Certificate revocation information used by the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html\\\">CreateCertificateAuthority</a> and <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_UpdateCertificateAuthority.html\\\">UpdateCertificateAuthority</a> actions. Your private certificate authority (CA) can configure Online Certificate Status Protocol (OCSP) support and/or maintain a certificate revocation list (CRL). OCSP returns validation information about certificates as requested by clients, and a CRL contains an updated list of certificates revoked by your CA. For more information, see <a href=\\\"\
  https://docs.aws.amazon.com/privateca/latest/APIReference/API_RevokeCertificate.html\\\">RevokeCertificate</a> and <a href=\\\"https://docs.aws.amazon.com/privateca/latest/userguide/revocation-setup.html\\\">Setting up a certificate revocation method</a> in the <i>Amazon Web Services Private Certificate Authority User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CrlConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CrlConfiguration\"\n        },\n        {\n          \"description\": \"Configuration of the certificate revocation list (CRL), if any, maintained by your private CA. A CRL is typically updated approximately 30 minutes after a certificate is revoked. If for any reason a CRL update fails, Amazon Web Services Private CA makes further attempts every 15 minutes.\"\n        }\n      ]\n    },\n    \"OcspConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OcspConfiguration\"\n\
  \        },\n        {\n          \"description\": \"Configuration of Online Certificate Status Protocol (OCSP) support, if any, maintained by your private CA. When you revoke a certificate, OCSP responses may take up to 60 minutes to reflect the new status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-revocation-configuration-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: RevocationConfiguration
---
