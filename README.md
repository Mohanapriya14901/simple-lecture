🔐 SoCo Sign-In Page

This is the **Sign-In module** for the **SoCo App**, a mental well-being and social connection platform designed to help users maintain emotional health, connect with peers, and track their daily passion streaks.

🚀 Features

- Beautiful **React Native (Expo)** frontend  
- Modern **TypeScript (.tsx)** codebase  
- Responsive, mobile-first UI design  
- Integrated **backend-ready sign-in form**  
- Validation for user email & password  
- Ready to connect with **Node.js + Express + MongoDB** backend

🧩 Tech Stack

| Layer | Technology |
|-------|-------------|
| Frontend | React Native + Expo |
| Language | TypeScript (.tsx) |
| UI | Styled Components / React Native Paper |
| Backend (for integration) | Node.js + Express |
| Database (for integration) | MongoDB |

 🛠️ Installation and Setup
 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/soco-signin.git
cd soco-signin
````
2️⃣ Install dependencies

```bash
npm install
```
 3️⃣ Run the app (Expo)

```bash
npm start
```

or

```bash
expo start
```

⚙️ Folder Structure

soco-signin/
│
├── assets/              # Images, icons, and logo files
├── components/          # Reusable UI components
├── screens/
│   ├── SignInScreen.tsx # Main Sign-In UI screen
│
├── App.tsx              # Entry point for the app
├── package.json
├── tsconfig.json
└── README.md            # Project documentation
```

🔗 Backend Integration (Optional)

If you want to connect the sign-in form to your backend:

1. Set up your **backend** using **Node.js + Express + MongoDB**
2. Update your API endpoint in the sign-in function, for example:

```tsx
const handleSignIn = async () => {
  try {
    const response = await fetch("http://localhost:5000/api/auth/signin", {
      method: "POST",
      headers: { "Content-Type": "application/json" },
      body: JSON.stringify({ email, password }),
    });

    const data = await response.json();
    if (data.success) {
      alert("Login Successful!");
    } else {
      alert(data.message);
    }
  } catch (error) {
    console.error(error);
  }
};📸 UI Preview

Below is a preview of the SoCo Sign-In page 👇
![Sign-In Preview](./assets/soco-signin-preview.png)

✨ Future Enhancements

* ✅ JWT authentication
* ✅ Forgot password feature
* ✅ Google/Apple Sign-In integration
* ✅ Backend user validation with MongoDB

🧠 Inspiration

SoCo is designed to **build emotional wellness through connection and self-reflection**.
The sign-in module is the first step in making that vision real — fast, simple, and secure.
