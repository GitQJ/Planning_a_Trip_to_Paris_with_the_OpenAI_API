# Planning_a_Trip_to_Paris_with_the_OpenAI_API
Use OpenAI's powerful API to answer questions about tourist attractions in Paris.

## AI Paris Travel Guide: Multi-Turn Chatbot with OpenAI Chat API & Prompt Design | Python, LLMs

Built a multi-turn travel guide chatbot with the OpenAI Chat Completions API. A system prompt sets the guide's persona, and it answers Paris tourist questions while keeping the full conversation history in context.

# CONTEXT
A tourism company scenario: give clients a virtual Parisian expert for common questions about landmarks and getting around. The brief required consistent, concise answers.

# MY ROLE
I wrote the system prompt, built the message structure and implemented the conversation loop.

# WHAT I DID
• Set up the OpenAI client and model (gpt-4o-mini) with the API key kept in an environment variable
• Wrote a system message to define the assistant's role and tone (comprehensive AI-powered Parisian travel guide)
• Structured the conversation as a list of role/content dictionaries (system, user, assistant)
• Looped over 3 pre-defined questions (driving distance Louvre to Eiffel Tower, location of the Arc de Triomphe, must-see Louvre artworks), appending each reply to the history so follow-ups keep context
• Set temperature 0.0 for repeatable answers and max_tokens 100 to keep responses short

# RESULTS
• Working conversation loop returning an answer for each question (e.g.: The distance from the Louvre Museum to the Eiffel Tower is approximately 3 miles (about 5 kilometers) when driving. However, travel time can vary depending on traffic conditions. Typically, it takes around 15 to 30 minutes to drive between the two landmarks.)
• Consistent, concise output across runs thanks to temperature 0.0
• Answers cut off at the 100-token limit and were relevant in terms of insights after recheck

# TECH STACK
Python, OpenAI API (Chat Completions), prompt engineering
