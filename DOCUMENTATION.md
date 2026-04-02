# RimaRasa — Documentation

---

## 1. Introduction

RimaRasa is a mobile-based **pantun (traditional Malay poetry) generator** developed using **Flutter**. The system is designed to help users create personalized pantun based on their emotions and personal stories using AI-powered text generation.

---

## 2. Objectives

* To generate personalized pantun from user input  
* To provide a simple and intuitive mobile interface  
* To store favorite pantun locally  
* To enable sharing of generated pantun  

---

## 3. System Architecture

The system follows a **client-server architecture**:

* **Frontend:** Flutter mobile application  
* **Backend:** AI service / API (e.g., GPT-based text generation)  

  * Processes user input  
  * Generates pantun  
  * Returns formatted text to the app  

---

## 4. Modules

### 4.1 User Input Module

* Accepts user story or emotion  
* Sends input to AI service  

### 4.2 AI Pantun Generator Module

* Processes input with AI backend  
* Generates pantun in proper rhyme and structure  
* Returns generated text to frontend  

### 4.3 Favorites Module

* Saves generated pantun locally  
* Displays user’s saved pantun  

### 4.4 Sharing Module

* Enables sharing pantun via social media or messaging apps  

---

## 5. Data Storage Design

```
favorites/
└── pantunId
├── text
├── createdAt
```


* Local storage uses **shared_preferences** to persist favorites  
* AI-generated pantun are temporary unless saved  

---

## 6. Authentication Flow (Optional)

*(If integrated with Firebase or user login)*

1. User logs in via authentication service  
2. System verifies credentials  
3. User accesses home screen and features  

---

## 7. Environment Configuration

Sensitive data, like API keys for the AI service, should be stored securely and **never hard-coded** in the app:

* AI API key  
* Optional Firebase identifiers  

This prevents exposure in public repositories.

---

## 8. Security Implementation

* `.gitignore` applied for sensitive files  
* API keys stored separately and loaded at runtime  
* Local storage for favorites is sandboxed  
* AI service endpoints are secured via API tokens  

---

## 9. Challenges

* Ensuring pantun rhyme and cultural accuracy  
* Handling AI latency for generation  
* Managing state and UI updates in Flutter  
* Storing favorites efficiently  

---

## 10. Future Improvements

* Multi-language support (Malay + English)  
* Cloud sync for favorites  
* Advanced AI model customization for pantun style  
* Offline mode for generating pantun without internet  
* Enhanced UI/UX design and animations  

---

## 11. Conclusion

RimaRasa offers a creative and AI-powered way to generate traditional Malay pantun. It demonstrates integration of Flutter mobile development with AI backend services, providing both cultural and technological value.
