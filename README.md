# SpeakStep — updated GitHub files

- Login screen before practice. Demo credentials: user ID `ishashah`, password `isha12shah`.
- Short sentences first, gradually increasing in complexity. Student name is not repeated in every sentence.
- Gujarati meaning and an example for each key word are shown before speaking.
- Browser speech playback, audio recording, playback and approximate transcript feedback.
- 60-day access window starts on first successful login in this browser.
- There is no daily practice limit. The learner can practise as much as they want during the 30-day access period.

## Important security note
This is a static front-end demo. Credentials stored in `app.js` are visible to anyone who can access the public GitHub source, and browser storage can be modified or cleared. Do not use this as real authentication. For a real launch, implement server-side authentication, secure password hashing, and server-side access timing.

## Publish
Upload all four files to the repository root. In GitHub, open Settings → Pages → Deploy from a branch, choose `main` and `/(root)`, then save. Use the HTTPS URL in Chrome or Edge and allow microphone access.

## Speech feedback limitations
The app compares browser speech-recognition text to the sentence. It cannot reliably score individual sounds, accent, or fluency. For true pronunciation assessment, connect a speech assessment service through a backend.

Progress and the start date are stored in local browser storage. Audio is not uploaded to your server by this code; browser speech recognition behavior depends on the browser vendor.
