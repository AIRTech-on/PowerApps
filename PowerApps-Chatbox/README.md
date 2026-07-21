# 💬 PowerApps Chatbox with Modern UI/UX

A conversational interface built in **PowerApps** that transforms **Dataverse Notes** into a modern chat experience.  
Instead of binding notes to a simple gallery, this app re‑imagines them as a dynamic conversation screen — complete with chat bubbles, avatars, and timestamps.

---

## ✨ Features
- **Dataverse Notes Integration**: Comments stored in Dataverse are displayed as chat messages.
- **Gallery-based conversation flow**: Messages aligned left/right depending on sender.
- **Modern UI styling**: Rounded bubbles, avatars, timestamps for realistic chat feel.
- **Conditional formatting**: Different colors for user vs. system messages.
- **Responsive design**: Works across devices and screen sizes.

---

## 📸 Screenshots
 Screenshots are added in the screenshot folder.

---

## 🛠️ Technical Details
- **Data Source**: Dataverse `Notes` table.
- 
- **Gallery Setup**:
  - Each note becomes a gallery item styled as a chat bubble.
  - Alignment/Color/X/Y based on sender:
    If(ThisItem.CreatedBy = User().Email, Align.Right, Align.Left)
    
    If(ThisItem.CreatedBy = User().Email, RGBA(0,120,212,1), RGBA(240,240,240,1))


