# 🎴 Sticker Tracker 🎴

Sticker Tracker is a mobile web application where the user is able to track the progress on the 2026 World Cup Official Sticker Album. The user can mark stickers as collected, search by name, sort countries, export/import album and it supports dark/light mode.


<img width="200" height="450" alt="stickertracker1" src="https://github.com/user-attachments/assets/b740547d-f463-4676-9230-54ba4a732901" />

<img width="200" height="450" alt="stickertracker2" src="https://github.com/user-attachments/assets/ceb251d1-7df7-4f0b-865d-bff6c0fd41e9" />

<img width="200" height="450" alt="stickertracker7" src="https://github.com/user-attachments/assets/59744c3b-0ccd-404e-a68a-eb3f9e8c14e1" />

<img width="200" height="450" alt="stickertracker9" src="https://github.com/user-attachments/assets/5cf7b9f9-5a74-4056-8469-af248da1412b" />


---

## ✅ Test the app ✅

- Web-app (PWA): [Test Here](https://laratastudios.com/StickerTracker-Public/)

---

## 💫 Features 💫
- Mobile-first PWA
- Real-time search and filtering
- Multiple sorting modes
- Live album statistics
- Quick navigation using flag index
- Automatic local persistence using browser storage
- Export/Import album
- Fill/Clear album for convinience
- Support light and dark mode
  


---

## 🛠️ Built With 🛠️

- React
- Vite
- JavaScript
- HTML
- CSS
- Local Storage API
- PWA technologies

---

## 💡 Important Design Decisions 💡

Throught this project I had to take multiple important decisions regarding the projects future. Some of them were:

### 🗂️Album Progression Persistency🗂️
One of the primary design goals of the application was to ensure that user never lose their collection progress. Rather than requiring user accounts or back end database, the application automatically saves the entire album state to the browser's Local Storage whenever changes are made. This allows users to close the app, refresh the page, or return days later and continue exactly where they left off. The decision to use Local Storage keeps the application lightweight, fully client-side, and functional without an internet connection after PWA installation.


### 📤Export/Import System📤
The application includes an export and import system that allows users to transfer their album progress between devices or share it with others. Instead of exporting the complete album data—which would include static information such as country names and flags—the system exports only the collection state of the stickers. This significantly reduces the size of the generated code while ensuring compatibility with future updates to the application. During import, the application reconstructs the user’s album by combining the exported collection data with the built-in album dataset. This approach produces compact shareable codes, avoids duplication of static data, and provides a simple backup mechanism without requiring cloud storage or user accounts.



### 📱Mobile Priority📱
The application was designed with a mobile-first philosophy because collecting stickers is an activity users are likely to perform while away from a computer, such as while opening packs, trading with friends, or browsing an album. Every major interface decision was made with smartphone usability in mind, including large touch targets, sticky navigation elements, quick filtering options, and efficient one-handed navigation through the country flag index. The layout also adapts to larger screens while maintaining the same intuitive experience. By prioritizing mobile usability from the beginning, the application functions naturally as a Progressive Web App that feels closer to a native mobile application than a traditional website.

---

## 🎓 What I learned 🎓

This project taught me:
- Basic and Advance React workflow
- Managing complex state updates in React
- Working with local storage API
- Balancing feature development with simplicity and usability
- Learning how PWA works
- Designing UI interactions that minimize disruption
- Implementing custom data serialization and restoration


---

## 🎯 Technical Challenges 🎯

- Handling browser limitations: Developing the application as a Progressive Web App required accounting for differences in browser behavior across platforms. Certain APIs, such as clipboard functionality, are not consistently supported on all mobile browsers and installed PWAs, particularly on iOS. To ensure a reliable experience, the application was designed with fallbacks and alternative interaction methods so that core features remain usable even when browser capabilities differ.
- Completion sort complications: One of the most challenging aspects of the project was implementing the completion-based sorting mode. A straightforward implementation would cause the list of countries to reorder immediately whenever a sticker was collected or uncollected, making the interface feel unstable and forcing users to repeatedly find their previous position. To solve this, the application separates the displayed order from the live completion calculations, updating the ordering only at appropriate moments. This preserves the intended sorting behavior while maintaining a smooth and intuitive user experience.


---

## 🔮 Future Improvements 🔮

- Support for additional sticker albums
- Cloud synchronization
- QR code to export/import
- Native mobile app versions for AppStore and Google Play
- Duplicates page
- Share duplicates list with friends


---

## ⚙️ Source Code ⚙️

The full source code is private while the project is in active development.
This repository serves as a showcase of the project, including gameplay footage, technical explanations and playable builds. 
