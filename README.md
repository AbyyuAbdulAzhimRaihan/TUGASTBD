# TUGASTBD
# API
API is available. Built using python and flask and psycopg2

| Business Case                                               | URL                                     | Method | Arguments              |
|-------------------------------------------------------------|-----------------------------------------|--------|------------------------|
| Add book order information (using TCL)                      | localhost:5000/order                    | POST   | isbn                   |
| Aggregate branch revenue                                    | localhost:5000/branch/revenue           | GET    | -                      |
| Aggregate book stock per branch                             | localhost:5000/branch/stock             | GET    | -                      |
| See information about manager for each branch location      | localhost:5000/manager_branch           | GET    | -                      |
| Add a book to a user’s wishlist                             | localhost:5000/wishlist                 | POST   | isbn, userid           |
| Change book or user information about a wishlist            | localhost:5000/wishlist/[userid]        | PUT    | isbn, userid           |
| Change user’s password (forgot password usecase)            | localhost:5000/user/[userid]            | PUT    | new_pass, userid       |
| Delete a user (users have the rights to be forgotten)       | localhost:5000/user/[userid]            | DELETE | userid                |
| Search books, authors, or publishers by keywords            | localhost:5000/search_books?search_term=[keyword] | GET    | keyword               |
