# Mind Swipe Practices

This repository contains a dynamic list of daily mindfulness practices for the **Mind Swipe** iOS app. The data is stored in a simple `JSON` format and can be updated at any time without needing to update the app.

---

## 📄 File Structure

- `practices.json`:  
  A list of 75 recommended mindful practices with properties like difficulty, category, and premium flag.

- `quotes.json`:  
  A collection of 325 inspirational quotes organized by the same categories as practices for seamless pairing.

---

## 🗂️ Practice Categories

The mindfulness practices are organized into the following categories:

| Category | Description |
|----------|-------------|
| **Breathing** | Breath-focused techniques for calm and awareness |
| **Stillness** | Meditation and quiet observation practices |
| **Focus** | Concentration and attention training exercises |
| **Compassion** | Self-kindness and loving-kindness practices |
| **Movement** | Mindful physical activities and body awareness |
| **Detox** | Digital breaks and mental decluttering |
| **Ritual** | Mindful daily activities and routines |
| **Nature** | Outdoor and nature-based mindfulness |
| **Visualization** | Guided imagery and mental exercises |
| **Gratitude** | Appreciation and thankfulness practices |
| **Senses** | Five senses awareness and grounding |
| **Work** | Workplace mindfulness and professional stress relief |
| **Productive** | Mindful productivity and task management |

---

## 📊 Practices Overview

The `practices.json` file contains **75 mindfulness practices** designed for micro-moments of presence throughout the day, complemented by **221 inspirational quotes** in `quotes.json`. Each practice includes:

- **Clear instructions** telling users exactly what to do
- **Simple language** accessible to beginners and experts alike  
- **Time-efficient** exercises (mostly 1-5 minutes)
- **Probability weighting** to favor simple, effective practices
- **Premium/free designation** for app monetization

The `quotes.json` file provides inspirational wisdom with:
- **17 quotes per category** for rich variety and reduced repetition
- **Diverse sources** from ancient wisdom to modern mindfulness
- **Perfect pairing** with practices by matching categories
- **Motivational content** to inspire and encourage users

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

## 💬 Quotes Schema

Each inspirational quote follows this structure:

```json
{
  "id": "1",
  "quote": "Breath is the bridge which connects life to consciousness, which unites your body to your thoughts.",
  "category": "Breathing"
}
```

### Quote Field Definitions

| Field      | Type   | Description                                        |
|------------|--------|----------------------------------------------------|
| `id`       | String | Unique identifier                                  |
| `quote`    | String | Inspirational quote text                           |
| `category` | String | Same categories as practices for easy pairing      |

The quotes are designed to complement the practices and can be paired by category for a complete mindful moment experience.

---

## 🔄 Updating Content

To update the practices and quotes shown in the app:

1. Edit `practices.json` and/or `quotes.json`
2. Commit and push your changes
3. The app will fetch the new data automatically (no app update required)

Both files use the same category system, making it easy to pair related content for a cohesive mindful experience.

---

## 🔗 Usage in App

The files are fetched via:

**Practices:**
```
https://raw.githubusercontent.com/fabianfreund/mindful_swipe_data/main/practices.json
```

**Quotes:**
```
https://raw.githubusercontent.com/fabianfreund/mindful_swipe_data/main/quotes.json
```

Make sure your repository is **public** so the app can access the raw data.

---

## 📥 Contribution

Feel free to fork and suggest new practices and quotes! Open a pull request with new ideas for mindful moments and inspiring wisdom ✨

---

## 🧘 About Mind Swipe

Mind Swipe is a minimalist, no-login mindfulness app that helps users build a daily habit of mindful presence. This repo powers the dynamic content in the app.
