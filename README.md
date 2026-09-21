# AI Tools for Teachers - Zero-Cost RAG System
By Mr T Mahomed

**Portfolio project for AI Engineer role - No OpenAI API costs**

Live Demo: https://ai-tools-teachers-rag.vercel.app/

Tech Stack:
- PDF chunked into 62 embeddings
- all-MiniLM-L6-v2 (384 dimensions) - runs in browser via Xenova
- Supabase + pgvector for vector search
- Custom RPC: match_ai_tools()
- Client-side inference, zero server cost

This RAG answers questions from my digital product "AI Tools for Teachers".

How it works:
1. PDF -> 62 chunks -> local embeddings
2. Stored in Supabase ai_tools_embeddings table
3. User question -> embedding in browser -> similarity search

Built to prove RAG engineering without paid APIs.
