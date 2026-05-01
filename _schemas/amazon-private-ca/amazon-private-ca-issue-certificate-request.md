---
description: IssueCertificateRequest schema from Amazon Private CA API
layout: schema
name: IssueCertificateRequest
properties_list:
- description: ''
  name: ApiPassthrough
  type: object
- description: ''
  name: CertificateAuthorityArn
  type: object
- description: ''
  name: Csr
  type: object
- description: ''
  name: SigningAlgorithm
  type: object
- description: ''
  name: TemplateArn
  type: object
- description: ''
  name: Validity
  type: object
- description: ''
  name: ValidityNotBefore
  type: object
- description: ''
  name: IdempotencyToken
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-issue-certificate-request-schema.json
slug: amazon-private-ca-issue-certificate-request
source_filename: amazon-private-ca-issue-certificate-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-issue-certificate-request-schema.json\",\n  \"title\": \"IssueCertificateRequest\",\n  \"description\": \"IssueCertificateRequest schema from Amazon Private CA API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApiPassthrough\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApiPassthrough\"\n        },\n        {\n          \"description\": \"<p>Specifies X.509 certificate information to be included in the issued certificate. An <code>APIPassthrough</code> or <code>APICSRPassthrough</code> template variant must be selected, or else this parameter is ignored. For more information about using these templates, see <a href=\\\"https://docs.aws.amazon.com/privateca/latest/userguide/UsingTemplates.html\\\">Understanding Certificate Templates</a>.</p>\
  \ <p>If conflicting or duplicate certificate information is supplied during certificate issuance, Amazon Web Services Private CA applies <a href=\\\"https://docs.aws.amazon.com/privateca/latest/userguide/UsingTemplates.html#template-order-of-operations\\\">order of operation rules</a> to determine what information is used.</p>\"\n        }\n      ]\n    },\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) that was returned when you called <a href=\\\"https://docs.aws.amazon.com/privateca/latest/APIReference/API_CreateCertificateAuthority.html\\\">CreateCertificateAuthority</a>. This must be of the form:</p> <p> <code>arn:aws:acm-pca:<i>region</i>:<i>account</i>:certificate-authority/<i>12345678-1234-1234-1234-123456789012</i> </code> </p>\"\n        }\n      ]\n    },\n    \"Csr\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/CsrBlob\"\n        },\n        {\n          \"description\": \"<p>The certificate signing request (CSR) for the certificate you want to issue. As an example, you can use the following OpenSSL command to create the CSR and a 2048 bit RSA private key. </p> <p> <code>openssl req -new -newkey rsa:2048 -days 365 -keyout private/test_cert_priv_key.pem -out csr/test_cert_.csr</code> </p> <p>If you have a configuration file, you can then use the following OpenSSL command. The <code>usr_cert</code> block in the configuration file contains your X509 version 3 extensions. </p> <p> <code>openssl req -new -config openssl_rsa.cnf -extensions usr_cert -newkey rsa:2048 -days 365 -keyout private/test_cert_priv_key.pem -out csr/test_cert_.csr</code> </p> <p>Note: A CSR must provide either a <i>subject name</i> or a <i>subject alternative name</i> or the request will be rejected. </p>\"\n        }\n      ]\n    },\n    \"SigningAlgorithm\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/SigningAlgorithm\"\n        },\n        {\n          \"description\": \"<p>The name of the algorithm that will be used to sign the certificate to be issued. </p> <p>This parameter should not be confused with the <code>SigningAlgorithm</code> parameter used to sign a CSR in the <code>CreateCertificateAuthority</code> action.</p> <note> <p>The specified signing algorithm family (RSA or ECDSA) much match the algorithm family of the CA's secret key.</p> </note>\"\n        }\n      ]\n    },\n    \"TemplateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>Specifies a custom configuration template to use when issuing a certificate. If this parameter is not provided, Amazon Web Services Private CA defaults to the <code>EndEntityCertificate/V1</code> template. For CA certificates, you should choose the shortest path length that meets your needs. The path length\
  \ is indicated by the PathLen<i>N</i> portion of the ARN, where <i>N</i> is the <a href=\\\"https://docs.aws.amazon.com/privateca/latest/userguide/PcaTerms.html#terms-cadepth\\\">CA depth</a>.</p> <p>Note: The CA depth configured on a subordinate CA certificate must not exceed the limit set by its parents in the CA hierarchy.</p> <p>For a list of <code>TemplateArn</code> values supported by Amazon Web Services Private CA, see <a href=\\\"https://docs.aws.amazon.com/privateca/latest/userguide/UsingTemplates.html\\\">Understanding Certificate Templates</a>.</p>\"\n        }\n      ]\n    },\n    \"Validity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Validity\"\n        },\n        {\n          \"description\": \"<p>Information describing the end of the validity period of the certificate. This parameter sets the \\u201cNot After\\u201d date for the certificate.</p> <p>Certificate validity is the period of time during which a certificate is valid. Validity\
  \ can be expressed as an explicit date and time when the certificate expires, or as a span of time after issuance, stated in days, months, or years. For more information, see <a href=\\\"https://datatracker.ietf.org/doc/html/rfc5280#section-4.1.2.5\\\">Validity</a> in RFC 5280. </p> <p>This value is unaffected when <code>ValidityNotBefore</code> is also specified. For example, if <code>Validity</code> is set to 20 days in the future, the certificate will expire 20 days from issuance time regardless of the <code>ValidityNotBefore</code> value.</p> <p>The end of the validity period configured on a certificate must not exceed the limit set on its parents in the CA hierarchy.</p>\"\n        }\n      ]\n    },\n    \"ValidityNotBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Validity\"\n        },\n        {\n          \"description\": \"<p>Information describing the start of the validity period of the certificate. This parameter sets the \\u201cNot Before\\\
  \" date for the certificate.</p> <p>By default, when issuing a certificate, Amazon Web Services Private CA sets the \\\"Not Before\\\" date to the issuance time minus 60 minutes. This compensates for clock inconsistencies across computer systems. The <code>ValidityNotBefore</code> parameter can be used to customize the \\u201cNot Before\\u201d value. </p> <p>Unlike the <code>Validity</code> parameter, the <code>ValidityNotBefore</code> parameter is optional.</p> <p>The <code>ValidityNotBefore</code> value is expressed as an explicit date and time, using the <code>Validity</code> type value <code>ABSOLUTE</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/acm-pca/latest/APIReference/API_Validity.html\\\">Validity</a> in this API reference and <a href=\\\"https://datatracker.ietf.org/doc/html/rfc5280#section-4.1.2.5\\\">Validity</a> in RFC 5280.</p>\"\n        }\n      ]\n    },\n    \"IdempotencyToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\
  \n        },\n        {\n          \"description\": \"Alphanumeric string that can be used to distinguish between calls to the <b>IssueCertificate</b> action. Idempotency tokens for <b>IssueCertificate</b> time out after one minute. Therefore, if you call <b>IssueCertificate</b> multiple times with the same idempotency token within one minute, Amazon Web Services Private CA recognizes that you are requesting only one certificate and will issue only one. If you change the idempotency token for each call, Amazon Web Services Private CA recognizes that you are requesting multiple certificates.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateAuthorityArn\",\n    \"Csr\",\n    \"SigningAlgorithm\",\n    \"Validity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-issue-certificate-request-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: IssueCertificateRequest
---
