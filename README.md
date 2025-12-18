# GradePlus 📚

**GradePlus** is a collaborative educational platform designed to streamline exam preparation for students. It solves the common problem of scrambling for Previous Year Questions (PYQs) and study materials by providing a centralized hub where students can upload, access, and discuss resources collaboratively.

## 🚀 Features

### 👨‍🎓 For Students (Users)
* **Resource Hub:** Access a wide range of study materials, including PYQs, notes, and external links.
* **Integrated Viewers:** View PDFs directly within the app using advanced PDF viewing tools.
* **Subject Discussions:** Built-in chat functionality for specific subjects to discuss topics and doubts.
* **Downloads:** Save materials offline for easy access.

### 🛡️ For Moderators
* **Content Management:** Tools to add documents, links, and manage subject materials.
* **Request Handling:** View and manage user requests for new resources.

### 🔐 For Admins
* **Role Management:** Capability to add and view moderators to maintain platform quality.

## 🛠️ Tech Stack

This project is built using **Flutter** and leverages a robust set of packages for functionality and UI.

* **Framework:** Flutter (Dart)
* **State Management:** Provider
* **Backend & Database:**
  * Firebase Auth (Google Sign-In, Email/Password)
  * Cloud Firestore
  * Firebase Storage
  * Firebase Database (Realtime)
* **File Handling:**
  * `flutter_pdfview`, `advance_pdf_viewer`, `syncfusion_flutter_pdfviewer` (PDF Viewing)
  * `file_picker`, `image_picker` (File Uploads)
  * `open_file` (Opening files natively)
* **UI & Animations:**
  * `lottie` (Animations)
  * `flutter_screenutil` (Responsive Design)
  * `getwidget`, `flutter_speed_dial` (UI Components)
  * `iconsax`, `font_awesome_flutter` (Iconography)
* **Utilities:**
  * `flutter_local_notifications` (Notifications)
  * `url_launcher` (Opening external links)
  * `Youtubeer_flutter` (Video playback)
  * `flutter_secure_storage` (Secure data persistence)

## 📂 Project Structure

The project is organized into logical sections based on user roles and functionality:

```text
lib/
├── constants/         # App-wide constants
├── screens/
│   ├── admin_section/      # Admin specific screens (Add Moderator, etc.)
│   ├── moderator_section/  # Moderator tools (Add Docs, Links, Requests)
│   ├── user_section/       # Student facing screens (Home, Subjects, Chat)
│   │   ├── components/     # Reusable user widgets (PDFViewer, SideNav)
│   │   └── subjects/       # Subject-specific content (Materials, PYQs)
│   └── login/              # Authentication screens and logic
├── onboarding.dart    # Intro/Onboarding screen
└── main.dart          # Entry point
