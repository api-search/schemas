---
description: Schema describing the claims contained in an OpenID Connect ID Token as defined in the OIDC Core 1.0 specification. The ID Token is a JSON Web Token (JWT) that contains claims about the authentication event and the end-user. It is the primary artifact that distinguishes OIDC from plain OAuth 2.0.
layout: schema
name: OpenID Connect ID Token Claims
properties_list:
- description: Issuer Identifier for the issuer of the response. Must be the HTTPS URL of the OpenID Provider.
  name: iss
  type: string
- description: Subject Identifier. A locally unique and never reassigned identifier for the end-user within the issuer, intended to be consumed by the client.
  name: sub
  type: string
- description: Audience(s) that this ID Token is intended for. Must contain the OAuth 2.0 client_id of the relying party.
  name: aud
  type: object
- description: Expiration time on or after which the ID Token must not be accepted for processing. Represented as seconds since the Unix epoch.
  name: exp
  type: integer
- description: Time at which the JWT was issued. Represented as seconds since the Unix epoch.
  name: iat
  type: integer
- description: Time when the end-user authentication occurred. Required when a max_age request is made or when auth_time is requested as an essential claim.
  name: auth_time
  type: integer
- description: A string value used to associate a client session with an ID Token and to mitigate replay attacks. The value is passed through unmodified from the authentication request.
  name: nonce
  type: string
- description: Authentication Context Class Reference. A string specifying the authentication context class that the authentication performed satisfied.
  name: acr
  type: string
- description: Authentication Methods References. JSON array of strings that are identifiers for authentication methods used in the authentication.
  name: amr
  type: array
- description: Authorized Party. The client_id of the party to which the ID Token was issued. Required when the ID Token has a single audience value that differs from the authorized party.
  name: azp
  type: string
- description: Access Token hash value. Provides validation that the access token is tied to the ID Token.
  name: at_hash
  type: string
- description: Code hash value. Provides validation that the authorization code is tied to the ID Token.
  name: c_hash
  type: string
- description: State hash value. Provides validation that the state parameter is tied to the ID Token.
  name: s_hash
  type: string
- description: Full name of the end-user in displayable form.
  name: name
  type: string
- description: Given name(s) or first name(s) of the end-user.
  name: given_name
  type: string
- description: Surname(s) or last name(s) of the end-user.
  name: family_name
  type: string
- description: Middle name(s) of the end-user.
  name: middle_name
  type: string
- description: Casual name of the end-user.
  name: nickname
  type: string
- description: Shorthand name by which the end-user wishes to be referred to.
  name: preferred_username
  type: string
- description: URL of the end-user's profile page.
  name: profile
  type: string
- description: URL of the end-user's profile picture.
  name: picture
  type: string
- description: URL of the end-user's web page or blog.
  name: website
  type: string
- description: End-user's preferred email address.
  name: email
  type: string
- description: Whether the end-user's email address has been verified.
  name: email_verified
  type: boolean
- description: End-user's gender.
  name: gender
  type: string
- description: End-user's birthday in ISO 8601 YYYY-MM-DD format. The year may be 0000 to indicate it was omitted.
  name: birthdate
  type: string
- description: End-user's time zone from the IANA Time Zone Database.
  name: zoneinfo
  type: string
- description: End-user's locale as a BCP 47 language tag.
  name: locale
  type: string
- description: End-user's preferred telephone number in E.164 format.
  name: phone_number
  type: string
- description: Whether the end-user's phone number has been verified.
  name: phone_number_verified
  type: boolean
- description: End-user's preferred postal address.
  name: address
  type: object
- description: Time the end-user's information was last updated. Represented as seconds since the Unix epoch.
  name: updated_at
  type: integer
provider_name: OIDC
provider_slug: oidc
schema_file: json-schema/oidc-id-token.json
slug: oidc-id-token
source_filename: oidc-id-token.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"oidc-id-token.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenID Connect ID Token Claims\",\n  \"description\": \"Schema describing the claims contained in an OpenID Connect ID Token as defined in the OIDC Core 1.0 specification. The ID Token is a JSON Web Token (JWT) that contains claims about the authentication event and the end-user. It is the primary artifact that distinguishes OIDC from plain OAuth 2.0.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"iss\",\n    \"sub\",\n    \"aud\",\n    \"exp\",\n    \"iat\"\n  ],\n  \"properties\": {\n    \"iss\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Issuer Identifier for the issuer of the response. Must be the HTTPS URL of the OpenID Provider.\"\n    },\n    \"sub\": {\n      \"type\": \"string\",\n      \"description\": \"Subject Identifier. A locally unique and never reassigned identifier for the end-user within the\
  \ issuer, intended to be consumed by the client.\",\n      \"maxLength\": 255\n    },\n    \"aud\": {\n      \"description\": \"Audience(s) that this ID Token is intended for. Must contain the OAuth 2.0 client_id of the relying party.\",\n      \"oneOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      ]\n    },\n    \"exp\": {\n      \"type\": \"integer\",\n      \"description\": \"Expiration time on or after which the ID Token must not be accepted for processing. Represented as seconds since the Unix epoch.\"\n    },\n    \"iat\": {\n      \"type\": \"integer\",\n      \"description\": \"Time at which the JWT was issued. Represented as seconds since the Unix epoch.\"\n    },\n    \"auth_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Time when the end-user authentication occurred. Required when a max_age request is made or when\
  \ auth_time is requested as an essential claim.\"\n    },\n    \"nonce\": {\n      \"type\": \"string\",\n      \"description\": \"A string value used to associate a client session with an ID Token and to mitigate replay attacks. The value is passed through unmodified from the authentication request.\"\n    },\n    \"acr\": {\n      \"type\": \"string\",\n      \"description\": \"Authentication Context Class Reference. A string specifying the authentication context class that the authentication performed satisfied.\"\n    },\n    \"amr\": {\n      \"type\": \"array\",\n      \"description\": \"Authentication Methods References. JSON array of strings that are identifiers for authentication methods used in the authentication.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"azp\": {\n      \"type\": \"string\",\n      \"description\": \"Authorized Party. The client_id of the party to which the ID Token was issued. Required when the ID Token has a single audience\
  \ value that differs from the authorized party.\"\n    },\n    \"at_hash\": {\n      \"type\": \"string\",\n      \"description\": \"Access Token hash value. Provides validation that the access token is tied to the ID Token.\"\n    },\n    \"c_hash\": {\n      \"type\": \"string\",\n      \"description\": \"Code hash value. Provides validation that the authorization code is tied to the ID Token.\"\n    },\n    \"s_hash\": {\n      \"type\": \"string\",\n      \"description\": \"State hash value. Provides validation that the state parameter is tied to the ID Token.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the end-user in displayable form.\"\n    },\n    \"given_name\": {\n      \"type\": \"string\",\n      \"description\": \"Given name(s) or first name(s) of the end-user.\"\n    },\n    \"family_name\": {\n      \"type\": \"string\",\n      \"description\": \"Surname(s) or last name(s) of the end-user.\"\n    },\n    \"middle_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Middle name(s) of the end-user.\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n      \"description\": \"Casual name of the end-user.\"\n    },\n    \"preferred_username\": {\n      \"type\": \"string\",\n      \"description\": \"Shorthand name by which the end-user wishes to be referred to.\"\n    },\n    \"profile\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the end-user's profile page.\"\n    },\n    \"picture\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the end-user's profile picture.\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the end-user's web page or blog.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"End-user's preferred email address.\"\n    },\n    \"email_verified\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the end-user's email address has been verified.\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"description\": \"End-user's gender.\"\n    },\n    \"birthdate\": {\n      \"type\": \"string\",\n      \"description\": \"End-user's birthday in ISO 8601 YYYY-MM-DD format. The year may be 0000 to indicate it was omitted.\",\n      \"pattern\": \"^\\\\d{4}-\\\\d{2}-\\\\d{2}$\"\n    },\n    \"zoneinfo\": {\n      \"type\": \"string\",\n      \"description\": \"End-user's time zone from the IANA Time Zone Database.\",\n      \"examples\": [\"America/Los_Angeles\", \"Europe/Paris\"]\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"End-user's locale as a BCP 47 language tag.\",\n      \"examples\": [\"en-US\", \"fr-FR\"]\n    },\n    \"phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"End-user's preferred telephone number in E.164 format.\",\n      \"examples\"\
  : [\"+1-555-555-1234\"]\n    },\n    \"phone_number_verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the end-user's phone number has been verified.\"\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"description\": \"End-user's preferred postal address.\",\n      \"properties\": {\n        \"formatted\": {\n          \"type\": \"string\",\n          \"description\": \"Full mailing address, formatted for display.\"\n        },\n        \"street_address\": {\n          \"type\": \"string\",\n          \"description\": \"Full street address, which may include house number, street name, and PO box.\"\n        },\n        \"locality\": {\n          \"type\": \"string\",\n          \"description\": \"City or locality.\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"State, province, prefecture, or region.\"\n        },\n        \"postal_code\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Zip code or postal code.\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country name.\"\n        }\n      }\n    },\n    \"updated_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Time the end-user's information was last updated. Represented as seconds since the Unix epoch.\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/json-schema/oidc-id-token.json
tags:
- Authentication
- Identity
- JWT
- OAuth
- OIDC
- OpenID Connect
title: OpenID Connect ID Token Claims
---
