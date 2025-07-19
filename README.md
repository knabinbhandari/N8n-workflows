# AI Cake Creator Web App

AI Cake Creator is an interactive web app that transforms any name or occasion into a custom AI-generated cake design.

Tech Stack:
Frontend: Built using Bolt.new (Next.js-based tool) and hosted on Netlify.
Backend: Powered by n8n for workflow automation.
AI Models: Uses OpenAI for prompt generation and Replicate.com for high-quality AI image generation.

How It Works:
User Input:
A user enters a name or occasion (e.g., Sarah's Birthday) on the frontend interface.
Webhook to n8n:
The frontend sends a POST request to n8n, triggering the User Sends Request node.
Prompt Generation:
The OpenAI Chat Model dynamically creates a creative cake design prompt, e.g.,
"Generate a birthday cake image with Sarah's name, pink roses, and sparkles.
AI Image Creation:
The Replicate API takes this prompt and returns a unique cake design.
Image Delivery:
The Download Image node processes the image URL, and the Respond to Requests node sends the final cake image back to the user.

Link to Live Demo: https://calm-cendol-1a3ff2.netlify.app/

