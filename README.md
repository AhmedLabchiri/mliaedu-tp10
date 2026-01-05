# RestClient Android Application

## Description
This is a **RestClient Android app** that communicates with a backend server to manage bank accounts.  
It supports creating, reading, updating, and deleting accounts via **REST API** (JSON or XML).

## Features
- List all accounts (`GET /banque/comptes`)  
- Add new account (`POST /banque/comptes`)  
- Update an existing account (`PUT /banque/comptes/{id}`)  
- Delete an account (`DELETE /banque/comptes/{id}`)  
- Fully compatible with **Emulator** and **Physical Device**  
- Handles both **JSON** and **XML** responses

## Technologies Used
- **Kotlin / Java** for Android  
- **Retrofit** for API calls  
- **AndroidX** libraries  
- **Gradle** build system  

## Installation & Setup

1. **Clone the project**:

```bash
git clone https://github.com/yourusername/Restclient.git
