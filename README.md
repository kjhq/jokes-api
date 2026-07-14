# jokes-api

serverless joke api with token auth. random joke from dynamodb — no valid token, 401.

![python](https://img.shields.io/badge/python-3776AB?style=flat-square&logo=python&logoColor=white)
![aws lambda](https://img.shields.io/badge/aws%20lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white)
![api gateway](https://img.shields.io/badge/api%20gateway-FF4F8B?style=flat-square&logo=amazonaws&logoColor=white)
![dynamodb](https://img.shields.io/badge/dynamodb-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white)

---

## what it does

fetches a random joke from the database. requires a valid `auth` header. built on aws lambda, api gateway, and dynamodb.

- proper auth checks
- exception handling + logging
- 500 on server errors with a clear message

`python` `lambda` `api gateway` `dynamodb`

---

## sample request

```
GET /Production/api/jokes HTTP/1.1
Host: h0zensjtaj.execute-api.ap-south-1.amazonaws.com
auth: 0
```

---

## sample response

```json
{
    "content": "What did the ocean say to the beach? Nothing, it just waved.",
    "authenticationStatus": true,
    "error": null
}
```

---

<div align="center">

built by [kjhq](https://kjhq.dev) · [@kjhqdev](https://x.com/kjhqdev)

</div>
