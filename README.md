# 🍕 NextPizza – Fullstack Pizza Ordering App

Welcome to **NextPizza**, a modern and full-featured pizza ordering application built with:

- **Next.js 13 App Router**
- **TypeScript**
- **Prisma (ORM)**
- **NextAuth.js (Authentication)**
- **Tailwind CSS**

---

## 🧾 About the Project

This project was originally built while following a 24-hour Russian-language course on YouTube. I actively coded along for the first half and later continued by analyzing the structure and key features on my own, such as authentication and database integration. Many parts were improved or refactored into my own style and ideas.

It became my main **pet project**, where I practiced building a scalable fullstack app with a clean architecture.

> The original version was developed in a **private repository**. For transparency, I uploaded the final version to this public repo. That's why all commits appear close in time.

---

## 🧠 Features

- ✅ Product catalog with real-time filtering and sorting  
- 🧀 Filter by dough type, size, price, and ingredients  
- 🔍 Product search  
- 🔐 Secure authentication via email, GitHub, or Google  
- 🛒 Cart system with price calculation  
- ⚡ Modern UI with fully responsive layout  
- 🌐 Clean file structure and modular approach  

---

## 📁 Folder Structure
├── app/ # Application routes (Next.js App Router)
├── prisma/ # Prisma schema, migrations, and seed
├── public/ # Static files (images, favicons, etc.)
├── shared/ # Reusable UI components, hooks, lib
├── @types/ # Custom TypeScript types

---
📸 Screenshots
<details> <summary>Click to expand screenshots</summary>
🏠 Home Page

🔐 Login Modal

</details>

--- 

🌍 Language Note
Even though the original tutorial was in Russian, this project is fully accessible to English and Hebrew-speaking developers. The UI is visually clear and uses universally understood design patterns.

🤝 Acknowledgements
This project was inspired by a YouTube course but heavily adapted, modified, and expanded independently to serve as a showcase of fullstack skills using the modern Next.js stack.

---

📬 Contact
If you'd like to connect or give feedback, feel free to reach out via LinkedIn or open an issue here on GitHub.

---
## 💻 Getting Started

Follow these steps to run the project locally:

```bash
git clone https://github.com/AntonG87/next-pizza-evelson.git
cd next-pizza-evelson
npm install
npx prisma generate
npx prisma migrate dev --name init
npm run dev

---

