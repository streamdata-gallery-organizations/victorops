{
  "info": {
    "name": "Victor Ops Retrieve information for a user",
    "_postman_id": "982125a8-577a-4986-9dad-75734452bd0d",
    "description": "Get the information for the specified user\n\nThis API may be called a maximum of 15 times per minute.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Alerts",
      "item": [
        {
          "id": "385cdafe-6423-4c03-b760-cbd2e5a53f21",
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
              "id": "e3bd4717-d2f2-4609-a27b-ebca54f058dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Incidents",
      "item": [
        {
          "id": "b43697a9-f253-4e92-9c83-5a48cf2146ea",
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
              "id": "202297ee-f4e3-441e-9518-e82c303bb80f"
            }
          ]
        },
        {
          "id": "c6ec5959-040b-4252-ac1b-4efa42f7d0cb",
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
              "id": "83cc1e0e-0362-4d1c-99b2-3d68d5fcec8e"
            }
          ]
        },
        {
          "id": "6278c503-4249-4d5c-93dc-79cc3235448c",
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
              "id": "e6970b7f-199d-49a4-91e3-86c28dde93bc"
            }
          ]
        },
        {
          "id": "cf85d557-3e08-41af-b642-409d5968076a",
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
              "id": "fb3509a0-a310-4dbc-a70d-2580a5c0284d"
            }
          ]
        },
        {
          "id": "fb0918c4-7d2f-40ad-851b-018d13b06d46",
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
              "id": "247004ae-35e7-48f6-a479-9620ed46f503"
            }
          ]
        },
        {
          "id": "478de483-9f1b-441c-b5af-4dcf1d4d2611",
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
              "id": "aacc0949-bd33-4184-a11b-3f8ad6014bee"
            }
          ]
        },
        {
          "id": "3bebfc8b-7bcc-4889-9893-adff5e6f0e0f",
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
              "id": "71d74aa5-2e6c-4a31-85f3-f3b682611cfe"
            }
          ]
        }
      ]
    },
    {
      "name": "Oncall",
      "item": [
        {
          "id": "81f2bc2d-4c6e-457a-85e5-30b595bfafac",
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
              "id": "b5722d31-8f58-4309-98c6-030e6e040aa5"
            }
          ]
        }
      ]
    },
    {
      "name": "Org",
      "item": [
        {
          "id": "81bc29ce-b202-4ac0-8486-82f6e64d51da",
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
              "id": "59c2ed34-4c8d-4616-892b-79aa6b90de5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "41a590f0-0fe7-4997-a068-85c4f887ece6",
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
              "id": "6e715e26-920c-4c51-a5cc-3febdb80d47f"
            }
          ]
        },
        {
          "id": "0e9aa51c-52ae-4848-a3a5-7ed5bb0e3412",
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
              "id": "6e5b7f88-7811-447f-9ffe-ee818f5fabd2"
            }
          ]
        },
        {
          "id": "a469a4f8-c624-4e0e-97b5-79d4d653bb1d",
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
              "id": "1327d970-8ee3-48dd-a509-9f8657d41d95"
            }
          ]
        },
        {
          "id": "12b86cc3-8d9e-4307-8559-6daaf1b03c71",
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
              "id": "45116fe8-fab2-4c81-aef4-b78946971332"
            }
          ]
        },
        {
          "id": "bd3debaf-fa95-4e1e-a0fa-3c44efd2a234",
          "name": "api_public.v1.policies.policy.oncall.user.patch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/policies/:policy/oncall/user"
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
                  "id": "policy",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Replaces a currently on-call user in the escalation policy with another.  In many cases, the policy slug\nwill match the slug of the team that contains it.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "538e931d-d68a-4457-af43-f73b80b8ac25"
            }
          ]
        }
      ]
    },
    {
      "name": "Profile",
      "item": [
        {
          "id": "1934c334-cdcc-418a-9b6e-af340d1a0379",
          "name": "api_public.v1.profile.username.policies.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all the paging policy steps for the user on the org associated with the API key\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38960e5f-ab08-4da7-876c-5edb3f2315e1"
            }
          ]
        },
        {
          "id": "4028f4d8-005e-4100-aac8-83f2b9c7df69",
          "name": "api_public.v1.profile.username.policies.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83792ff2-004f-49df-be5d-1e129482d12f"
            }
          ]
        },
        {
          "id": "347defa9-981b-40fe-a3e2-7d6ac3608e19",
          "name": "api_public.v1.profile.username.policies.step.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8289a8f-4c63-40ab-b31d-5370cefc45c3"
            }
          ]
        },
        {
          "id": "ae947262-3d6c-43ed-b7d9-49cd87b0eef0",
          "name": "api_public.v1.profile.username.policies.step.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca257077-5190-45e6-bc37-a2f8e2c2e455"
            }
          ]
        },
        {
          "id": "840cf57f-199d-43b3-a21d-63e87105c638",
          "name": "api_public.v1.profile.username.policies.step.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a rule for a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b454800b-db93-4ae2-936e-f51769f2fce6"
            }
          ]
        },
        {
          "id": "d2428b89-a5f0-4e8d-b6ab-6c51663f53e6",
          "name": "api_public.v1.profile.username.policies.step.rule.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a rule from a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ff9c27a-f0d3-4e03-9d2b-917e1f9f2fc8"
            }
          ]
        },
        {
          "id": "461a6cbb-899b-4915-9af0-6848f6b5cf6e",
          "name": "api_public.v1.profile.username.policies.step.rule.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a rule for a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff66503d-c842-49fe-8c94-abd2d2f5d425"
            }
          ]
        },
        {
          "id": "f9e8ec8e-c636-452a-aadb-527eecf6109b",
          "name": "api_public.v1.profile.username.policies.step.rule.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/profile/:username/policies/:step/:rule"
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
                  "id": "username",
                  "value": "username",
                  "type": "string"
                },
                {
                  "id": "step",
                  "value": "step",
                  "type": "string"
                },
                {
                  "id": "rule",
                  "value": "rule",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a rule from a paging policy step\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "380be63b-6b21-46bf-87c9-fb0700cc2251"
            }
          ]
        }
      ]
    },
    {
      "name": "Team",
      "item": [
        {
          "id": "180d309a-a9a2-4671-9493-c7077639c5e2",
          "name": "api_public.v1.team.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/team?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of teams for your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9c9c8ae-52d9-49fb-b57c-88265e2255d6"
            }
          ]
        },
        {
          "id": "0b6d1695-b1a0-4c76-8be5-bcc2d08574e9",
          "name": "api_public.v1.team.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/team?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a team to your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3740ff97-6d4c-4b9c-9636-4799583cb099"
            }
          ]
        },
        {
          "id": "0dc5590b-d083-465e-ae40-044ebb43ef89",
          "name": "api_public.v1.team.team.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the information for the specified team.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1f425e6-735d-4710-a724-e276f5a10f45"
            }
          ]
        },
        {
          "id": "03047252-9258-4248-aed3-20c1e42d157b",
          "name": "api_public.v1.team.team.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update the designated team\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cdb9c5c-baf8-4525-82bd-d3c794b3300c"
            }
          ]
        },
        {
          "id": "84144486-eaff-4a29-96fd-460b3c9ecf2b",
          "name": "api_public.v1.team.team.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a team from your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f3a4d5c-1e4d-4013-a09e-e173156583af"
            }
          ]
        },
        {
          "id": "5f8d6574-cea5-4abe-8e56-08cdd2cce23b",
          "name": "api_public.v1.team.team.members.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/members"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the members for the specified team.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e8bb662-ec0a-4143-b972-eda3a4dd9b81"
            }
          ]
        },
        {
          "id": "7eaa3ddf-d932-45a0-b758-28086cad01d0",
          "name": "api_public.v1.team.team.members.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/members"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a team member to your team.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9da4782b-eb95-4583-9a3c-7c25af0cdecb"
            }
          ]
        },
        {
          "id": "6d23a9ea-2677-4886-bf4c-c2115ebf6944",
          "name": "api_public.v1.team.team.members.user.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/members/:user"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a team from your organization.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f5404d1-83b8-4ade-8b73-96be363c3db3"
            }
          ]
        },
        {
          "id": "f0852da9-8822-4af6-aa92-ef33588f4763",
          "name": "api_public.v1.team.team.oncall.schedule.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/oncall/schedule"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "__NOTE: This call is deprecated. Please use `GET /api-public/v2/team/{team}/oncall/schedule`.__\n\nGet the on-call schedule for a team, including on-call overrides.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7b6d254-c939-4b60-b58c-8da21c29ae1e"
            }
          ]
        },
        {
          "id": "cac3826d-cf0d-43fc-958c-651031af9736",
          "name": "api_public.v1.team.team.oncall.user.patch",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/oncall/user"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "__NOTE: This API call is deprecated. Please use `PATCH /api-public/v2/policies/{policy}/oncall/user`__\n\nReplaces a currently on-call user on the team with another.\n\nThis API may be called a maximum of 6 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3990ad4b-10f3-4f5f-97e3-7319e01d283e"
            }
          ]
        },
        {
          "id": "5378db74-f9c7-4f14-afc5-ca3e02d0d3d8",
          "name": "api_public.v1.team.team.policies.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/team/:team/policies"
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
                  "id": "team",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the escalation policies for the specified team.\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8eb203bd-13de-439c-abd3-49b5507bf441"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "933c5257-a53c-4033-91d2-3c92ef3b6c57",
          "name": "api_public.v1.user.get",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/user?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of users for your organization\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69fd977d-0880-4663-b130-8e7fcb598d1d"
            }
          ]
        },
        {
          "id": "c3d99893-f5f2-4dfd-a6b4-55c604a07c98",
          "name": "api_public.v1.user.post",
          "request": {
            "url": "http://api.victorops.com/api-public/v1/user?No Name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a user to your organization\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9955eee-ef69-4baf-9162-02dd656b0b94"
            }
          ]
        },
        {
          "id": "912c70f4-f0f7-4089-8ff9-a77b29e36610",
          "name": "api_public.v1.user.user.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the information for the specified user\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81889dc7-60b5-4d4a-9581-8c078a3fa2e9"
            }
          ]
        },
        {
          "id": "664db534-97f9-4643-a5fc-b266119e9142",
          "name": "api_public.v1.user.user.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.victorops.com",
              "path": [
                "api-public/v1/user/:user"
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
                  "id": "user",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove a user from your organization\n\nThis API may be called a maximum of 15 times per minute."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db37fe08-2ce7-4e87-bd1f-b65d368648f7"
            }
          ]
        }
      ]
    }
  ]
}