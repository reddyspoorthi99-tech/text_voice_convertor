# 🔊 Text → Audio Converter

A simple web application that converts text into speech using the browser's built-in **Speech Synthesis API**. Users can paste or type any text and select a voice to listen to it in audio form.

---

## Features

- Convert any text to speech directly in the browser.  
- Select from multiple available voices.  
- Highlights female voices with a 🌸 icon.  
- Automatically splits large texts into manageable chunks for smooth reading.  
- Displays live status updates while speaking.  

---

## Technologies Used

- **HTML5** – for structure.  
- **CSS3** – for styling.  
- **JavaScript** – for text-to-speech functionality using `SpeechSynthesis`.  

---

## How to Use

1. Clone or download this repository.  
2. Open the `index.html` file in your browser.  
3. Paste or type the text you want to convert into the textarea.  
4. Choose a voice from the dropdown menu.  
5. Click **Convert to Audio**.  
6. Listen as the text is read aloud.  

---

## Code Overview

- **`populateVoices()`** – Fetches all available voices and populates the dropdown.  
- **`speakChunk(chunk, voice, rate)`** – Reads a chunk of text aloud with the selected voice.  
- **`convertText()`** – Handles splitting large texts into chunks, selecting the voice, and reading all chunks sequentially.  

---

## Notes

- Works best in modern browsers like Chrome, Edge, or Firefox.  
- Voice availability may vary depending on your operating system and browser.  
- Large texts are automatically split to avoid speech synthesis limits (~2000 characters per chunk).  

