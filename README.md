# AI-Quiz-Generator
---
# Below link contains source code 

https://drive.google.com/drive/folders/1f1UwPM0iprVq7CcR7U2K9JXclkCVoBOb?usp=sharing
---
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








