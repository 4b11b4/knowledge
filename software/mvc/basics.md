# Model
- Handles data and logic.
- Responsible for getting data from database.

# Controller
- Sits between client and model.
- Handles requests from client, retrives and sends data to and from model.
  - Provides functions such as: add, delete, get, etc.
- Uses appropriate view to present data to client.

# View
- Can have multiple views for a single model.
