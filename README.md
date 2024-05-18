# when-i-die-issues
[Issues] When I die

![hackathonSSST2024 drawio](https://github.com/edin-fazlic/when-i-die-issues/assets/102242061/7d5f3f27-4f99-48e2-a68b-912b6f3557b9)

Auth
  - Login / registration

Home
  - Navigation:
    - messages
    - trusted people (TP)
    - settings
    - they trust me (optional)

Messages
  - Data
    - List of messages, where each message:
      - id, text, TP list
  - Actions:
    - View list
    - Delete a message
  - Navigate
    - Message details (view single message = Edit a message)
    - Add a message

Message details (Edit)
  - Data
    - Message text
    - TP for this message (name, email, id)
  - Actions
    - Save message
    - Delete message
    - Remove TP
    - Add TP
  - Navigate
    - View all messages

TP
  - Data
    - List of TPs
      - name, email, id, count of messages
  - Actions
    - Remove TP (with warning if there are messages)
  - Navigate
    - TP details (view)
   
TP details (view)
  - Data
    - Name, last name, email, id, status (accepted, pending, rejected), messages (subject, id)
  - Navigate
    - Message details
    - View all TP
    - Edit
  - Actions
      - Remove TP

TP edit
  - Data
    - Name, last name, email, id
  - Actions
    - Save
    - Cancel
   
They trust me
  - Data

    - List of users
      - name, email, id, (their settings, if they set with confirmation)
  - Actions
    - Reject user (with warning), accept user, they died
