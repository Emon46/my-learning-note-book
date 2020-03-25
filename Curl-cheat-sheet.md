# Curl-cheat-sheet

# login
```curl
$ curl -X GET -d '{ "mail": "admin@mail.com", "password": "*****" }' -H 'Content-Type: application/json'  http:/localhost:8000/login
```
# delete
```curl
$ curl -X DELETE -H "Accept: application/json" -H "Authorization: Bearer $token" http:/localhost:8000/delete-book/1
```
# post 
```curl
$ curl -X POST -H "Accept: application/json" -H "Authorization: Bearer $token" -d '{ "book_name": "himu334", "auhtor": "habh" }' http:/localhost:8000/book
```
