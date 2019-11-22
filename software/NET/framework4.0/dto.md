# DTO: Data Transfer Object
- Instead of sending returning the EF (Entity Framework) model, it's possible
  to define a DTO (Data Transfer Object) to return a subset of the model.
  - For example: you request a book by ID number, and you only want to return
    the author name, title, and year published instead of the id, full date
    published, publisher, price, etc.
