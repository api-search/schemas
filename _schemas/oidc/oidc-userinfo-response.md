---
description: Schema describing the response from the OpenID Connect UserInfo endpoint as defined in OIDC Core 1.0. The UserInfo endpoint returns claims about the authenticated end-user. The claims returned depend on the scopes requested and granted during the authorization flow (profile, email, address, phone).
layout: schema
name: OpenID Connect UserInfo Response
properties_list:
- description: Subject Identifier. A locally unique and never reassigned identifier for the end-user at the issuer. This is the only required claim in the UserInfo response.
  name: sub
  type: string
- description: Full name of the end-user in displayable form, including all name parts and possibly titles and suffixes. Requires 'profile' scope.
  name: name
  type: string
- description: Given name(s) or first name(s) of the end-user. Requires 'profile' scope.
  name: given_name
  type: string
- description: Surname(s) or last name(s) of the end-user. Requires 'profile' scope.
  name: family_name
  type: string
- description: Middle name(s) of the end-user. Requires 'profile' scope.
  name: middle_name
  type: string
- description: Casual name of the end-user that may or may not be the same as the given_name. Requires 'profile' scope.
  name: nickname
  type: string
- description: Shorthand name by which the end-user wishes to be referred to at the relying party. Requires 'profile' scope.
  name: preferred_username
  type: string
- description: URL of the end-user's profile page. Requires 'profile' scope.
  name: profile
  type: string
- description: URL of the end-user's profile picture. This URL must refer to an image file rather than a web page containing an image. Requires 'profile' scope.
  name: picture
  type: string
- description: URL of the end-user's web page or blog. Requires 'profile' scope.
  name: website
  type: string
- description: End-user's preferred email address. Its value must conform to RFC 5322 addr-spec syntax. Requires 'email' scope.
  name: email
  type: string
- description: Whether the end-user's email address has been verified by the provider. Requires 'email' scope.
  name: email_verified
  type: boolean
- description: End-user's gender. Values defined by the specification include 'female' and 'male', but other values may be used. Requires 'profile' scope.
  name: gender
  type: string
- description: End-user's birthday in ISO 8601 YYYY-MM-DD format. A year value of 0000 indicates the year was omitted. Requires 'profile' scope.
  name: birthdate
  type: string
- description: End-user's time zone as a string from the IANA Time Zone Database. Requires 'profile' scope.
  name: zoneinfo
  type: string
- description: End-user's locale represented as a BCP 47 language tag. Typically an ISO 639-1 language code and an ISO 3166-1 country code. Requires 'profile' scope.
  name: locale
  type: string
- description: End-user's preferred telephone number in E.164 format. Requires 'phone' scope.
  name: phone_number
  type: string
- description: Whether the end-user's phone number has been verified by the provider. Requires 'phone' scope.
  name: phone_number_verified
  type: boolean
- description: End-user's preferred postal address. Requires 'address' scope.
  name: address
  type: object
- description: Time the end-user's information was last updated. Represented as the number of seconds since the Unix epoch (1970-01-01T00:00:00Z).
  name: updated_at
  type: integer
provider_name: OIDC
provider_slug: oidc
schema_file: json-schema/oidc-userinfo-response.json
slug: oidc-userinfo-response
source_filename: oidc-userinfo-response.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"oidc-userinfo-response.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenID Connect UserInfo Response\",\n  \"description\": \"Schema describing the response from the OpenID Connect UserInfo endpoint as defined in OIDC Core 1.0. The UserInfo endpoint returns claims about the authenticated end-user. The claims returned depend on the scopes requested and granted during the authorization flow (profile, email, address, phone).\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sub\"\n  ],\n  \"properties\": {\n    \"sub\": {\n      \"type\": \"string\",\n      \"description\": \"Subject Identifier. A locally unique and never reassigned identifier for the end-user at the issuer. This is the only required claim in the UserInfo response.\",\n      \"maxLength\": 255\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the end-user in displayable form, including all name parts and\
  \ possibly titles and suffixes. Requires 'profile' scope.\"\n    },\n    \"given_name\": {\n      \"type\": \"string\",\n      \"description\": \"Given name(s) or first name(s) of the end-user. Requires 'profile' scope.\"\n    },\n    \"family_name\": {\n      \"type\": \"string\",\n      \"description\": \"Surname(s) or last name(s) of the end-user. Requires 'profile' scope.\"\n    },\n    \"middle_name\": {\n      \"type\": \"string\",\n      \"description\": \"Middle name(s) of the end-user. Requires 'profile' scope.\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n      \"description\": \"Casual name of the end-user that may or may not be the same as the given_name. Requires 'profile' scope.\"\n    },\n    \"preferred_username\": {\n      \"type\": \"string\",\n      \"description\": \"Shorthand name by which the end-user wishes to be referred to at the relying party. Requires 'profile' scope.\"\n    },\n    \"profile\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"uri\",\n      \"description\": \"URL of the end-user's profile page. Requires 'profile' scope.\"\n    },\n    \"picture\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the end-user's profile picture. This URL must refer to an image file rather than a web page containing an image. Requires 'profile' scope.\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the end-user's web page or blog. Requires 'profile' scope.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"End-user's preferred email address. Its value must conform to RFC 5322 addr-spec syntax. Requires 'email' scope.\"\n    },\n    \"email_verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the end-user's email address has been verified by the provider. Requires 'email' scope.\"\n    },\n    \"gender\": {\n      \"type\": \"\
  string\",\n      \"description\": \"End-user's gender. Values defined by the specification include 'female' and 'male', but other values may be used. Requires 'profile' scope.\"\n    },\n    \"birthdate\": {\n      \"type\": \"string\",\n      \"description\": \"End-user's birthday in ISO 8601 YYYY-MM-DD format. A year value of 0000 indicates the year was omitted. Requires 'profile' scope.\",\n      \"pattern\": \"^\\\\d{4}-\\\\d{2}-\\\\d{2}$\"\n    },\n    \"zoneinfo\": {\n      \"type\": \"string\",\n      \"description\": \"End-user's time zone as a string from the IANA Time Zone Database. Requires 'profile' scope.\",\n      \"examples\": [\"America/Los_Angeles\", \"Europe/Paris\"]\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"End-user's locale represented as a BCP 47 language tag. Typically an ISO 639-1 language code and an ISO 3166-1 country code. Requires 'profile' scope.\",\n      \"examples\": [\"en-US\", \"fr-FR\"]\n    },\n    \"phone_number\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"End-user's preferred telephone number in E.164 format. Requires 'phone' scope.\",\n      \"examples\": [\"+1-555-555-1234\"]\n    },\n    \"phone_number_verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the end-user's phone number has been verified by the provider. Requires 'phone' scope.\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"End-user's preferred postal address. Requires 'address' scope.\",\n      \"properties\": {\n        \"formatted\": {\n          \"type\": \"string\",\n          \"description\": \"Full mailing address formatted for display or use on a mailing label.\"\n        },\n        \"street_address\": {\n          \"type\": \"string\",\n          \"description\": \"Full street address component, which may include house number, street name, PO box, and multi-line information.\"\n        },\n        \"locality\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"City or locality component.\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"State, province, prefecture, or region component.\"\n        },\n        \"postal_code\": {\n          \"type\": \"string\",\n          \"description\": \"Zip code or postal code component.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country name component.\"\n        }\n      }\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Time the end-user's information was last updated. Represented as the number of seconds since the Unix epoch (1970-01-01T00:00:00Z).\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/json-schema/oidc-userinfo-response.json
tags:
- Authentication
- Identity
- JWT
- OAuth
- OIDC
- OpenID Connect
title: OpenID Connect UserInfo Response
---
