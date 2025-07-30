# Mind Swipe Practices

This repository contains a dynamic list of daily mindfulness practices for the **Mind Swipe** iOS app. The data is stored in a simple `JSON` format and can be updated at any time without needing to update the app.

---

## 📄 File Structure

- `practices.json`:  
  A list of recommended mindful practices with properties like difficulty, category, and premium flag.

---

## 📦 JSON Schema

Each practice follows this structure:

```json
{
  "id": "1",
  "title": "Breathe with Awareness",
  "description": "A short practice: breathe with awareness to reconnect with presence.",
  "category": "Breathing",
  "difficulty": "easy",
  "isPremium": false,
  "probability": 0.9
}
```

### Field Definitions

| Field         | Type    | Description                                                  |
|---------------|---------|--------------------------------------------------------------|
| `id`          | String  | Unique identifier                                            |
| `title`       | String  | Name of the practice                                         |
| `description` | String  | Short explanation of the practice                            |
| `category`    | String  | Theme or context (e.g. "Breathing", "Reflection")            |
| `difficulty`  | String  | One of: `easy`, `medium`, `hard`                             |
| `isPremium`   | Boolean | Marks if the practice is premium-only                        |
| `probability` | Float   | Value between 0.0–1.0 for weighted random selection          |

---

## 🔄 Updating Practices

To update the practices shown in the app:

1. Edit `practices.json`
2. Commit and push your changes
3. The app will fetch the new data automatically (no app update required)

---

## 🔗 Usage in App

The file is fetched via:

```
https://raw.githubusercontent.com/fabianfreund/mindful_swipe_data/main/practices.json
```

Make sure your repository is **public** so the app can access the raw data.

---

## 📥 Contribution

Feel free to fork and suggest new practices! Open a pull request with new ideas for mindful moments ✨

---

## 🧘 About Mind Swipe

Mind Swipe is a minimalist, no-login mindfulness app that helps users build a daily habit of mindful presence. This repo powers the dynamic content in the app.
