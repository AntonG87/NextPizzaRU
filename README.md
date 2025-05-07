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

📸 Screenshots
<details> <summary>Click to expand screenshots</summary>
  
🏠 Home Page

![image](https://github.com/user-attachments/assets/4c737053-f766-415c-b4f9-285fa3d230c4)

![image](https://github.com/user-attachments/assets/3c960a47-47a8-4ba2-9b0a-3d7dcd10c980)


🔐 Login Modal

![image](https://github.com/user-attachments/assets/6cc711ba-dc75-4a62-8220-e439dfe929d9)

![image](https://github.com/user-attachments/assets/53f327db-2d3d-4ecc-9c30-043bef085c7c)


🛒 Cart

![image](https://github.com/user-attachments/assets/2b7ffbf7-74cd-4459-870e-2c0a1e48bc71)

![image](https://github.com/user-attachments/assets/1a7366b9-6c4c-4765-b6dc-cb21de11d542)


🍕 Modal Choose

![image](https://github.com/user-attachments/assets/4eff4c7a-9d1e-43c8-9641-1e0bb26ad8da)

![image](https://github.com/user-attachments/assets/f8b498b5-3ec5-451f-9272-8d4bf1297331)

![image](https://github.com/user-attachments/assets/358099af-3110-4725-b588-dbaa6183d73e)


✅ Filters 

![image](https://github.com/user-attachments/assets/9a5d73a9-edff-4551-b327-04e6fcf87872)


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

---
## 📁 Folder Structure
```bash
├── app/                         # Next.js App Router pages and layout
│   ├── (checkout)/             # Checkout route and layout
│   ├── (dashboard)/            # Admin dashboard route and layout
│   ├── (root)/                 # Root routes
│   │   ├── @modal/            # Modal UI and logic
│   │   ├── not-auth/          # Pages for unauthorized users
│   │   ├── product/           # Product details
│   │   └── profile/           # User profile section
│   ├── api/                   # API route handlers and styles
│   ├── globals.css            # Global styles
│   └── layout.tsx             # Root layout
│
├── @types/                     # Global and third-party TS type declarations
│   ├── next-auth.d.ts
│   ├── prisma.ts
│   └── yookassa.ts
│
├── prisma/                     # Prisma schema, client, and seed
│   ├── migrations/
│   ├── constants.ts
│   ├── prisma-client.ts
│   ├── schema.prisma
│   └── seed.ts
│
├── public/                     # Static assets
│   └── assets/
│       └── logo.png
│
├── shared/                     # Shared logic and reusable modules
│   ├── components/            # Reusable UI components
│   │   ├── shared/
│   │   └── ui/
│   ├── constants/             # Constant values and validation schemas
│   │   ├── auth-options.ts
│   │   ├── checkout-form-schema.ts
│   │   └── pizza.ts
│   ├── hooks/                 # Custom React hooks
│   │   ├── use-cart.ts
│   │   ├── use-filters.ts
│   │   ├── use-ingredients.ts
│   │   ├── use-pizza-options.ts
│   │   └── use-query-filters.ts
│   ├── lib/                   # Helper functions and utilities
│   │   ├── calc-cart-item-total-price.ts
│   │   ├── calc-total-pizza-price.ts
│   │   ├── creat-payment.ts
│   │   ├── find-or-create-cart.ts
│   │   ├── find-pizzas.ts
│   │   ├── get-available-pizza-sizes.ts
│   │   ├── get-cart-details.ts
│   │   ├── get-cart-item-details.ts
│   │   ├── get-pizza-details.ts
│   │   ├── get-user-session.ts
│   │   ├── send-email.ts
│   │   └── update-cart-total-amount.ts
│   ├── services/              # API clients and DTOs
│   │   ├── dto/
│   │   │   └── cart.dto.ts
│   │   ├── api-client.ts
│   │   ├── auth.ts
│   │   ├── cart.ts
│   │   ├── constants.ts
│   │   ├── ingredients.ts
│   │   ├── instance.ts
│   │   ├── products.ts
│   │   └── stories.ts
│   └── store/                 # Zustand stores
│       ├── cart.ts
│       ├── category.ts
│       └── index.ts
│
├── .env                        # Environment variables
├── .gitignore                  # Ignored files and folders
├── next.config.mjs             # Next.js config file
├── tailwind.config.ts          # TailwindCSS config
├── postcss.config.mjs          # PostCSS config
├── tsconfig.json               # TypeScript configuration
└── package.json                # Project dependencies and scripts
```

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
