API Testing & Troubleshooting Portfolio (Postman)

 📌 Project Overview
This repository contains automated API test suites created using Postman to demonstrate API testing, HTTP protocol validation, and request/response troubleshooting skills for IT Technical Support and Support Engineering roles.

---

🛠️ Collection 1: 01_CRUD_Operations
* Target API: JSONPlaceholder (`https://jsonplaceholder.typicode.com`)
* **File:** `01_CRUD_Operations.postman_collection.json`

 Test Cases Covered:
* **`POST` /posts (Create):** Validated successful payload creation and verified HTTP `201 Created` status response.
* **`GET` /posts/1 (Read):** Validated data retrieval, verified HTTP `200 OK` status, and verified JSON body schema attributes (`id`, `title`, `body`).
* **`PUT` /posts/1 (Update):** Validated resource updates, verified status HTTP `200 OK`, and confirmed updated body structure.
* **`DELETE` /posts/1 (Delete):** Validated resource removal and verified HTTP `200 OK` status response.
---

## 🛠️ Collection 2: 02_Error_Handling_Tests
* **Target API:** JSONPlaceholder (`https://jsonplaceholder.typicode.com`)
* **File:** `02_Error_Handling_Tests.postman_collection.json`

### Test Cases Covered:
* **`GET` /posts/999999 (404 Not Found):** Asserts API handling when requesting non-existent records.
* **`GET` /invalid_endpoint_xyz (404 Bad Route):** Validates system fallback behavior for non-existent URI paths.
---

## 🚀 How to Run These Tests
1. Download or clone this repository to your computer.
2. Open **Postman**.
3. Click **Import** in the top left corner.
4. Upload the `.postman_collection.json` file.
5. Click **Run Collection** to execute all tests automatically.
---

## 🛠️ Collection 3: 03_Auth_And_Headers
* **Target API:** ReqRes (`https://reqres.in`)
* **File:** `03_Auth_And_Headers.postman_collection.json`

### Test Cases Covered:
* **`POST` /api/login (Success):** Validates authentication payload, verifies HTTP `200 OK`, and asserts presence of auth token.
* **`GET` /api/users/2 (Header Check):** Tests protected resource access and response policies.
* **`POST` /api/login (Missing Password):** Verifies authentication failure handling and asserts HTTP `400 Bad Request` status response.
---

## 🛠️ Collection 4: 04_Dynamic_Workflows
* **Target API:** JSONPlaceholder (`https://jsonplaceholder.typicode.com`)
* **File:** `04_Dynamic_Workflows.postman_collection.json`

### Test Cases Covered:
* **`POST` /posts (Create & Store Variable):** Generates a new resource, asserts HTTP `201 Created`, and dynamically extracts response `id` into collection scope.
* **`PUT` /posts/{{created_post_id}} (Dynamic Update):** Utilizes stored collection variable to target created resource and asserts HTTP `200 OK`.
* **`DELETE` /posts/{{created_post_id}} (Dynamic Delete):** Verifies dynamic resource cleanup and asserts HTTP `200 OK`.
