---
description: The response for a user object.
layout: schema
name: User
properties_list:
- description: The internal database ID (uid) of the user.
  name: id
  type: integer
- description: The UUID for the user.
  name: uuid
  type: string
- description: The user name.
  name: name
  type: string
- description: The first name of the user.
  name: first_name
  type: string
- description: The last name of the user.
  name: last_name
  type: string
- description: The date/time of the last login for the user.
  name: last_login_at
  type: string
- description: The date/time when the user was created.
  name: created_at
  type: string
- description: The e-mail address of the user.
  name: mail
  type: string
- description: The telephone numbers for the user.
  name: phone
  type: object
- description: The job title of the user.
  name: job_title
  type: string
- description: The job function of the user.
  name: job_function
  type: string
- description: The company of the user.
  name: company
  type: string
- description: The country of the user.
  name: country
  type: string
- description: The state of the user, if in the United States.
  name: state
  type: string
- description: The timezone of the user.
  name: timezone
  type: string
- description: The user's picture url.
  name: picture_url
  type: string
- description: The various feature flags for the user.
  name: features
  type: array
- description: ''
  name: flags
  type: object
- description: Metadata related to the user.
  name: metadata
  type: object
- description: ''
  name: _links
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-user-schema.json
slug: acquia-cloud-user
source_filename: acquia-cloud-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"The response for a user object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"deprecated\": true,\n      \"type\": \"integer\",\n      \"description\": \"The internal database ID (uid) of the user.\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID for the user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The user name.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the user.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the user.\"\n    },\n    \"last_login_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"The date/time of the last login for the user.\",\n      \"nullable\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date/time when the user was created.\"\n    },\n    \"mail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The e-mail address of the user.\"\n    },\n    \"phone\": {\n      \"type\": \"object\",\n      \"description\": \"The telephone numbers for the user.\",\n      \"properties\": {\n        \"office\": {\n          \"type\": \"string\",\n          \"description\": \"The office telephone number for the user.\",\n          \"nullable\": true\n        },\n        \"tfa\": {\n          \"type\": \"string\",\n          \"description\": \"The tfa backup telephone number for the user.\",\n          \"nullable\": true\n        }\n      }\n    },\n    \"job_title\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The job title of the user.\"\n    },\n    \"job_function\": {\n      \"type\": \"string\",\n      \"description\": \"The job function of the user.\",\n      \"enum\": [\n        \"--\",\n        \"Business Executive\",\n        \"IT Executive\",\n        \"IT Architect or IT Operations\",\n        \"Product or Digital Marketing\",\n        \"Website Design or Development\"\n      ]\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"description\": \"The company of the user.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country of the user.\",\n      \"enum\": [\n        \"--\",\n        \"United States\",\n        \"Afghanistan\",\n        \"Albania\",\n        \"Algeria\",\n        \"American Samoa\",\n        \"Andorra\",\n        \"Angola\",\n        \"Anguilla\",\n        \"Antigua and Barbuda\",\n        \"Argentina\",\n        \"Armenia\",\n        \"Ascension Island\",\n        \"Australia\",\n\
  \        \"Austria\",\n        \"Azerbaijan\",\n        \"Bahamas\",\n        \"Bahrain\",\n        \"Bangladesh\",\n        \"Barbados\",\n        \"Belarus\",\n        \"Belgium\",\n        \"Belize\",\n        \"Benin\",\n        \"Bermuda\",\n        \"Bhutan\",\n        \"Bolivia\",\n        \"Bosnia and Herzegovina\",\n        \"Botswana\",\n        \"Brazil\",\n        \"British Indian Ocean Territory\",\n        \"Brunei Darussalam\",\n        \"Bulgaria\",\n        \"Burkina Faso\",\n        \"Burundi\",\n        \"Cambodia\",\n        \"Cameroon\",\n        \"Canada\",\n        \"Cape Verde\",\n        \"Cayman Islands\",\n        \"Central African Republic\",\n        \"Chad\",\n        \"Chile\",\n        \"China\",\n        \"Colombia\",\n        \"Comoros\",\n        \"Congo\",\n        \"Cook Islands\",\n        \"Costa Rica\",\n        \"Cote D Ivoire\",\n        \"Croatia\",\n        \"Cuba\",\n        \"Cyprus\",\n        \"Czech Republic\",\n        \"Denmark\",\n  \
  \      \"Djibouti\",\n        \"Dominica\",\n        \"Dominican Republic\",\n        \"Ecuador\",\n        \"Egypt\",\n        \"El Salvador\",\n        \"Equatorial Guinea\",\n        \"Eritrea\",\n        \"Estonia\",\n        \"Ethiopia\",\n        \"Falkland Islands\",\n        \"Faroe Islands\",\n        \"Federated States of Micronesia\",\n        \"Fiji\",\n        \"Finland\",\n        \"France\",\n        \"French Guiana\",\n        \"French Polynesia\",\n        \"Gabon\",\n        \"Georgia\",\n        \"Germany\",\n        \"Ghana\",\n        \"Greece\",\n        \"Greenland\",\n        \"Grenada\",\n        \"Guadeloupe\",\n        \"Guatemala\",\n        \"Guam\",\n        \"Guinea\",\n        \"Guinea Bissau\",\n        \"Guyana\",\n        \"Haiti\",\n        \"Holy See (Vatican City)\",\n        \"Honduras\",\n        \"Hong Kong\",\n        \"Hungary\",\n        \"Iceland\",\n        \"India\",\n        \"Indonesia\",\n        \"Iran\",\n        \"Ireland\",\n      \
  \  \"Isle of Man\",\n        \"Israel\",\n        \"Italy\",\n        \"Jamaica\",\n        \"Japan\",\n        \"Jordan\",\n        \"Kazakhstan\",\n        \"Kenya\",\n        \"Kiribati\",\n        \"Korea\",\n        \"Kuwait\",\n        \"Kyrgyzstan\",\n        \"Laos\",\n        \"Latvia\",\n        \"Lebanon\",\n        \"Lesotho\",\n        \"Liberia\",\n        \"Libya\",\n        \"Liechtenstein\",\n        \"Lithuania\",\n        \"Luxembourg\",\n        \"Macau\",\n        \"Macedonia\",\n        \"Madagascar\",\n        \"Malawi\",\n        \"Malaysia\",\n        \"Maldives\",\n        \"Mali\",\n        \"Malta\",\n        \"Marshall Islands\",\n        \"Martinique\",\n        \"Mauritius\",\n        \"Mayotte\",\n        \"Mexico\",\n        \"Moldova\",\n        \"Monaco\",\n        \"Mongolia\",\n        \"Montenegro\",\n        \"Montserrat\",\n        \"Morocco\",\n        \"Mozambique\",\n        \"Myanmar\",\n        \"Namibia\",\n        \"Nauru\",\n        \"Nepal\"\
  ,\n        \"Netherlands\",\n        \"Netherlands Antilles\",\n        \"New Caledonia\",\n        \"New Zealand\",\n        \"Nicaragua\",\n        \"Niger\",\n        \"Nigeria\",\n        \"Niue\",\n        \"Norfolk Island\",\n        \"Northern Mariana Islands\",\n        \"Norway\",\n        \"Oman\",\n        \"Pakistan\",\n        \"Palau\",\n        \"Palestine\",\n        \"Panama\",\n        \"Papua New Guinea\",\n        \"Paraguay\",\n        \"Peru\",\n        \"Philippines\",\n        \"Pitcairn\",\n        \"Poland\",\n        \"Portugal\",\n        \"Puerto Rico\",\n        \"Qatar\",\n        \"Reunion\",\n        \"Romania\",\n        \"Russian Federation\",\n        \"Rwanda\",\n        \"Saint Vincent and the Grenadines\",\n        \"San Marino\",\n        \"Sao Tome and Principe\",\n        \"Saudi Arabia\",\n        \"Senegal\",\n        \"Serbia\",\n        \"Seychelles\",\n        \"Sierra Leone\",\n        \"Singapore\",\n        \"Slovakia\",\n        \"Slovenia\"\
  ,\n        \"Solomon Islands\",\n        \"Somalia\",\n        \"South Africa\",\n        \"South Georgia\",\n        \"Spain\",\n        \"Sri Lanka\",\n        \"St. Kitts and Nevis\",\n        \"St. Lucia\",\n        \"St. Pierre and Miquelon\",\n        \"Sudan\",\n        \"Suriname\",\n        \"Swaziland\",\n        \"Sweden\",\n        \"Switzerland\",\n        \"Syrian Arab Republic\",\n        \"Taiwan\",\n        \"Tajikistan\",\n        \"Tanzania\",\n        \"Thailand\",\n        \"The Gambia\",\n        \"Togo\",\n        \"Tokelau\",\n        \"Tonga\",\n        \"Trinidad and Tobago\",\n        \"Tunisia\",\n        \"Turkey\",\n        \"Turkmenistan\",\n        \"Turks and Caicos Islands\",\n        \"Tuvalu\",\n        \"Uganda\",\n        \"Ukraine\",\n        \"United Arab Emirates\",\n        \"United Kingdom\",\n        \"Uruguay\",\n        \"Uzbekistan\",\n        \"Vanuatu\",\n        \"Venezuela\",\n        \"Viet Nam\",\n        \"Virgin Islands\",\n      \
  \  \"Western Samoa\",\n        \"Yemen\",\n        \"Yugoslavia\",\n        \"Zaire\",\n        \"Zambia\",\n        \"Zimbabwe\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the user, if in the United States.\",\n      \"enum\": [\n        \"Alabama\",\n        \"Alaska\",\n        \"American Samoa\",\n        \"Arizona\",\n        \"Arkansas\",\n        \"California\",\n        \"Colorado\",\n        \"Connecticut\",\n        \"Delaware\",\n        \"District of Columbia\",\n        \"Florida\",\n        \"Georgia\",\n        \"Hawaii\",\n        \"Idaho\",\n        \"Illinois\",\n        \"Indiana\",\n        \"Iowa\",\n        \"Kansas\",\n        \"Kentucky\",\n        \"Louisiana\",\n        \"Maine\",\n        \"Maryland\",\n        \"Massachusetts\",\n        \"Michigan\",\n        \"Minnesota\",\n        \"Mississippi\",\n        \"Missouri\",\n        \"Montana\",\n        \"Nebraska\",\n        \"Nevada\",\n        \"\
  New Hampshire\",\n        \"New Jersey\",\n        \"New Mexico\",\n        \"New York\",\n        \"North Carolina\",\n        \"North Dakota\",\n        \"Northern Mariana Islands\",\n        \"Ohio\",\n        \"Oklahoma\",\n        \"Oregon\",\n        \"Pennsylvania\",\n        \"Rhode Island\",\n        \"South Carolina\",\n        \"South Dakota\",\n        \"Tennessee\",\n        \"Texas\",\n        \"U.S. Virgin Islands\",\n        \"Utah\",\n        \"Vermont\",\n        \"Virginia\",\n        \"Washington\",\n        \"West Virginia\",\n        \"Wisconsin\",\n        \"Wyoming\"\n      ]\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"The timezone of the user.\"\n    },\n    \"picture_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The user's picture url.\"\n    },\n    \"features\": {\n      \"deprecated\": true,\n      \"type\": \"array\",\n      \"description\": \"The various feature flags for\
  \ the user.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"ci-pipelines\",\n          \"n3-disabled\",\n          \"n3-hybrid-mode\",\n          \"on-demand-environments\",\n          \"php7\",\n          \"php71\",\n          \"platform\"\n        ]\n      }\n    },\n    \"flags\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_user-flags\"\n    },\n    \"metadata\": {\n      \"deprecated\": true,\n      \"type\": \"object\",\n      \"description\": \"Metadata related to the user.\",\n      \"properties\": {\n        \"applications\": {\n          \"type\": \"object\",\n          \"description\": \"An array of application metadata for the user.\",\n          \"properties\": {\n            \"recent\": {\n              \"type\": \"array\",\n              \"description\": \"An array containing recent visited application information.\",\n              \"items\": {\n                \"type\": \"object\",\n                \"\
  properties\": {\n                  \"uuid\": {\n                    \"type\": \"string\",\n                    \"format\": \"uuid\",\n                    \"description\": \"The application UUID.\"\n                  },\n                  \"recent_at\": {\n                    \"type\": \"string\",\n                    \"format\": \"date-time\",\n                    \"description\": \"The date-time when the application was accessed.\"\n                  }\n                }\n              }\n            },\n            \"starred\": {\n              \"type\": \"array\",\n              \"description\": \"An array containing starred application UUIDs.\",\n              \"items\": {\n                \"type\": \"string\",\n                \"format\": \"uuid\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    }\n  },\n  \"required\": [\n    \"uuid\",\n    \"name\",\n  \
  \  \"first_name\",\n    \"last_name\",\n    \"last_login_at\",\n    \"created_at\",\n    \"mail\",\n    \"phone\",\n    \"job_title\",\n    \"job_function\",\n    \"company\",\n    \"country\",\n    \"timezone\",\n    \"picture_url\",\n    \"flags\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-user-schema.json
tags:
- Content
- Experience
title: User
---
