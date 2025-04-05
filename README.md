# AI-Quiz-Generator
---
# Below link contains source code 

https://drive.google.com/drive/folders/1f1UwPM0iprVq7CcR7U2K9JXclkCVoBOb?usp=sharing
---

# About 

The AI Quiz Generator is designed to leverage OpenAI's ChatGPT API to create customizable multiple-choice quizzes. This allows users to define the language, topic, and difficulty of the quiz, making it a versatile tool for varied educational and entertainment purposes. The application enhances user experience with a loading screen displaying random facts and an end screen featuring score-based gifs and messages.


This system implements several features to deliver an engaging quiz experience:
- **Customizable Quizzes**: Users can select the language, topic, difficulty, and number of questions.
- **Interactive Loading Screen**: Displays live response streams and random facts to keep users entertained during data retrieval.
- **Ed-style Multiple Choice Quiz**: Includes explanations and a progress bar to enhance learning.
- **Dynamic End Screen**: Features gifs, sarcastic messages, and confetti based on quiz scores.
- **Kahoot-style Audio Player**: Contains 14 tracks to entertain users during the quiz.

Technologies used include Next.js 13.4 with the new App router, Tailwind CSS, and OpenAI's `gpt-3-turbo` API. The repository also utilizes various packages like `framer-motion` for animations, `highlight.js` for syntax highlighting, `react-confetti`, `react-loader-spinner`, `react-icons`, `react-use` for the `useAudio()` hook, and `react-simple-typewriter`.For development and deployment, tools like `create-next-app` and Vercel are used. The OpenAI integration involves custom prompt engineering to ensure responses are in JSON format, optimizing the API query for the best results.

![home-page](https://github.com/user-attachments/assets/90bad36f-e947-444a-bf57-6eaf1eb72618)

## Features
- Customisable language, topic, difficulty, and number of questions
- Loading screen that displays the live response stream and random webdev/programming facts (gives you something to do as it can take around 20-30 seconds for the quiz to generate)
- Multiple choice Ed-style quiz with explanations and a progress bar
- End screen with gifs, sarcastic messages, and confetti (>= 80%) that adapt to your quiz score
- 14 track kahoot-flavored audio player (this is the real highlight, the quiz is just something to do while you're groovin :grin:)

## Tech Used

- Next.js 13.4 (using the new App router)
- Tailwind CSS
- OpenAI's `gpt-3-turbo` API

## Packages Used
- [framer-motion](https://www.framer.com/motion/) (for animations)
- [highlight.js](https://www.npmjs.com/package/highlight.js) (for syntax highlighting)
- [react-confetti](https://www.npmjs.com/package/react-confetti)
- [react-loader-spinner](https://www.npmjs.com/package/react-loader-spinner)
- [react-icons](https://react-icons.github.io/react-icons/)
- [react-use](https://github.com/streamich/react-use) (for the `useAudio()` hook)
- [react-simple-typewriter](https://www.npmjs.com/package/react-simple-typewriter)

## Tools ##
- `create-next-app` (development and building)
- Vercel (deployment)

## OpenAI Integration

A custom prompt is created by interpolating user entered form data. Crucially, the response is asked to be returned in JSON format. Light "prompt engineering" was required to ensure the response was consistently in the correct format (for example: explicitly saying what the names of the keys should be).

![prompt](https://github.com/user-attachments/assets/7200a628-24f1-482b-9e3c-b698f3d98922)

The API is queried. After playing with the available parameters, I found leaving most of them at their default setting worked well.

![api-request](https://github.com/user-attachments/assets/0ab01d75-462a-404c-937b-76d8ea74c6b2)

## Screenshots
# Loading Screen
![loading-screen](https://github.com/user-attachments/assets/e3bc0f39-3488-461a-af82-4cb3a73d1848)

# Quiz Screen
![quiz-screen](https://github.com/user-attachments/assets/eda3117a-6024-4563-bd0f-5dd6b09fd68b)

# End Screen
![end-screen](https://github.com/user-attachments/assets/aba64c63-d292-4993-9854-e6676c98a320)








