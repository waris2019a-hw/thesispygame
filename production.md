# Production Structure: Python Fantasy - Knight's Journey

## 1. Overview
A gamified Python learning platform where users progress through "Quests" to learn programming. The app features real-time code execution in the browser, a persistence layer via Firebase, and a fantasy-themed user interface.

## 2. Technical Stack
- **Frontend:** HTML5, Tailwind CSS (Styling), Font Awesome (Icons).
- **Python Runtime:** Pyodide (allows Python execution in the browser via WebAssembly).
- **Backend/Database:** Firebase (Firestore for data, Firebase Auth for user management).
- **Fonts:** Kanit (Thai/English), Fira Code (Monospace for code).

## 3. Core Components & UI Structure
### A. Authentication & Entry
- **Login Modal:** User registration with name and avatar selection (Wizard, Knight, Warrior, Oracle).
- **Admin Auth:** Password-protected access to administrative tools (Knight management).
- **Sign Out:** Session clearing and Firebase authentication logout.

### B. Main Interface
- **Header:** Displays user profile (avatar, name, rank), current XP, and navigation to Leaderboard/Inventory.
- **Sidebar (Journey Map):** Navigation menu for the 12 learning Quests.
- **Main Content Area:**
    - **Quest Header:** Quest tag, title, and reward item display.
    - **Learning Materials:** Knowledge scrolls (text) and embedded YouTube tutorial videos.
    - **The Forge (Code Editor):** Interactive Python editor with "Forge Code" (Run) and "Sage" (AI Analysis/Fix) capabilities.
    - **Console Output:** Real-time output of the executed Python code.
    - **Quiz Card:** Multi-phase multiple-choice questions to validate learning.

### C. Gamification Elements
- **Inventory (Armory):** A visual collection of earned items based on quest completion.
- **Progress Tracking:** Experience Points (XP) and Ranks (Novice $\rightarrow$ Squire $\rightarrow$ Knight $\rightarrow$ Grand Knight $\rightarrow$ Knight Legend).
- **Leaderboard:** Real-time ranking of the "Greatest Knights" fetched from Firestore.

## 4. Data Model (Firestore)
**Collection:** `artifacts/{appId}/public/data/knights/{uid}`
- `uid`: Unique user identifier.
- `name`: Knight's display name.
- `avatar`: Selected emoji avatar.
- `score`: Accumulated XP.
- `rank`: Current title based on score.
- `completed`: List of finished quest IDs.
- `inventory`: List of acquired items.
- `updatedAt`: Timestamp of last synchronization.

## 5. Quest Map (Curriculum)
1. **Introduction** $\rightarrow$ Golden Compass
2. **Flowchart** $\rightarrow$ Strategic Map
3. **Print** $\rightarrow$ War Horn
4. **Variables** $\rightarrow$ Travel Backpack
5. **Operators** $\rightarrow$ Calculation Abacus
6. **Conditions** $\rightarrow$ Truth Shield
7. **Loops** $\rightarrow$ Eternal Hourglass
8. **Functions** $\rightarrow$ Secret Scroll
9. **Collections** $\rightarrow$ Item Chest
10. **GUI Development** $\rightarrow$ Magic Orb
11. **Unit Testing** $\rightarrow$ Golden Magnifier
12. **Debugging** $\rightarrow$ Holy Broom
