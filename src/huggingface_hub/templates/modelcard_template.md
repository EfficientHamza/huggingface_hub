from transformers import pipeline

chatbot = pipeline("conversational", model="facebook/blenderbot-400M-distill")

conversation = chatbot("Hello! How can I assist you?")
print(conversation)
from transformers import pipeline

chatbot = pipeline("text-generation", model="microsoft/DialoGPT-medium")

response = chatbot("What are the benefits of AI chatbots?", max_length=100)
print(response)
