# Spanish CEFR Vocabulary Lists for Flashcard App

These JSON files contain Spanish vocabulary organized by CEFR proficiency levels, ready to use with your flashcard application.

## Files Included

1. **beginner.json** - A1-A2 level vocabulary (300+ words)
   - Basic greetings and phrases
   - Common verbs and everyday vocabulary
   - Numbers, colors, days of the week
   - Family, food, body parts
   - Essential adjectives and adverbs

2. **intermediate.json** - B1-B2 level vocabulary (300+ words)
   - More complex verbs and expressions
   - Abstract concepts
   - Academic and professional vocabulary
   - Conjunctions and discourse markers
   - Emotion and opinion vocabulary

3. **advanced.json** - C1-C2 level vocabulary (300+ words)
   - Sophisticated vocabulary
   - Academic and formal register
   - Nuanced expressions
   - Literary and technical terms
   - Complex adverbs and idiomatic phrases

## File Format

Each JSON file contains an array of vocabulary objects with this structure:

```json
{
  "spanish": "palabra",
  "english": "word",
  "pos": "noun",
  "level": "A1"
}
```

### Fields:
- **spanish**: The Spanish word or phrase
- **english**: English translation
- **pos**: Part of speech (verb, noun, adjective, adverb, phrase, etc.)
- **level**: Specific CEFR sublevel (A1, A2, B1, B2, C1, C2)

## How to Use with Your Flashcard App

### Option 1: Upload to GitHub

1. Create a GitHub account (if you don't have one): https://github.com/join
2. Create a new repository:
   - Go to https://github.com/new
   - Name it something like `spanish-vocabulary-flashcards`
   - Make it public
   - Click "Create repository"
3. Upload the three JSON files:
   - Click "uploading an existing file"
   - Drag and drop: beginner.json, intermediate.json, advanced.json
   - Click "Commit changes"
4. Get the raw file URLs:
   - Click on each file
   - Click the "Raw" button
   - Copy the URL (should look like: `https://raw.githubusercontent.com/YOUR-USERNAME/spanish-vocabulary-flashcards/main/beginner.json`)
5. Update your flashcard app:
   - Open the flashcard HTML file
   - Find the `VOCABULARY_SOURCES` object
   - Replace the URLs with your GitHub raw URLs

### Option 2: Use Kent State Web Space

If you have web space through Kent State:

1. Upload the three JSON files to your web directory
2. Make sure they're publicly accessible
3. Update the `VOCABULARY_SOURCES` URLs in your flashcard app to point to your Kent State URLs

### Option 3: Test Locally

For testing purposes, you can use local file paths, but this only works when the HTML file and JSON files are in the same directory.

## Updating the Flashcard App

In your `spanish_flashcards_dynamic.html` file, locate this section:

```javascript
const VOCABULARY_SOURCES = {
    beginner: 'YOUR-URL-HERE/beginner.json',
    intermediate: 'YOUR-URL-HERE/intermediate.json',
    advanced: 'YOUR-URL-HERE/advanced.json'
};
```

Replace the placeholder URLs with your actual file URLs.

## Customization

You can easily customize these vocabulary lists:

1. **Add more words**: Simply add new objects to the JSON array
2. **Edit translations**: Modify the "english" field
3. **Adjust levels**: Change the "level" field if you think a word belongs to a different CEFR level
4. **Add example sentences**: You could add a new field like `"example": "Esta es una oración de ejemplo"`

## Example of Adding a Word

```json
{
  "spanish": "ordenador",
  "english": "computer",
  "pos": "noun",
  "level": "A2"
}
```

## CEFR Level Guidelines

- **A1-A2 (Beginner)**: ~800-1000 words total
  - Basic communication
  - Survival vocabulary
  - Everyday situations

- **B1-B2 (Intermediate)**: ~2500-3000 words total
  - Express opinions
  - Handle most situations
  - Understand main points of clear texts

- **C1-C2 (Advanced)**: ~5000+ words total
  - Sophisticated expression
  - Understand complex texts
  - Professional and academic contexts

## Sources and Methodology

These vocabulary lists were compiled based on:
- Common CEFR vocabulary guidelines
- Frequency analysis of Spanish language usage
- Standard Spanish language learning curricula
- Institute Cervantes curriculum recommendations

## License

These vocabulary lists are provided for educational use. Feel free to modify and share them for non-commercial language learning purposes.

## Feedback and Contributions

If you'd like to add more vocabulary or suggest improvements:
1. Edit the JSON files
2. Test them in your flashcard app
3. Share your improvements with others learning Spanish

## Citation

If you use these lists in academic work or published materials, please cite appropriately:

```
Spanish CEFR Vocabulary Lists (2024). Compiled for educational flashcard application.
```

## Technical Notes

- All files are UTF-8 encoded
- JSON is valid and can be parsed by any JSON parser
- Files are optimized for web delivery (no unnecessary whitespace)
- Compatible with the flashcard application's expected format

## Contact

For questions about using these files with your flashcard app or suggestions for improvements, please reach out through your Kent State University channels.

---

**Happy Learning! ¡Buena suerte con tu español!** 🇪🇸📚
