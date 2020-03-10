---
# This file is automatically generated from the API using `sentry/api-docs/generator.py.`
# Do not manually edit this file.
{
  "api_path": "/api/0/issues/{issue_id}/events/", 
  "authentication": "required", 
  "description": "This endpoint lists an issue's events.", 
  "example_request": "GET /api/0/issues/1/events/ HTTP/1.1\nHost: sentry.io\nAuthorization: Bearer <token>", 
  "example_response": "HTTP/1.1 200 OK\nContent-Length: 952\nX-XSS-Protection: 1; mode=block\nX-Content-Type-Options: nosniff\nContent-Language: en\nAccess-Control-Expose-Headers: X-Sentry-Error, Retry-After\nVary: Accept-Language, Cookie\nAccess-Control-Allow-Methods: GET, HEAD, OPTIONS\nLink: <https://sentry.io/api/0/issues/1/events/?&cursor=0:0:1>; rel=\"previous\"; results=\"false\"; cursor=\"0:0:1\", <https://sentry.io/api/0/issues/1/events/?&cursor=0:100:0>; rel=\"next\"; results=\"false\"; cursor=\"0:100:0\"\nAllow: GET, HEAD, OPTIONS\nAccess-Control-Allow-Origin: *\nAccess-Control-Allow-Headers: X-Sentry-Auth, X-Requested-With, Origin, Accept, Content-Type, Authentication, Authorization\nContent-Type: application/json\nX-Frame-Options: deny\n\n[\n  {\n    \"crashFile\": null, \n    \"culprit\": \"raven.scripts.runner in main\", \n    \"dateCreated\": \"2020-03-10T05:57:36Z\", \n    \"event.type\": \"default\", \n    \"eventID\": \"d1199944a8f34d53976b287ef410b3d7\", \n    \"groupID\": \"1\", \n    \"id\": \"d1199944a8f34d53976b287ef410b3d7\", \n    \"location\": null, \n    \"message\": \"This is an example python exception\", \n    \"platform\": \"python\", \n    \"projectID\": \"2\", \n    \"tags\": [\n      {\n        \"key\": \"browser\", \n        \"value\": \"Chrome 28.0.1500\"\n      }, \n      {\n        \"key\": \"browser.name\", \n        \"value\": \"Chrome\"\n      }, \n      {\n        \"key\": \"client_os\", \n        \"value\": \"Windows 8\"\n      }, \n      {\n        \"key\": \"client_os.name\", \n        \"value\": \"Windows\"\n      }, \n      {\n        \"key\": \"environment\", \n        \"value\": \"prod\"\n      }, \n      {\n        \"key\": \"level\", \n        \"value\": \"error\"\n      }, \n      {\n        \"key\": \"release\", \n        \"value\": \"284bca5a5bb4a5d8b2541892cc492af84e7fb8c4\"\n      }, \n      {\n        \"key\": \"user\", \n        \"query\": \"user.id:\\\"1\\\"\", \n        \"value\": \"id:1\"\n      }, \n      {\n        \"key\": \"server_name\", \n        \"value\": \"web01.example.org\"\n      }, \n      {\n        \"key\": \"url\", \n        \"value\": \"http://example.com/foo\"\n      }\n    ], \n    \"title\": \"This is an example python exception\", \n    \"user\": {\n      \"data\": null, \n      \"email\": \"sentry@example.com\", \n      \"id\": \"1\", \n      \"ip_address\": \"127.0.0.1\", \n      \"name\": \"Sentry\", \n      \"username\": \"sentry\"\n    }\n  }\n]", 
  "method": "GET", 
  "parameters": null, 
  "path_parameters": [
    {
      "description": "the ID of the issue to retrieve.", 
      "name": "issue_id", 
      "type": "string"
    }
  ], 
  "query_parameters": [
    {
      "description": "if this is set to true then the event payload will include the full event body, including the stacktrace. Set to 1 to enable.", 
      "name": "full", 
      "type": "bool"
    }
  ], 
  "sidebar_order": 18, 
  "title": "List an Issue's Events", 
  "warning": null
}
---