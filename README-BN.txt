LM26 ADMIN WEB — SETUP (বাংলা)
================================
ফাইল: index.html, firebase.json, .firebaserc

1) Firebase Console > Authentication > Sign-in method > Email/Password চালু করুন।
2) Authentication > Users থেকে আপনার Admin account তৈরি করুন/নিশ্চিত করুন।
3) Admin account-এর UID অবশ্যই index.html-এ থাকা configured Admin UID-এর সঙ্গে মিলতে হবে:
   B7RH4NNrrgdZpx6kRf6NvIlE8j12
4) Realtime Database Rules-এর জন্য সঙ্গে দেওয়া database.rules.json দেখুন এবং Publish করুন।
5) আপনার কম্পিউটারে Node.js ইনস্টল করে Terminal/CMD-তে:
   npm install -g firebase-tools
   firebase login
   এই ফোল্ডারে গিয়ে: firebase deploy --only hosting
6) সফল হলে Firebase Hosting URL দেখাবে।

সীমাবদ্ধতা:
- Admin password এই ফাইলে রাখা নেই; Firebase Authentication ব্যবহার হয়।
- এই dashboard শুধু PING ও SHOW_MESSAGE command queue করে।
- Android app online, signed-in এবং user consent দেওয়া থাকলে command দেখাবে।
- এটি গোপন নজরদারি, SMS/call reading, camera/mic control বা অদৃশ্য remote access করে না।
