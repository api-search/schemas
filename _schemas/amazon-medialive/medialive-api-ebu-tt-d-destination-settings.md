---
description: Ebu Tt DDestination Settings
layout: schema
name: EbuTtDDestinationSettings
properties_list:
- description: ''
  name: CopyrightHolder
  type: object
- description: ''
  name: FillLineGap
  type: object
- description: ''
  name: FontFamily
  type: object
- description: ''
  name: StyleControl
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-ebu-tt-d-destination-settings-schema.json
slug: medialive-api-ebu-tt-d-destination-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ebu-tt-d-destination-settings-schema.json\",\n  \"title\": \"EbuTtDDestinationSettings\",\n  \"description\": \"Ebu Tt DDestination Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CopyrightHolder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"copyrightHolder\"\n          },\n          \"description\": \"Complete this field if you want to include the name of the copyright holder in the copyright tag in the captions metadata.\"\n        }\n      ]\n    },\n    \"FillLineGap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbuTtDFillLineGapControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fillLineGap\"\
  \n          },\n          \"description\": \"Specifies how to handle the gap between the lines (in multi-line captions).\\n\\n- enabled: Fill with the captions background color (as specified in the input captions).\\n- disabled: Leave the gap unfilled.\"\n        }\n      ]\n    },\n    \"FontFamily\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontFamily\"\n          },\n          \"description\": \"Specifies the font family to include in the font data attached to the EBU-TT captions. Valid only if styleControl is set to include. If you leave this field empty, the font family is set to \\\"monospaced\\\". (If styleControl is set to exclude, the font family is always set to \\\"monospaced\\\".)\\n\\nYou specify only the font family. All other style information (color, bold, position and so on) is copied from the input captions. The size is always set to 100% to allow the downstream\
  \ player to choose the size.\\n\\n- Enter a list of font families, as a comma-separated list of font names, in order of preference. The name can be a font family (such as \\u201cArial\\u201d), or a generic font family (such as \\u201cserif\\u201d), or \\u201cdefault\\u201d (to let the downstream player choose the font).\\n- Leave blank to set the family to \\u201cmonospace\\u201d.\"\n        }\n      ]\n    },\n    \"StyleControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbuTtDDestinationStyleControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"styleControl\"\n          },\n          \"description\": \"Specifies the style information (font color, font position, and so on) to include in the font data that is attached to the EBU-TT captions.\\n\\n- include: Take the style information (font color, font position, and so on) from the source captions and include that information in the font data attached to the EBU-TT captions.\
  \ This option is valid only if the source captions are Embedded or Teletext.\\n- exclude: In the font data attached to the EBU-TT captions, set the font family to \\\"monospaced\\\". Do not include any other style information.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ebu-tt-d-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: EbuTtDDestinationSettings
---
