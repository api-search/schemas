---
description: <p>The client branding attributes for iOS device types. These attributes are displayed on the iOS client login screen only.</p> <important> <p>Client branding attributes are public facing. Ensure you do not include sensitive information.</p> </important>
layout: schema
name: IosClientBrandingAttributes
properties_list:
- description: ''
  name: LogoUrl
  type: object
- description: ''
  name: Logo2xUrl
  type: object
- description: ''
  name: Logo3xUrl
  type: object
- description: ''
  name: SupportEmail
  type: object
- description: ''
  name: SupportLink
  type: object
- description: ''
  name: ForgotPasswordLink
  type: object
- description: ''
  name: LoginMessage
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-ios-client-branding-attributes-schema.json
slug: workspaces-ios-client-branding-attributes
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogoUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientUrl\"\n        },\n        {\n          \"description\": \"The logo. This is the standard-resolution display that has a 1:1 pixel density (or @1x), where one pixel is equal to one point. The only image format accepted is a binary data object that is converted from a <code>.png</code> file.\"\n        }\n      ]\n    },\n    \"Logo2xUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientUrl\"\n        },\n        {\n          \"description\": \"<p>The @2x version of the logo. This is the higher resolution display that offers a scale factor of 2.0 (or @2x). The only image format accepted is a binary data object that is converted from a <code>.png</code> file.</p> <note> <p> For more information about iOS image size and resolution, see <a href=\\\"https://developer.apple.com/design/human-interface-guidelines/ios/icons-and-images/image-size-and-resolution/\\\
  \">Image Size and Resolution </a> in the <i>Apple Human Interface Guidelines</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"Logo3xUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientUrl\"\n        },\n        {\n          \"description\": \"<p>The @3x version of the logo. This is the higher resolution display that offers a scale factor of 3.0 (or @3x).The only image format accepted is a binary data object that is converted from a <code>.png</code> file.</p> <note> <p> For more information about iOS image size and resolution, see <a href=\\\"https://developer.apple.com/design/human-interface-guidelines/ios/icons-and-images/image-size-and-resolution/\\\">Image Size and Resolution </a> in the <i>Apple Human Interface Guidelines</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"SupportEmail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientEmail\"\n        },\n        {\n          \"description\": \"<p>The\
  \ support email. The company's customer support email address.</p> <note> <ul> <li> <p>In each platform type, the <code>SupportEmail</code> and <code>SupportLink</code> parameters are mutually exclusive. You can specify one parameter for each platform type, but not both.</p> </li> <li> <p>The default email is <code>workspaces-feedback@amazon.com</code>.</p> </li> </ul> </note>\"\n        }\n      ]\n    },\n    \"SupportLink\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientUrl\"\n        },\n        {\n          \"description\": \"<p>The support link. The link for the company's customer support page for their WorkSpace.</p> <note> <ul> <li> <p>In each platform type, the <code>SupportEmail</code> and <code>SupportLink</code> parameters are mutually exclusive. You can specify one parameter for each platform type, but not both.</p> </li> <li> <p>The default support link is <code>workspaces-feedback@amazon.com</code>.</p> </li> </ul> </note>\"\n       \
  \ }\n      ]\n    },\n    \"ForgotPasswordLink\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientUrl\"\n        },\n        {\n          \"description\": \"The forgotten password link. This is the web address that users can go to if they forget the password for their WorkSpace.\"\n        }\n      ]\n    },\n    \"LoginMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoginMessage\"\n        },\n        {\n          \"description\": \"The login message. Specified as a key value pair, in which the key is a locale and the value is the localized message for that locale. The only key supported is <code>en_US</code>. The HTML tags supported include the following: <code>a, b, blockquote, br, cite, code, dd, dl, dt, div, em, i, li, ol, p, pre, q, small, span, strike, strong, sub, sup, u, ul</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>The client branding attributes for iOS device types. These attributes\
  \ are displayed on the iOS client login screen only.</p> <important> <p>Client branding attributes are public facing. Ensure you do not include sensitive information.</p> </important>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IosClientBrandingAttributes\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-ios-client-branding-attributes-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-ios-client-branding-attributes-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: IosClientBrandingAttributes
---
