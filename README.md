# Alchemyst AI LangChain 0.3.x Integration

## Overview

This package provides seamless integration between [Alchemyst AI](https://alchemyst.ai) and [LangChain JS 0.3.x](https://js.langchain.com/), enabling developers to leverage Alchemyst's unified context cloud within LangChain-powered applications.

**Alchemyst AI** is the context cloud for LLMs and AI Agents, purpose-built to serve as the connective tissue of your entire AI stack. It offers a unified memory layer that bridges data ingestion, context management, orchestration, inference, and deployment. By acting as a central hub for context and knowledge, Alchemyst enables your AI systems to access, share, and persist information across tools, sessions, and workflows.

With this integration, you can:

- **Aggregate and enrich data** from diverse sources, making it accessible to LLMs and agents in real time.
- **Maintain persistent, context-aware memory** that enhances reasoning, retrieval, and generation.
- **Orchestrate complex workflows** by connecting specialized frameworks, libraries, and platforms.
- **Deploy modular, scalable AI solutions** that are easy to maintain and evolve.

## Features

- **Plug-and-play context management**: Effortlessly connect LangChain memory, retrievers, and tools to Alchemyst's context cloud.
- **Unified knowledge layer**: Share context and memory across multiple agents, sessions, and workflows.
- **Real-time data ingestion**: Stream and synchronize data from external sources into your LangChain pipelines.
- **Production-ready orchestration**: Build robust, scalable AI applications with persistent context and state.

## Installation

```bash
bun install
```

## Usage

To run the integration example:

```bash
bun run index.ts
```

## Example

```typescript
import { AlchemystMemory } from "@alchemyst-ai/langchain";
import { ConversationChain } from "langchain/chains";

// Initialize Alchemyst memory
const memory = new AlchemystMemory({ apiKey: "YOUR_ALCHEMYST_API_KEY" });

// Use with LangChain ConversationChain
const chain = new ConversationChain({ memory });

const response = await chain.call({ input: "Hello, who won the world cup in 2022?" });
console.log(response);
```

## Why Use Alchemyst with LangChain?

- **Persistent, cross-session memory**: Retain knowledge across conversations and agents.
- **Unified context for orchestration**: Coordinate complex workflows with shared state.
- **Future-proof integrations**: Easily connect new tools and frameworks as your stack evolves.

## Documentation

- [Alchemyst AI Documentation](https://docs.alchemyst.ai)
- [LangChain JS Documentation](https://js.langchain.com/)

## License

MIT

---

This integration was created using `bun init` with bun v1.2.21. [Bun](https://bun.com) is a fast all-in-one JavaScript runtime.
