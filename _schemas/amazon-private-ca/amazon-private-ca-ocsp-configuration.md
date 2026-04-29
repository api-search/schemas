---
description: <p>Contains information to enable and configure Online Certificate Status Protocol (OCSP) for validating certificate revocation status.</p> <p>When you revoke a certificate, OCSP responses may take up to 60 minutes to reflect the new status.</p>
layout: schema
name: OcspConfiguration
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: OcspCustomCname
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-ocsp-configuration-schema.json
slug: amazon-private-ca-ocsp-configuration
source_filename: amazon-private-ca-ocsp-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-ocsp-configuration-schema.json\",\n  \"title\": \"OcspConfiguration\",\n  \"description\": \"<p>Contains information to enable and configure Online Certificate Status Protocol (OCSP) for validating certificate revocation status.</p> <p>When you revoke a certificate, OCSP responses may take up to 60 minutes to reflect the new status.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Flag enabling use of the Online Certificate Status Protocol (OCSP) for validating certificate revocation status.\"\n        }\n      ]\n    },\n    \"OcspCustomCname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CnameString\"\
  \n        },\n        {\n          \"description\": \"<p>By default, Amazon Web Services Private CA injects an Amazon Web Services domain into certificates being validated by the Online Certificate Status Protocol (OCSP). A customer can alternatively use this object to define a CNAME specifying a customized OCSP domain.</p> <note> <p>The content of a Canonical Name (CNAME) record must conform to <a href=\\\"https://www.ietf.org/rfc/rfc2396.txt\\\">RFC2396</a> restrictions on the use of special characters in URIs. Additionally, the value of the CNAME must not include a protocol prefix such as \\\"http://\\\" or \\\"https://\\\".</p> </note> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/privateca/latest/userguide/ocsp-customize.html\\\">Customizing Online Certificate Status Protocol (OCSP) </a> in the <i>Amazon Web Services Private Certificate Authority User Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-ocsp-configuration-schema.json
tags:
- AWS
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: OcspConfiguration
---
