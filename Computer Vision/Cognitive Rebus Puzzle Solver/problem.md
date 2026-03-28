# Problem Definition: Visual Rebus Puzzle Decoding

## 📖 Overview
You are given a collection of visual rebus puzzles and must decode each one into its corresponding English word or phrase. Rebus puzzles combine images, text, numbers, and spatial arrangements to represent words creatively through visual wordplay. 

This challenge tests the model's ability to perform **visual-linguistic reasoning**—interpreting visual patterns and transforming them into language through non-literal, creative problem-solving.

## 🗄️ Dataset Specifications

### General Domain
* **Domain:** Visual puzzle solving / Visual wordplay
* **Task:** Decode rebus puzzles into English phrases
* **Format:** Image-to-text generation

### Image Format
* **Format:** `.PNG` images
* **Resolution:** Variable (typically ranging from 400x400 to 800x800 pixels)
* **Color Space:** RGB 
* **Content:** Visual puzzles combining text, numbers, shapes, and symbols.

## 🧩 Puzzle Archetypes
The dataset contains puzzles that utilize various creative techniques. The solving architecture must be able to recognize and reason through the following spatial and semantic relationships:

| Technique | Example Visual | Target Solution |
| :--- | :--- | :--- |
| **Number Substitution** | "4 GET IT" | "Forget it" |
| **Compound Splitting** | "BREAK + FAST" | "Breakfast" |
| **Spatial Arrangement** | "ONCE" above "UPON" above "A" above "TIME" | "Once upon a time" |
| **Count-based** | "POT" + eight "O" shapes | "Potatoes" |
| **Orientation** | Rotated or reversed text | "No idea" (upside down) |
| **Size Relationships** | Large "MAN" over small "AGE" | "Manage" |

---

## 🎯 Evaluation Metrics
*(Note: Define how the solution is scored here)*
* **Primary Metric:** Exact Match Accuracy (case-insensitive string matching).
* **Secondary Metric:** Levenshtein Distance (to account for minor spelling variances or missing articles like "a" or "the").