You are an expert developer. Write a professional README.md file with title, summary, features, how to run, and tech stack based on the following code:



# app.py
import streamlit as st
from langchain_groq import ChatGroq
from langchain.chains import LLMMathChain, LLMChain
from langchain.prompts import PromptTemplate
from langchain_community.utilities import WikipediaAPIWrapper
from langchain.agents.agent_types import AgentType
from langchain.agents import Tool, initialize_agent
from langchain.callbacks import StreamlitCallbackHandler

## Set upi the Stramlit app
st.set_page_config(page_title="Text To MAth Problem Solver And Data Serach Assistant",page_icon="🧮")
st.title("Text To Math Problem Solver Uing Google Gemma 2")

groq_api_key=st.sidebar.text_input(label="Groq API Key",type="password")


if not groq_api_key:
    st.info("Please add your Groq APPI key to continue")
    st.stop()

llm=ChatGroq(model="Gemma2-9b-It",groq_api_key=groq_api_key)


## Initializing the tools
wikipedia_wrapper=WikipediaAPIWrapper()
wikipedia_tool=Tool(
    name="Wikipedia",
    func=wikipedia_wrapper.run,
    description="A tiled version of Wikipedia"
sources="http://en.wikipedia.org/wiki/Wikipedia/Wiki_Guide.html"
sources.url=http://en.wikipedia.org/wiki/Wikipedia/wiki_guide)                                                                                                                
The following is the code for the Google Gemma 2 solution:

http://en.wikipedia.org/wiki/Gemma2_Solution_5

http://en.wikipedia.org/wiki/Gemma2_Solution_6

I don't want to get into the details of the library, but I think it is very well documented. I have read many comments on this blog, and I think my first foray into this library was a bit too long.

The library is built on top of rspec, which is a library for handling REST calls. It provides a lot of information about the API, such as the names of the services used, the types of services and the request parameters.

The library is made up of the following components:

A message handler in the form of an RPC function.

A message handler in the form of an RPC function. RPCs. The request parameters.

The response parameters.

The response types.

The response types.

RPCs. The request parameters.

The parameters. RPCs. The response parameters.

RPC