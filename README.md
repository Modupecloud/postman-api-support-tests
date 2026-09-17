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

## 🚀 How to Run These Tests
1. Download or clone this repository to your computer.
2. Open **Postman**.
3. Click **Import** in the top left corner.
4. Upload the `.postman_collection.json` file.
5. Click **Run Collection** to execute all tests automatically.
