{
  "info": {
    "name": "BetterDoctor Retrieve a specific doctor description",
    "_postman_id": "b899850b-f0d8-4394-b83d-5527e31813f3",
    "description": "Returns a doctor object based on an uid or a slug",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Doctor",
      "item": [
        {
          "id": "ec2ceadc-14f8-49ef-8e6d-c001f1e39d59",
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
              "id": "ce3bc7ae-8c25-423d-899e-369e4ab87aa1"
            }
          ]
        }
      ]
    },
    {
      "name": "Doctors",
      "item": [
        {
          "id": "0a7d7bc8-efc8-4a53-b4ef-144dd3f4af8c",
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
              "id": "a8b8ee79-3c3a-4864-ad2c-fead99ddc1ce"
            }
          ]
        }
      ]
    }
  ]
}