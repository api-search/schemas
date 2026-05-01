---
description: Contains information about the certificate subject. The <code>Subject</code> field in the certificate identifies the entity that owns or controls the public key in the certificate. The entity can be a user, computer, device, or service. The <code>Subject </code>must contain an X.500 distinguished name (DN). A DN is a sequence of relative distinguished names (RDNs). The RDNs are separated by commas in the certificate.
layout: schema
name: ASN1Subject
properties_list:
- description: ''
  name: Country
  type: object
- description: ''
  name: Organization
  type: object
- description: ''
  name: OrganizationalUnit
  type: object
- description: ''
  name: DistinguishedNameQualifier
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: CommonName
  type: object
- description: ''
  name: SerialNumber
  type: object
- description: ''
  name: Locality
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Surname
  type: object
- description: ''
  name: GivenName
  type: object
- description: ''
  name: Initials
  type: object
- description: ''
  name: Pseudonym
  type: object
- description: ''
  name: GenerationQualifier
  type: object
- description: ''
  name: CustomAttributes
  type: object
provider_name: Amazon Private CA
provider_slug: amazon-private-ca
schema_file: json-schema/amazon-private-ca-asn1subject-schema.json
slug: amazon-private-ca-asn1subject
source_filename: amazon-private-ca-asn1subject-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-asn1subject-schema.json\",\n  \"title\": \"ASN1Subject\",\n  \"description\": \"Contains information about the certificate subject. The <code>Subject</code> field in the certificate identifies the entity that owns or controls the public key in the certificate. The entity can be a user, computer, device, or service. The <code>Subject </code>must contain an X.500 distinguished name (DN). A DN is a sequence of relative distinguished names (RDNs). The RDNs are separated by commas in the certificate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountryCodeString\"\n        },\n        {\n          \"description\": \"Two-digit code that specifies the country in which the certificate subject\
  \ located.\"\n        }\n      ]\n    },\n    \"Organization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String64\"\n        },\n        {\n          \"description\": \"Legal name of the organization with which the certificate subject is affiliated. \"\n        }\n      ]\n    },\n    \"OrganizationalUnit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String64\"\n        },\n        {\n          \"description\": \"A subdivision or unit of the organization (such as sales or finance) with which the certificate subject is affiliated.\"\n        }\n      ]\n    },\n    \"DistinguishedNameQualifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ASN1PrintableString64\"\n        },\n        {\n          \"description\": \"Disambiguating information for the certificate subject.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String128\"\
  \n        },\n        {\n          \"description\": \"State in which the subject of the certificate is located.\"\n        }\n      ]\n    },\n    \"CommonName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String64\"\n        },\n        {\n          \"description\": \"<p>For CA and end-entity certificates in a private PKI, the common name (CN) can be any string within the length limit. </p> <p>Note: In publicly trusted certificates, the common name must be a fully qualified domain name (FQDN) associated with the certificate subject.</p>\"\n        }\n      ]\n    },\n    \"SerialNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ASN1PrintableString64\"\n        },\n        {\n          \"description\": \"The certificate serial number.\"\n        }\n      ]\n    },\n    \"Locality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String128\"\n        },\n        {\n          \"description\"\
  : \"The locality (such as a city or town) in which the certificate subject is located.\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String64\"\n        },\n        {\n          \"description\": \"A title such as Mr. or Ms., which is pre-pended to the name to refer formally to the certificate subject.\"\n        }\n      ]\n    },\n    \"Surname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String40\"\n        },\n        {\n          \"description\": \"Family name. In the US and the UK, for example, the surname of an individual is ordered last. In Asian cultures the surname is typically ordered first.\"\n        }\n      ]\n    },\n    \"GivenName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String16\"\n        },\n        {\n          \"description\": \"First name.\"\n        }\n      ]\n    },\n    \"Initials\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/String5\"\n        },\n        {\n          \"description\": \"Concatenation that typically contains the first letter of the <b>GivenName</b>, the first letter of the middle name if one exists, and the first letter of the <b>Surname</b>.\"\n        }\n      ]\n    },\n    \"Pseudonym\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String128\"\n        },\n        {\n          \"description\": \"Typically a shortened version of a longer <b>GivenName</b>. For example, Jonathan is often shortened to John. Elizabeth is often shortened to Beth, Liz, or Eliza.\"\n        }\n      ]\n    },\n    \"GenerationQualifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String3\"\n        },\n        {\n          \"description\": \"Typically a qualifier appended to the name of an individual. Examples include Jr. for junior, Sr. for senior, and III for third.\"\n        }\n      ]\n  \
  \  },\n    \"CustomAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomAttributeList\"\n        },\n        {\n          \"description\": \"<p/> <p>Contains a sequence of one or more X.500 relative distinguished names (RDNs), each of which consists of an object identifier (OID) and a value. For more information, see NIST\\u2019s definition of <a href=\\\"https://csrc.nist.gov/glossary/term/Object_Identifier\\\">Object Identifier (OID)</a>.</p> <note> <p>Custom attributes cannot be used in combination with standard attributes.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-private-ca/refs/heads/main/json-schema/amazon-private-ca-asn1subject-schema.json
tags:
- Certificate Authority
- Certificates
- PKI
- Security
- X.509
- TLS
- IoT
title: ASN1Subject
---
