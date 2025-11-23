# GOOGLE Cloud Function

🔍 What Are Cloud Functions?

Cloud Functions are small pieces of code that run only when triggered by an event.
No servers, VMs, or containers to manage.
You write the function → deploy → Google runs it automatically.

“Write code, and Google will execute it whenever something happens.”

⭐ When to Use Cloud Functions

Use Cloud Functions for event-driven or small backend logic, such as:

📁 File upload to Cloud Storage → process it

📩 Pub/Sub message → react to it

🌐 HTTP request → return a response

🗂️ Firestore document changes → run logic

Great for automation, microservices, and lightweight integrations.

🔧 How Cloud Functions Work (Simple)

✍️ Write your function (Python, Node.js, Go, Java, etc.)

🎯 Choose a trigger (HTTP, Pub/Sub, Storage, Firestore…)

🚀 Deploy to Google Cloud

⚡ Google runs it automatically when triggered

💰 Pay only for the execution time

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


