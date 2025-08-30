# 🚖 KGP YATRI App (Expo + Expo Router Tabs)

This project is a **React Native app built with Expo Router**.  
It features a **tab-based navigation** with screens for Home, Rides, Chat, and Profile.  

---

## 📂 Project Structure

```plaintext

app/
│── _layout.tsx         # Root layout, defines Tab Navigator
│── home.tsx            # Home screen (tab)
│── rides.tsx           # Rides screen (tab)
│── chat.tsx            # Chat screen (tab)
│── profile.tsx         # Profile screen (tab)

# Authentication
│── sign-in.tsx         # Login screen
│── sign-up.tsx         # Register screen
│── welcome.tsx         # Onboarding / welcome screen

# Ride Booking Flow
│── find-ride.tsx       # Search for rides
│── book-ride.tsx       # Book a ride
│── confirm-ride.tsx    # Confirm ride details

# APIs
│── create+api.ts       # Create ride API
│── pay+api.ts          # Payment API integration
│── driver+api.ts       # Driver-related API
│── user+api.ts         # User-related API
│── [id]+api.ts         # Dynamic ride/user API

components/
│── RideLayout.tsx      # Common ride layout wrapper
│── RideCard.tsx        # Ride item card
│── DriverCard.tsx      # Driver details card
│── CustomButton.tsx    # Reusable button
│── GoogleTextInput.tsx # Google Maps input
│── InputField.tsx      # Reusable text input
│── Map.tsx             # Map view integration
│── OAuth.tsx           # Google OAuth login
│── Payment.tsx         # Payment component

lib/
│── fetch.ts            # API fetch helpers
│── map.ts              # Google Maps utilities
│── utils.ts            # General utilities
│── auth.ts             # Auth-related utilities

constants/
│── index.ts            # App constants (API keys, values, etc.)

```

- **`_layout.tsx`** → Sets up the bottom tab navigation using Expo Router.  
- **Other screens** (`home.tsx`, `rides.tsx`, `chat.tsx`, `profile.tsx`) are linked directly to the tabs.  

---

# 🛠️ Tech Stack

- [Expo](https://expo.dev/) (React Native framework)  
- [Expo Router](https://expo.github.io/router) (file-based routing)  
- [React Navigation](https://reactnavigation.org/) (tabs & navigation under the hood)  
- TypeScript  

---

# ▶️ Getting Started

## 1. Clone the repository
```bash
git clone https://github.com/Akashkittu/kgp_yatri.git
cd kgp_yatri
```
## 2. 🔑 Environment Variables

Create a **.env** file in the root of your project and add the following:

```bash
EXPO_PUBLIC_API_KEY=your_api_key_here
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here
DATABASE_URL=your_postgres_connection_string_here
STRIPE_SECRET_KEY=your_stripe_secret_key_here
EXPO_PUBLIC_STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key_here
EXPO_PUBLIC_GOOGLE_API_KEY=your_google_api_key_here
EXPO_PUBLIC_DIRECTIONS_API_KEY=your_google_directions_api_key_here
EXPO_PUBLIC_GEOAPIFY_API_KEY=your_geoapify_api_key_here
```

## 3. Install dependencies
```bash
npm install
# or
yarn install
```

## 4. Run the app
```bash
npx expo start
```
Scan the QR code with your phone (Expo Go app) or run on an emulator.

## 📱 Features
Bottom Tab Navigation

🏠 Home  
🚘 Rides  
💬 Chat  
👤 Profile  

Organized using Expo Router’s file system-based navigation.


## 📸 Screenshots
<p align="center"><img src="https://github.com/Akashkittu/kgp_yatri/blob/main/image_2.jpg?raw=true" width="250"/> <img src="https://github.com/Akashkittu/kgp_yatri/blob/main/_image3.jpg?raw=true" width="250"/> <img src="https://github.com/Akashkittu/kgp_yatri/blob/main/image4.jpg?raw=true" width="250"/> <img src="https://github.com/Akashkittu/kgp_yatri/blob/main/image_1.jpg?raw=true" width="250"/> </p>


## 👨‍💻 Contributing

Feel free to fork this repository, create a branch, and submit a pull request for improvements.


## Contact

For any queries, feel free to reach out at [akashburnwal550@gmail.com].
