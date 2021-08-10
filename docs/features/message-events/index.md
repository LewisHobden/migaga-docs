# Message Events
When a message comes in, Migaga can reply or automatically delete the message based on the content.  
This is particularly useful for filtering profanity, or a lighthearted way to respond to that "same old question" new users usually ask. 

## Concepts
- Auto-deleted messages will be posted in server logs just like normally deleted messages. 
- Message events are also fired for edited messages, so Migaga can handle those trying to be tricky. 

## Getting Started
### [Command] Setting up an auto-delete rule
`/message events add-auto-delete <contains> <strict mode>`

**Permissions**  
You must have the "Manage Messages" privilege to use this slash command. 

**Contains**  
This is the text to search the message for - Migaga searches messages loosely for this text. 

**Strict Mode**  
If strict mode is enabled, this event will only trigger if the messages contains _only_ that which you have configured.

**What to Expect**  
Once the auto delete has been set up, Migaga will begin to automatically delete messages which contain the text you provided.. even if it is edited in.  

### [Command] Setting up an auto-respond rule
`/message events add-auto-delete <contains> <response> <strict mode>`

**Permissions**  
You must have the "Manage Messages" privilege to use this slash command.

**Contains**  
This is the text to search the message for - Migaga searches messages loosely for this text.

**Response**
The text that Migaga will reply to the user with, if the text is matched. 

**Strict Mode**  
If strict mode is enabled, this event will only trigger if the messages contains _only_ that which you have configured.

**What to Expect**  
Once the auto reply has been set up, Migaga will begin to automatically reply to which contain the text you provided.  
