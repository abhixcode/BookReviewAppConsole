# Book Review App (Console)

This is a console based application for the Book Review App (https://github.com/abhixcode/BookReviewApp). This is specifically designed to demo PUT and DELETE HTTP methods of the main prototype. The server is hosted in the same environment as the main application, only at a different port (5001). Both web-based and console applications point to the same MySQL DB (AWS RDS).

# External Tools

* Flask
* Flask-SQLAlchemy
* PyJWT is a Python library which allows you to encode and decode JSON Web Tokens (JWT). JWT is an open, industry-standard (RFC 7519) for representing claims securely between two parties.

# HTTP REST API

| Endpoint                    | Methods   | Action                   | Use                        |
| --------------------------- |:---------:|:------------------------:| --------------------------:|
| /register                   | GET, POST | register()               | For new user registeration |
| /login                      | GET, POST | login()                  | For user login             |
| /records/<string:bookname>  | GET       | login()                  | For retrieving reviews     |
| /records/delete/<int:id>    | DELETE    | login()                  | For deleting reviews       |
| /records/add                | POST      | login()                  | For adding reviews         |
| /records/update/<int:id>    | PUT       | login()                  | For updating reviews       |
