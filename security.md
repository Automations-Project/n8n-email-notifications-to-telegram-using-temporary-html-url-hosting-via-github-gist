For Security Reasons we will summuray the n8n template code into text as follow:
**Workflow Summary:**
**Additional Processing:**
- **Sticky Note** (n8n-nodes-base.stickyNote)
  Details:
    - **Content**:
```plaintext
## Simple Conversion of Emails into HTML Webpages
To-do:
* Configure your GitHub credentials through `Predefined Credential Type` => `GitHub API`.
* Add your Telegram credentials by providing your `Chat ID`.
* [**Optional**] You can host this [small project](https://github.com/Automations-Project/Emails/tree/main) on your own domain using GitHub Pages.
 ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ![image](https://cdn.statically.io/gh/Automations-Project/Emails/main/iloven8n.min.svg)



 ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌  ‌ ‌ ‌  ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ‌ ![image](https://cdn.statically.io/gh/Automations-Project/Emails/main/iloven8n%E2%80%8C.min.svg)
``` 
- **Email Trigger (IMAP)** (n8n-nodes-base.emailReadImap)
**Data Fetching and Processing:**
- **Github Gist** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Save HTML content``` 

**Additional Processing:**
- **Telegram** (n8n-nodes-base.telegram)
- **Wait** (n8n-nodes-base.wait)
  Details:
    - **Notes**: ```plaintext
Delete within 3h``` 

**Data Fetching and Processing:**
- **Github Gist ‌** (n8n-nodes-base.httpRequest)
  Details:
    - **Notes**: ```plaintext
Remove HTML content``` 

**Additional Processing:**
- **Telegram ‌** (n8n-nodes-base.telegram)
