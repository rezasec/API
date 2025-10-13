### Request Methods  
When making an HTTP call to a server, we use a request method (also called an HTTP verb) to indicate what kind of action we want to perform. These usually match the CRUD operations:

| Method | Operation |  
| ------- | ---------- |  
| **GET** | Retrieve data (Read) |  
| **POST** | Send data (Create) |  
| **PUT/PATCH** | Update data (Update) |  
| **DELETE** | Delete data (Delete) |  

- **PUT** usually replaces an entire resource.  
- **PATCH** is used for partial updates.  

Since we’re just getting books and not changing anything, we use a **GET** request. These are conventions, though—it depends on how the API was built. Always check the API documentation to confirm which method to use.

Refer to the **Postman Library API v2 docs** for examples.  

---

### Request URL  
A request also needs a URL that tells where the API call should go. It has three main parts:  

| Part | Description | Example |  
| ----- | ------------ | -------- |  
| **Protocol** | The transfer method | `https://` |  
| **Host** | Location of the server | `library-api.postmanlabs.com` |  
| **Path** | Route or resource | `/books` |  

So the full example URL is:  
`https://library-api.postmanlabs.com/books`  

Paths and full URLs like this are often called **API endpoints**.  

---

### Response Status Codes  
When the API responds, it sends a status code that shows whether the request worked or failed. For example, the Postman Library API returned **200 OK**, which means success.

Common status code categories:

| Code Range | Meaning | Example |  
| ----------- | -------- | -------- |  
| **2xx** | Success | 200 – OK, 201 – Created, 204 – No Content |  
| **3xx** | Redirection | 301 – Moved |  
| **4xx** | Client Error | 400 – Bad Request, 401 – Unauthorized, 403 – Forbidden, 404 – Not Found |  
| **5xx** | Server Error | 500 – Internal Server Error, 502 – Bad Gateway, 504 – Gateway Timeout |  

A **2xx** response means the request was successful, while **4xx** and **5xx** indicate problems on the client or server side.
