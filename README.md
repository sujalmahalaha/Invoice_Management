# Invoice Management System  

A full-stack Invoice Management System with a Django REST Framework backend and React frontend.  

## Author  
**Sujal Mahalaha**  



---

## Features  

### Backend  
- **Models**:  
  1. **Invoice**: Stores invoice number, customer name, and date.  
  2. **InvoiceDetail**: Includes description, quantity, unit price, and computed line total.  

- **API**:  
  - URL: `/api/invoices/`  
  - Methods: `GET`, `POST`, `PUT`, `DELETE`  
  - Features: Validation, auto-computed totals, pagination, and detailed error messages.  

### Frontend  
- Responsive and user-friendly interface.  
- Features:  
  - Invoice list with pagination  
  - Create/Edit invoice form  
  - Delete functionality  
  - Basic search and filter options  

---

## Tech Stack  
- **Frontend**: React, Vite, TailwindCSS  
- **Backend**: Django REST Framework, PostgreSQL  
- **Deployment**: Vercel  

---

## Setup  

### Frontend  
1. Initialize the project:  
    ```bash
    npm create vite@latest frontend -- --template react
    npm install -D tailwindcss postcss autoprefixer
    npx tailwindcss init -p
    ```
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



