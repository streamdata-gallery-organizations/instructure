{
  "info": {
    "name": "Instructure Canvas Utility APIs List of CommMessages for a user",
    "_postman_id": "53e87388-db99-408e-ab98-872cac7aef75",
    "description": "List of commmessages for a user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Comm",
      "item": [
        {
          "id": "f426369c-9c06-44c5-92f3-21d35cfe90a8",
          "name": "list-of-commmessages-for-a-user",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/comm_messages?end_time=%7B%7D&start_time=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of commmessages for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b13a9753-f7dc-43aa-9576-9774bc850bd3"
            }
          ]
        }
      ]
    }
  ]
}