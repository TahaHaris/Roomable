# 📱 Roomable: Study Room Availability App

**Roomable** is a **mobile application** designed for UT Austin students to find available study rooms in real-time. Built with **React Native (Expo)** and powered by **Firebase Realtime Database**, it provides instant insights into room occupancy, helping users quickly locate ideal study spaces.

## 🚀 Key Features

* **Real-time Availability:** Track study room occupancy status instantly.
* **Intuitive Navigation:** Floor-based interface to quickly find available rooms.
* **Detailed Room Info:** View capacity, amenities, and live sensor data (distance, sound levels).
* **Mobile-First Design:** Optimized for a seamless experience on iOS and Android devices.

## 🛠️ Tech Stack

| Category      | Tools Used                             |
| :------------ | :------------------------------------- |
| **Mobile App** | React Native (Expo)                    |
| **Backend** | Firebase Realtime Database             |
| **UI/UX** | React Native components, Custom Styling |
| **Development** | Node.js, npm, Expo CLI                 |

## 📸 Screenshots

### Home Screen
![Home Screen](https://raw.githubusercontent.com/TahaHaris/Roomable/main/Roomable-Overview.png)

### Floor View
![Floor View](https://raw.githubusercontent.com/TahaHaris/Roomable/main/roomable-floor.png)

### Room Details
![Room Details](https://raw.githubusercontent.com/TahaHaris/Roomable/main/roomable-roomdetails.png)

## 💡 Project Overview & Impact

Roomable addresses the common challenge students face in finding available study spaces on a busy university campus. By leveraging real-time sensor data and a mobile-first approach, it transforms the user experience from guesswork to instant, informed decision-making. This project demonstrates the integration of IoT concepts with robust mobile application development and cloud-based backend services to solve a practical, everyday problem.

## ⚡ Quick Start

To get Roomable up and running on your local machine:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/roomable.git](https://github.com/your-username/roomable.git)
    cd roomable
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    ```
3.  **Start the development server:**
    ```bash
    npx expo start
    ```
    This will open the Expo Dev Tools in your browser. You can then scan the QR code with the Expo Go app on your phone, or press `a` for Android Emulator / `i` for iOS Simulator.

**Note:** For detailed setup of Node.js, Expo CLI, Android/iOS development environments, Firebase configuration, and troubleshooting, please refer to the [Detailed Setup & Troubleshooting Guide](FULL_SETUP_GUIDE.md).

## ☁️ Firebase Integration

Roomable connects to a Firebase Realtime Database to fetch real-time study room availability status.

* **Database URL:** `https://study-room-availability-default-rtdb.firebaseio.com`
* **Data Path:** The app listens to the `/sensor` path for room status, distance, and sound data.
* **Configuration:** Firebase connection is configured in `config/firebase.js`.
* **Mobile Configuration Files:**
    * `GoogleService-Info.plist` (for iOS) is included in the repository.
    * For Android, download `google-services.json` from your Firebase Console and place it in the project root.

## 📁 Project Structure

* `/app`: Main application code using Expo Router for navigation (`index.tsx`, `floor/[id].tsx`, `room/[id].tsx`).
* `/hooks`: Custom React hooks, including Firebase data fetching hooks.
* `/config`: Configuration files, including Firebase setup.

## ⚙️ Detailed Setup & Troubleshooting

For comprehensive instructions on installing prerequisites (Node.js, Expo CLI, Android/iOS development environments), detailed Firebase configuration, and common troubleshooting steps, please see the [FULL_SETUP_GUIDE.md](FULL_SETUP_GUIDE.md) file in this repository.

## 🤝 Contributing

1.  Fork the repository.
2.  Create your feature branch (`git checkout -b feature/amazing-feature`).
3.  Commit your changes (`git commit -m 'Add some amazing feature'`).
4.  Push to the branch (`git push origin feature/amazing-feature`).
5.  Open a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

* [Expo](https://expo.dev)
* [React Native](https://reactnative.dev)
* [Firebase](https://firebase.google.com)
