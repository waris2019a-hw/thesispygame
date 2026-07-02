# Firebase Database Configuration

This document contains the Firebase configuration and utility details used in the Python Fantasy application.

## Firebase Configuration
```json
{
  "apiKey": "AIzaSyBkRS0JyVqO8l4scTBAnB93D3B7BeAAE9w",
  "authDomain": "scorestudent-f18c5.firebaseapp.com",
  "databaseURL": "https://scorestudent-f18c5-default-rtdb.asia-southeast1.firebasedatabase.app",
  "projectId": "scorestudent-f18c5",
  "storageBucket": "scorestudent-f18c5.firebasestorage.app",
  "messagingSenderId": "55893928684",
  "appId": "1:55893928684:web:fcee9b42d6b8b87df853c9"
}
```

## Database Details
- **App ID:** `python-fantasy-v1`
- **Service:** Google Cloud Firestore
- **Authentication:** Firebase Auth (Anonymous and Custom Token)

## Integrated Utilities
The application exposes the following Firebase utilities to the `window` object:

### Firestore Utils (`window.firestoreUtils`)
- `doc`, `setDoc`, `getDoc`, `getDocs`, `updateDoc`, `deleteDoc`, `collection`, `onSnapshot`, `query`, `limit`

### Auth Utils (`window.firebaseAuthUtils`)
- `signInAnonymously`, `signInWithCustomToken`, `onAuthStateChanged`, `signOut`
