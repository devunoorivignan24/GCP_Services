# GOOGLE Cloud Function

🔍 What Are Cloud Functions?
Cloud Functions are small pieces of code that run only when triggered by an event.
No servers, VMs, or containers to manage.
You write the function → deploy → Google runs it automatically.
Think of it as:
	“Write code, and Google will execute it whenever something happens.”
	
⭐ When to Use Cloud Functions
Use Cloud Functions for event-driven or small backend logic, such as:
	• 📁 File upload to Cloud Storage → process it
	• 📩 Pub/Sub message → react to it
	• 🌐 HTTP request → return a response
	• 🗂️ Firestore document changes → run logic
Great for automation, microservices, and lightweight integrations.

🔧 How Cloud Functions Work (Simple)
	1. ✍️ Write your function (Python, Node.js, Go, Java, etc.)
	2. 🎯 Choose a trigger (HTTP, Pub/Sub, Storage, Firestore…)
	3. 🚀 Deploy to Google Cloud
	4. ⚡ Google runs it automatically when triggered
	5. 💰 Pay only for actual execution time (large free tier available)

           ┌──────────────┐
           │   Event       │
           │ (HTTP / PubSub│
           │  Storage etc.)│
           └───────┬──────┘
                   │ triggers
                   ▼
          ┌────────────────────┐
          │  Cloud Function     │
          │ (your code executes)│
          └─────────┬──────────┘
                    │ outputs
                    ▼
         ┌──────────────────────┐
         │ Response / Logs /     │
         │ DB Write / Processing │
         └──────────────────────┘


