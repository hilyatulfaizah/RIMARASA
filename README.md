# RimaRasa 

RimaRasa is a Flutter mobile application that generates **pantun** (traditional Malay poetry) based on the user's emotions and personal story, powered by AI.

---

## Overview

RimaRasa allows users to input their emotions or personal stories, and then generates personalized **pantun** using AI. This project demonstrates the integration of natural language processing with mobile development, offering a creative and culturally meaningful experience.

---

## Features

### 👨‍💻 User Features

- Generate pantun based on user input (story or mood)  
- Save generated pantun to favorites  
- Share pantun via social media or messaging apps  
- User-friendly, intuitive Flutter interface  

---

## Tech Stack

- **Framework:** Flutter (Dart)  
- **AI Backend:** OpenAI / GPT-based text generation  
- **State Management:** `setState` (StatefulWidget)  
- **Local Storage:** `shared_preferences`  
- **Optional:** Firebase (for user management or cloud storage)

---

Please refer to `DOCUMENTATION.md` for full details.

---
## Project Structure

```id="e1m9zp"
lib/
├── main.dart
├── home_screen.dart
├── pantun_generator.dart 
├── favorites_screen.dart 
├── models/ 
│ └── pantun_model.dart
├── services/ 
│ └── ai_service.dart
└── widgets/ 
├── pantun_card.dart
└── input_form.dart

```

---

## Getting Started

### Prerequisites

- Flutter SDK ≥ 3.4.3  
- Dart ≥ 3.4.3  
- Android Studio or VS Code with Flutter extension  
- (Optional) API key for AI backend

### Installation

```bash
git clone <repo-url>
cd RimaRasa
flutter pub get
flutter run
