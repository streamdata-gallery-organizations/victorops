{
  "info": {
    "name": "Victor Ops Get the available timeout values",
    "_postman_id": "5270eaf5-5b66-40cd-9ec0-d6a1930500d9",
    "description": "Get the available timeout values\n\ndescription: \"If still unacked after 1 minute\", type: 1\ndescription: \"If still unacked after 5 minutes\", type: 5\ndescription: \"If still unacked after 10 minutes\", type: 10\ndescription: \"If still unacked after 15 minutes\", type: 15\ndescription: \"If still unacked after 20 minutes\", type: 20\ndescription: \"If still unacked after 25 minutes\", type: 25\ndescription: \"If still unacked after 30 minutes\", type: 30\ndescription: \"If still unacked after 45 minutes\", type: 45\ndescription: \"If still unacked after 60 minutes\", type: 60\n\nThis API may be called a maximum of 15 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Alerts",
      "item": [
        {
          "id": "ac4c4d17-3e3d-4867-a39f-ee875133bcfd",
          "name": "api_public.v1.alerts.uuid.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/alerts/:uuid"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the details of an alert that was sent VictorOps by you.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20500592-1761-4c3d-ba6b-33588fa6489b"
            }
          ]
        }
      ]
    },
    {
      "name": "Incidents",
      "item": [
        {
          "id": "6d21b393-ac90-477b-9219-e2c1f9a7c337",
          "name": "api_public.v1.incidents.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of the currently open, acknowledged and recently resolved incidents.\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e09f622-ce0e-4363-8d59-237ff03fd587"
            }
          ]
        },
        {
          "id": "8b0b6e0e-5e45-4256-8ca8-61e1674ab7e3",
          "name": "api_public.v1.incidents.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new incident.\n\nThis call replicates the function of our\nmanual incident creation process.\nMonitoring tools and custom integrations\nshould be configured using our\nREST Endpoint.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "425e83fc-e5fa-4b9e-955b-2c18707f1e4d"
            }
          ]
        },
        {
          "id": "7b8f01ab-4138-4849-99f7-d872c830d9e3",
          "name": "api_public.v1.incidents.ack.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/ack?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e343bb21-9ed7-4604-aca6-2cce3e048641"
            }
          ]
        },
        {
          "id": "1f5d1e9c-1ca0-40c0-9406-94a48dfd99c5",
          "name": "api_public.v1.incidents.byUser.ack.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/byUser/ack?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41eab08f-442e-42ac-a28b-52ae99774ed2"
            }
          ]
        },
        {
          "id": "407ee99b-2ad4-434c-bca7-0d498548f3fe",
          "name": "api_public.v1.incidents.byUser.resolve.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/byUser/resolve?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "025cd6f4-5254-466b-9540-b632a5cc00cd"
            }
          ]
        },
        {
          "id": "063da161-e954-4ad7-9c7e-6f763f79c984",
          "name": "api_public.v1.incidents.reroute.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/reroute?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reroute one or more incidents to one or more users and/or escalation policies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd1d0dc4-dd78-4135-92c2-a1cebef07927"
            }
          ]
        },
        {
          "id": "3a6e4706-be99-42fe-bc9a-242f679bb77b",
          "name": "api_public.v1.incidents.resolve.patch",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/incidents/resolve?No Name=%7B%7D",
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc5b165e-e67a-41af-afc4-599d59acccca"
            }
          ]
        }
      ]
    },
    {
      "name": "Oncall",
      "item": [
        {
          "id": "9d821c52-f697-4785-b8ad-07ce1784971c",
          "name": "api_public.v1.oncall.current.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/oncall/current?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all on-call uesrs/teams for your organization.\n\nThis API may be called a maximum of 1 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90e0d07c-1875-4539-8fc4-693fc9323bd9"
            }
          ]
        }
      ]
    },
    {
      "name": "Org",
      "item": [
        {
          "id": "852636b1-130d-4e6c-8440-d296471ea25e",
          "name": "api_public.v1.org.routing_keys.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/org/routing-keys?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of routing keys and associated teams.\nThis API may be called a maximum of once a minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "684960c0-94e0-442f-9a22-50026d88143e"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "7d8d3f24-24bd-4bc7-90e8-312ef2c62078",
          "name": "api_public.v1.policies.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of escalation policy information.\nThis API may be called a maximum of once a minute"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "872b8064-e6d0-4b7f-9f72-0812c100c556"
            }
          ]
        },
        {
          "id": "dfe78bfd-bd90-4e06-ba08-97ff3eb331d9",
          "name": "api_public.v1.policies.types.contacts.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/contacts?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available contact types\n\ndescription: \"Email Address\", type: \"email\"\ndescription: \"Phone Number\", type: \"phone\"\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bbe8456-9f30-4bb3-88a6-0483ffb27d85"
            }
          ]
        },
        {
          "id": "0b5e3e48-31b0-413e-9f80-5601b87130e0",
          "name": "api_public.v1.policies.types.notifications.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/notifications?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available notification types\n\ndescription: \"Send a push notification to all my devices\", type: \"push\"\ndescription: \"Send an email to an email address\", type: \"email\"\ndescription: \"Send an SMS to a phone number\", type: \"sms\"\ndescription: \"Make a phone call to a phone number\", type: \"phone\"\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2c4f8a8d-0d6c-4c55-95fa-299f382aa876"
            }
          ]
        },
        {
          "id": "3b8db8b2-0adc-4f2e-b060-dd176a00f260",
          "name": "api_public.v1.policies.types.timeouts.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/policies/types/timeouts?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the available timeout values\n\ndescription: \"If still unacked after 1 minute\", type: 1\ndescription: \"If still unacked after 5 minutes\", type: 5\ndescription: \"If still unacked after 10 minutes\", type: 10\ndescription: \"If still unacked after 15 minutes\", type: 15\ndescription: \"If still unacked after 20 minutes\", type: 20\ndescription: \"If still unacked after 25 minutes\", type: 25\ndescription: \"If still unacked after 30 minutes\", type: 30\ndescription: \"If still unacked after 45 minutes\", type: 45\ndescription: \"If still unacked after 60 minutes\", type: 60\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6457a25-b852-4f12-83ba-de4733138686"
            }
          ]
        }
      ]
    }
  ]
}