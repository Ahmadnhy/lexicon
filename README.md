# Lexicon Novel

Advances in mobile technology have transformed the way people access information and entertainment, including the act of reading novels. Digital platforms offer convenience, accessibility, and portability that physical books cannot match. In light of this trend, the demand for novel-reading apps with modern, intuitive, and user-friendly interfaces is growing. Lexicon Novel project was developed to address this need.

## 🚀 Download
Demo App Link Download: [APK Download](https://drive.google.com/uc?export=download&id=1pp-f0zIqXFx15mnWAk4oxZRvJD20eFgP)

---

## ✨ Features

- **Modern UI/UX**: Clean, intuitive, and responsive design for an optimal reading experience.
- **Authentication**: Secure login, registration, and password recovery powered by Supabase Auth.
- **Explore & Discover**: Browse through various categories and find your next favorite story.
- **Reading Mode**: Comfortable reading interface with support for multiple chapters.
- **Library & Bookmarks**: Save novels to your personal collection for quick access.
- **Author Dashboard**: Write and publish your own stories directly through the app.
- **Admin Panel**: Comprehensive dashboard for content moderation and management.
- **Profile Customization**: Personalize your profile with avatars and bios.
- **Notifications**: Stay updated with the latest releases and updates.

---

## 🛠️ Tech Stack

- **Frontend**: [Flutter](https://flutter.dev/) (SDK ^3.7.0)
- **Backend**: [Supabase](https://supabase.com/) (Database, Auth, Storage)
- **Design**: Material Design 3
- **Icons**: Font Awesome Flutter, Cupertino Icons
- **Analytics & Charts**: FL Chart
- **Data Persistence**: Shared Preferences

---

## 📂 Project Structure

```text
lib/
├── constants/          # Application styling and theme constants
├── models/             # Data models (Novel, Chapter, Profile, Category)
├── screens/            # UI Screens (Home, Login, Admin, Reader, etc.)
├── services/           # Supabase and API logic
├── widgets/            # Reusable UI components
└── main.dart           # Application entry point and routing
```

---

## 🏁 Getting Started

### Prerequisites
- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- [Supabase Account](https://supabase.com/)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Ahmadnhy/lexicon.git
   ```

2. Navigate to the project directory:
   ```bash
   cd lexicon
   ```

3. Install dependencies:
   ```bash
   flutter pub get
   ```

4. Configure Supabase:
   Update `lib/main.dart` with your Supabase URL and Anon Key.

5. Run the application:
   ```bash
   flutter run
   ```

---

## 📊 Database Schema

### Profiles
- `id`: uuid (Primary Key)
- `full_name`: text
- `username`: text
- `avatar_url`: text
- `bio`: text
- `role`: text (admin/user)

### Novels
- `id`: bigint (Primary Key)
- `title`: text
- `author`: text
- `description`: text
- `cover_url`: text
- `published_date`: timestamp
- `category_id`: bigint (Foreign Key)
- `status`: text
- `chapter_count`: int
- `view_count`: int
- `average_rating`: float
- `total_ratings`: int

### Chapters
- `id`: bigint (Primary Key)
- `novel_id`: bigint (Foreign Key)
- `title`: text
- `content`: text
- `created_at`: timestamp

### Categories
- `id`: bigint (Primary Key)
- `name`: text
- `description`: text

---

## 🤝 Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---

**Developed by Ahmad nh👾 | [ahmadnh.is-a.dev](https://ahmadnh.is-a.dev)**