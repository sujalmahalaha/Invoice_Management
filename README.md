# Invoice Management System  

A **full-stack solution** for managing invoices, built with **Django REST Framework** (backend) and **React** (frontend).  

---

## 👤 Author  
**Sujal Mahalaha**  
deployment link - https://frontend-cx6rlemx5-sujal-mahalahas-projects.vercel.app/

---

## ⚙️ Features  

### Backend  
- **Models**:  
  - `Invoice`: Tracks invoice details like number, customer name, and date.  
  - `InvoiceDetail`: Includes description, quantity, unit price, and total.  
- **API**:  
  - URL: `/api/invoices/`  
  - Methods: `GET`, `POST`, `PUT`, `DELETE`  
- **Key Features**:  
  - Auto-computed totals  
  - Paginated responses  
  - Detailed error handling  

### Frontend  
- Responsive UI with features like:  
  - Paginated invoice list  
  - Create/Edit/Delete invoices  
  - Search and filter options  

---

## 🛠️ Tech Stack  
- **Frontend**: React, TailwindCSS  
- **Backend**: Django REST Framework, PostgreSQL  
- **Deployment**: Vercel  

---

## 🚀 Setup  

### Frontend  
1. Initialize the project:  
   ```bash
   npm create vite@latest frontend -- --template react
   npm install -D tailwindcss postcss autoprefixer
2. Add TailwindCSS to your CSS file:  
    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```
3. Run locally:  
    ```bash
    npm run dev
    ```  

### Backend  
1. Create the project and virtual environment:  
    ```bash
    python -m venv env
    .\env\scripts\activate
    django-admin startproject backend
    cd backend
    python manage.py startapp invoices
    ```
2. Configure PostgreSQL in `.env`:  
    ```plaintext
    DB_NAME=""
    DB_USER=""
    DB_PWD=""
    DB_HOST=""
    DB_PORT=1212
    ```
3. Run migrations and start the server:  
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    python manage.py runserver
    ```  



