## Login API:

- Url: https://1proxy.net/api/auth/login

- Json body: 
```
{
	"email": "username@gmail.com",
	"password": "password"
}
```

- Response:
```
{
  "user": {
    "id": 5,
    "first_name": "user",
    "last_name": "name",
    "phone_number": "0999999999",
    "email": "username@gmail.com",
    "role": "MEMBER",
    "created_at": "2023-11-04T05:48:38.000000Z",
    "updated_at": "2023-11-04T05:48:38.000000Z"
  },
  "token": "your-token",
  "token_type": "Bearer"
}
```
__________________________________

## GET PLAN:

- Url: https://1proxy.net/api/user-plans

- Headers:
```
{
	"Accept":"application/json",
  "Authorization": "Bearer your-token"
}
```

- Response:
```
{
    "status": "SUCCESS",
    "statusCode": 200,
    "data": [
      {
        "id": 6,
        "name": "DT MINI",
        "slug": "dt-mini",
        "amount": 100,
        "type": "MONTH",
        "proxy_type": "HTTP",
        "price": 10000,
        "is_active": 1,
        "description": "Proxy Datacenter IPv4<br>\n<strong>Số lượng: </strong>100<br>\n<strong>Ngày sử dụng: </strong>30 Ngày<br>\n<strong>Thời gian làm mới: </strong>2 ngày/lần<br>",
        "deleted_at": null,
        "created_at": "2023-11-06T15:51:40.000000Z",
        "updated_at": "2023-12-07T12:13:16.000000Z",
        "user_id": 5,
        "is_vip": 1
      },
      {
        "id": 7,
        "name": "DT 1K",
        "slug": "dt-1k",
        "amount": 1000,
        "type": "MONTH",
        "proxy_type": "HTTP",
        "price": 99000,
        "is_active": 1,
        "description": "Proxy Datacenter IPv4<br>\n<strong>Số lượng: </strong>1000<br>\n<strong>Ngày sử dụng: </strong>30 Ngày<br>\n<strong>Thời gian làm mới: </strong>2 ngày/lần<br>",
        "deleted_at": null,
        "created_at": "2023-11-06T15:52:20.000000Z",
        "updated_at": "2023-12-07T12:12:13.000000Z",
        "user_id": 5,
        "is_vip": 1
      },
      {
        "id": 8,
        "name": "DT 3K",
        "slug": "dt-3k",
        "amount": 3000,
        "type": "MONTH",
        "proxy_type": "HTTP",
        "price": 299000,
        "is_active": 1,
        "description": "Proxy Datacenter IPv4<br>\n<strong>Số lượng: </strong>3000<br>\n<strong>Ngày sử dụng: </strong>30 Ngày<br>\n<strong>Thời gian làm mới: </strong>2 ngày/lần<br>",
        "deleted_at": null,
        "created_at": "2023-11-06T15:52:44.000000Z",
        "updated_at": "2023-12-07T12:13:25.000000Z",
        "user_id": 5,
        "is_vip": 1
      },
      {
        "id": 9,
        "name": "DT 5K",
        "slug": "dt-5k",
        "amount": 5000,
        "type": "MONTH",
        "proxy_type": "HTTP",
        "price": 488000,
        "is_active": 1,
        "description": "Proxy Datacenter IPv4<br>\n<strong>Số lượng: </strong>5000<br>\n<strong>Ngày sử dụng: </strong>30 Ngày<br>\n<strong>Thời gian làm mới: </strong>2 ngày/lần<br>",
        "deleted_at": null,
        "created_at": "2023-11-06T15:53:03.000000Z",
        "updated_at": "2023-12-07T12:13:36.000000Z",
        "user_id": 5,
        "is_vip": 1
      },
      {
        "id": 10,
        "name": "DT 7K",
        "slug": "dt-7k",
        "amount": 7000,
        "type": "MONTH",
        "proxy_type": "HTTP",
        "price": 650000,
        "is_active": 1,
        "description": "Proxy Datacenter IPv4<br>\n<strong>Số lượng: </strong>7000<br>\n<strong>Ngày sử dụng: </strong>30 Ngày<br>\n<strong>Thời gian làm mới: </strong>2 ngày/lần<br>",
        "deleted_at": null,
        "created_at": "2023-11-06T15:55:33.000000Z",
        "updated_at": "2023-12-07T12:11:00.000000Z",
        "user_id": 5,
        "is_vip": 1
      },
      {
        "id": 14,
        "name": "DT MAX",
        "slug": "dt-max",
        "amount": 40000,
        "type": "MONTH",
        "proxy_type": "HTTP",
        "price": 2500000,
        "is_active": 1,
        "description": "Proxy HTTP IPv4 Datacenter<br>\n<strong>Số lượng: </strong>Không giới hạn<br>\n<strong>Ngày sử dụng: </strong>30 Ngày<br>\n<strong>Thời gian làm mới: </strong>2 ngày/lần<br>",
        "deleted_at": null,
        "created_at": "2023-12-21T10:57:51.000000Z",
        "updated_at": "2023-12-21T10:59:36.000000Z",
        "user_id": 5,
        "is_vip": 1
      },
      {
        "id": 15,
        "name": "DT MAXS",
        "slug": "dt-maxs",
        "amount": 40000,
        "type": "YEAR",
        "proxy_type": "HTTP",
        "price": 20000000,
        "is_active": 1,
        "description": "Proxy HTTP IPv4 Datacenter<br>\n<strong>Số lượng: </strong>Không giới hạn<br>\n<strong>Ngày sử dụng: </strong>1 Năm<br>\n<strong>Thời gian làm mới: </strong>2 ngày/lần<br>",
        "deleted_at": null,
        "created_at": "2023-12-21T10:58:39.000000Z",
        "updated_at": "2023-12-21T11:00:04.000000Z",
        "user_id": 5,
        "is_vip": 1
      }
    ]
  }
```
__________________________________

## GET GEOLOCAL

- Url: https://1proxy.net/api/geos?is_show_inactive=0

- Headers:
```
{
	"Accept":"application/json",
  "Authorization": "Bearer your-token"
}
```
- Response:
```
[
  {
    "id": 230,
    "name": "United States",
    "code": "US",
    "is_active": 1,
    "created_at": "2023-10-21T05:40:58.000000Z",
    "updated_at": "2023-11-11T03:31:46.000000Z"
  },
  {
    "id": 236,
    "name": "Viet Nam",
    "code": "VN",
    "is_active": 1,
    "created_at": "2023-10-21T05:40:58.000000Z",
    "updated_at": "2023-10-21T18:48:54.000000Z"
  }
]
```

__________________________________


## Check Budget:
- Url: https://1proxy.net/api/payments/budget

- Headers:
```
{
  "Accept":"application/json",
  "Authorization": "Bearer your-token"
}
```
- Response:
```
{
      "status": "SUCCESS",
      "statusCode": 200,
      "data": {
          "id": 3,
          "payment_code": "NAP5137",
          "amount_snap": 95646000,
          "created_at": "2023-11-04T05:48:38.000000Z",
          "updated_at": "2023-12-22T16:44:51.000000Z",
          "user_id": 5
      }
}
```

__________________________________


## BUY Proxy

- Url: https://1proxy.net/api/orders

- Json body:
```
  {
    "plan_id": 6,
    "geo_key": "VN"
  }
```
- Response:
```
  {
    "status": "SUCCESS",
    "statusCode": 200,
    "data": [
        {
            "id": 194,
            "price": "99000.00",
            "quantity": 1,
            "amount": 1000,
            "type": "MONTH",
            "proxy_type": "HTTP",
            "geo_key": "VN",
            "order_id": 201,
            "plan_id": 7,
            "user_id": 5,
            "created_at": "2023-12-22T16:44:51.000000Z",
            "updated_at": "2023-12-22T16:44:51.000000Z",
            "key": {
                "id": 194,
                "expired_at": "2024-01-21 16:44:51",
                "deleted_at": null,
                "deleted_reason": null,
                "created_at": "2023-12-22T16:44:51.000000Z",
                "updated_at": "2023-12-22T16:44:51.000000Z",
                "key": "bRw1SR4NFerUTxlz.QFYma8CBiuHlNCc7",
                "order_id": 201,
                "user_id": 5,
                "encryption_key": "B6BevvpR"
            },
            "user": {
                "id": 5,
                "first_name": "shang",
                "last_name": "ha",
                "phone_number": "0948111832",
                "email": "s0ckd3@gmail.com",
                "role": "ADMIN",
                "created_at": "2023-11-04T05:48:38.000000Z",
                "updated_at": "2023-11-04T05:48:38.000000Z"
            },
            "plan": {
                "id": 7,
                "name": "DT 1K",
                "slug": "dt-1k",
                "amount": 1000,
                "type": "MONTH",
                "proxy_type": "HTTP",
                "price": 99000,
                "is_active": 1,
                "description": "Proxy Datacenter IPv4<br>\n<strong>S\u1ed1 l\u01b0\u1ee3ng: <\/strong>1000<br>\n<strong>Ng\u00e0y s\u1eed d\u1ee5ng: <\/strong>30 Ng\u00e0y<br>\n<strong>Th\u1eddi gian l\u00e0m m\u1edbi: <\/strong>2 ng\u00e0y\/l\u1ea7n<br>",
                "deleted_at": null,
                "created_at": "2023-11-06T15:52:20.000000Z",
                "updated_at": "2023-12-07T12:12:13.000000Z",
                "user_id": 5,
                "is_vip": 1
            },
            "order": {
                "id": 201,
                "total": "99000.00",
                "user_id": 5,
                "payment_id": 401,
                "created_at": "2023-12-22T16:44:51.000000Z",
                "updated_at": "2023-12-22T16:44:51.000000Z",
                "key": {
                    "id": 194,
                    "expired_at": "2024-01-21 16:44:51",
                    "deleted_at": null,
                    "deleted_reason": null,
                    "created_at": "2023-12-22T16:44:51.000000Z",
                    "updated_at": "2023-12-22T16:44:51.000000Z",
                    "key": "bRw1SR4NFerUTxlz.QFYma8CBiuHlNCc7",
                    "order_id": 201,
                    "user_id": 5,
                    "encryption_key": "B6BevvpR"
                }
            }
        },
        {
            "id": 193,
            "price": "10000.00",
            "quantity": 1,
            "amount": 100,
            "type": "MONTH",
            "proxy_type": "HTTP",
            "geo_key": "US",
            "order_id": 200,
            "plan_id": 6,
            "user_id": 5,
            "created_at": "2023-12-22T16:44:46.000000Z",
            "updated_at": "2023-12-22T16:44:46.000000Z",
            "key": {
                "id": 193,
                "expired_at": "2024-01-21 16:44:46",
                "deleted_at": null,
                "deleted_reason": null,
                "created_at": "2023-12-22T16:44:46.000000Z",
                "updated_at": "2023-12-22T16:44:46.000000Z",
                "key": "3MQy1fecQDzCMTfo.MVtGcazLbf3RT1n1",
                "order_id": 200,
                "user_id": 5,
                "encryption_key": "WbGAjR6T"
            },
            "user": {
                "id": 5,
                "first_name": "shang",
                "last_name": "ha",
                "phone_number": "0948111832",
                "email": "s0ckd3@gmail.com",
                "role": "ADMIN",
                "created_at": "2023-11-04T05:48:38.000000Z",
                "updated_at": "2023-11-04T05:48:38.000000Z"
            },
            "plan": {
                "id": 6,
                "name": "DT MINI",
                "slug": "dt-mini",
                "amount": 100,
                "type": "MONTH",
                "proxy_type": "HTTP",
                "price": 10000,
                "is_active": 1,
                "description": "Proxy Datacenter IPv4<br>\n<strong>S\u1ed1 l\u01b0\u1ee3ng: <\/strong>100<br>\n<strong>Ng\u00e0y s\u1eed d\u1ee5ng: <\/strong>30 Ng\u00e0y<br>\n<strong>Th\u1eddi gian l\u00e0m m\u1edbi: <\/strong>2 ng\u00e0y\/l\u1ea7n<br>",
                "deleted_at": null,
                "created_at": "2023-11-06T15:51:40.000000Z",
                "updated_at": "2023-12-07T12:13:16.000000Z",
                "user_id": 5,
                "is_vip": 1
            },
            "order": {
                "id": 200,
                "total": "10000.00",
                "user_id": 5,
                "payment_id": 400,
                "created_at": "2023-12-22T16:44:46.000000Z",
                "updated_at": "2023-12-22T16:44:46.000000Z",
                "key": {
                    "id": 193,
                    "expired_at": "2024-01-21 16:44:46",
                    "deleted_at": null,
                    "deleted_reason": null,
                    "created_at": "2023-12-22T16:44:46.000000Z",
                    "updated_at": "2023-12-22T16:44:46.000000Z",
                    "key": "3MQy1fecQDzCMTfo.MVtGcazLbf3RT1n1",
                    "order_id": 200,
                    "user_id": 5,
                    "encryption_key": "WbGAjR6T"
                }
            }
        }
    ]
}

```
