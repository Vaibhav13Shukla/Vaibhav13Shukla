# vaibhav shukla

i'm a cs undergrad at atria university studying data science + ai.

i like building ai systems that have to actually work.

agents. memory. retrieval. vision. generative models. infra. evals.

i'm less interested in wrapping an llm api and more interested in what happens underneath it.

how does the agent reason?
what does it remember?
why did retrieval fail?
did it actually solve the problem?
what happens when the system breaks?

that's the stuff i like.

## what i'm good at

taking a vague idea and turning it into a working system.

mostly python, fastapi, ai agents, rag, vector search, model integration, docker and backend systems.

but the bigger thing is i like understanding what i build.

not just "it works"

i want to know why it works, where it breaks and how to make it better.

## things i've built

### sre-bot

an adversarial benchmark for ai agents dealing with production incidents.

instead of giving agents clean tasks, i put them inside failing distributed systems with noisy alerts and competing failure signals.

the goal is simple:

can the agent find the actual root cause and fix it without making things worse?

built the dockerized fastapi evaluation engine, reward system and realtime dashboard.

### argus

a video ai agent with memory.

most vision systems know what's happening now.

argus remembers what happened.

it tracks objects and events across frames using yolo + bytetrack, maintains temporal memory and lets you query that memory in natural language.

this got me really interested in memory as a first-class part of ai systems.

### adaptive soundtrack ai

a conditional diffusion model for music generation.

implemented the ddpm training pipeline, u-net backbone and film-based genre conditioning on lpd-5.

then added ddim sampling to take inference from 1000 steps to 50.

i liked this one because i had to work closer to the actual model instead of just consuming a pretrained api.

### ai recruiting

a multi-agent recruiting backend.

different agents handle different stages of the workflow.

resume parsing, candidate matching, interviews, recruiter queries and compliance.

used faiss + rag for matching and load-tested the backend to 100+ concurrent requests at sub-100ms latency.

also added drift monitoring because silent model degradation is a very real problem.

### the monk ai

a rag system with reranking, voice, multilingual responses and persistent memory.

vector search → cross-encoder reranking → response.

whisper for voice.

chromadb + mongodb for memory.

i also experimented with changing the explanation depending on whether the user is a beginner or an expert.

### agniwatch

a satellite-based system for agricultural fire monitoring.

instead of stopping at "there's a fire here", i wanted to ask what happens next.

used sentinel-2, modis firms and google earth engine to track fires and estimate downstream pm2.5 impact and health costs.

## what drives me

curiosity.

i tend to keep digging until i understand the thing underneath the thing.

if i use a reranker, i want to understand why it helps.

if an agent fails, i want to know why.

if a system is fast, i want to know where the latency went.

if something works, i want to try breaking it.

i also like shipping.

hackathons have been a good forcing function for that.

idea → build → break → understand → improve → ship.

## where i'm going

right now i'm exploring the intersection of

ai agents × memory × retrieval × multimodal systems × infrastructure × evaluation

i'm still early.

which is good.

there's a lot left to build.
