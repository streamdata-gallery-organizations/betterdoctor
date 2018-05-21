{
  "info": {
    "name": "BetterDoctor Retrieve a specific doctor description using NPI",
    "_postman_id": "6e5073bc-f1d2-4d3d-9ef6-cb6fbc96eee0",
    "description": "Returns a doctor object using NPI",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Doctor",
      "item": [
        {
          "id": "93e9a1f7-d619-4955-80ee-39969e810a48",
          "name": "doctor-search",
          "request": {
            "url": "http://api.betterdoctor.com/2016-03-01/doctors?fields=%7B%7D&first_name=%7B%7D&gender=%7B%7D&insurance_uid=%7B%7D&last_name=%7B%7D&limit=%7B%7D&location=%7B%7D&name=%7B%7D&practice_uid=%7B%7D&query=%7B%7D&skip=%7B%7D&sort=%7B%7D&specialty_uid=%7B%7D&user_key=%7B%7D&user_location=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Doctor search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d68b30e-a663-42ef-b8fd-4c3a28975771"
            }
          ]
        }
      ]
    },
    {
      "name": "Doctors",
      "item": [
        {
          "id": "b77b1219-e5aa-4e67-a3df-d90684cacb07",
          "name": "returns-a-doctor-object-based-on-an-uid-or-a-slug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "doctors/:uid"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a doctor object based on an uid or a slug"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "993e64dd-a0e1-4a43-ac69-32fc6e95b48f"
            }
          ]
        },
        {
          "id": "931c3534-d747-4288-8a0b-9cf00440fddb",
          "name": "returns-a-doctor-object-using-npi",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "doctors/npi/:npi"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "npi",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a doctor object using NPI"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f72d08f5-e04b-4986-a4f2-44970dff259e"
            }
          ]
        }
      ]
    }
  ]
}