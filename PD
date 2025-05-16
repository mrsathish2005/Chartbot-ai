import openai import os from dotenv import load_dotenv 

load_dotenv() openai.api_key = os.getenv("OPENAI_API_KEY") 

def get_response(user_input): try: response = openai.ChatCompletion.create( model="gpt-3.5-turbo", messages=[ {"role": "system", "content": "You are a helpful customer support assistant."}, {"role": "user", "content": user_input} ] ) return response['choices'][0]['message']['content'].strip() except Exception as e: return "Sorry, there was an error contacting the AI service." 
