<p align="center"><!-- awesome:hero --><img src=".github/assets/hero.gif" width="100%" alt="Animated isometric scene: a pink model orb sends UI blocks (a card, a chart, a button row and a toggle field) onto an empty app panel, where they assemble, reshuffle into new layouts and fly home."><!-- /awesome:hero --></p>

<!-- awesome:title --><h1 align="center">Awesome Generative UI</h1><!-- /awesome:title -->

<p align="center"><!-- awesome:tagline -->Frameworks, protocols and UI kits for interfaces that an AI model renders at runtime inside your own app.<!-- /awesome:tagline --></p>

<!-- awesome:badges -->
<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <a href="contributing.md"><img src="https://img.shields.io/badge/PRs-welcome-F472B6" alt="PRs welcome"></a>
  <a href="https://github.com/ianwieds/awesome-generative-ui/commits/main"><img src="https://img.shields.io/github/last-commit/ianwieds/awesome-generative-ui?color=F472B6" alt="Last commit"></a>
</p>
<!-- /awesome:badges -->

Generative UI is interface that an AI model picks, composes or writes while your app runs, instead of a screen a developer fixed in advance. This list covers the protocols, frameworks, renderers, UI kits, examples and research for building it into your own app.

## Contents

- [Protocols and specs](#protocols-and-specs)
- [Frameworks and SDKs](#frameworks-and-sdks)
- [A2UI renderers and tools](#a2ui-renderers-and-tools)
- [UI kits for AI apps](#ui-kits-for-ai-apps)
- [Streaming renderers](#streaming-renderers)
- [Agent framework support](#agent-framework-support)
- [Examples and demos](#examples-and-demos)
- [Research](#research)
- [Guides and reading](#guides-and-reading)
- [Contributing](#contributing)

## Protocols and specs

- [A2UI](https://github.com/a2ui-project/a2ui) - Declarative JSON format from Google for agents to request native components a client renders.
- [Adaptive Cards](https://github.com/microsoft/AdaptiveCards) - Microsoft JSON card format that bots and agents send for host apps to render natively.
- [AG-UI](https://github.com/ag-ui-protocol/ag-ui) - Event protocol that streams agent messages, tool calls and shared state to a front end.
- [MCP Apps](https://github.com/modelcontextprotocol/ext-apps) - Official MCP extension and SDK for tools that return interactive HTML UI to the host.
- [MCP-UI](https://github.com/MCP-UI-Org/mcp-ui) - SDKs for sending UI resources over MCP and rendering them in a client app.
- [OpenUI](https://github.com/thesysdev/openui) - Thesys spec and runtimes for OpenUI Lang, a compact streaming language for component trees.

## Frameworks and SDKs

- [AgenticGenUI](https://github.com/vivek100/AgenticGenUI) - Library of 40+ React components an agent can render in chat, built to work with CopilotKit.
- [AI SDK](https://github.com/vercel/ai) - Vercel TypeScript toolkit that renders typed tool results as React, Vue or Svelte components.
- [Chainlit](https://github.com/Chainlit/chainlit) - Python framework for chat apps where the backend sends custom UI elements mid-conversation.
- [CopilotKit](https://github.com/CopilotKit/CopilotKit) - Frontend stack for in-app agents with tool-based, declarative and open-ended generative UI.
- [COSUI](https://github.com/baidu/cosui) - Baidu UI protocols, render SDKs and San components for model-driven markdown and JSON UI.
- [Generative UI for Expo](https://github.com/darkresearch/generative-ui) - React Native streaming markdown renderer that injects components as the model writes.
- [GenUI SDK](https://github.com/opentiny/genui-sdk) - OpenTiny toolkit for embedding generated interfaces in Vue and Angular apps.
- [GenUI SDK for Flutter](https://github.com/flutter/genui) - Builds screens from your own Flutter widget catalog and sends UI state back to the agent.
- [Hashbrown](https://github.com/liveloveapp/hashbrown) - Angular and React framework that lets a model render your components from the browser.
- [json-render](https://github.com/vercel-labs/json-render) - Vercel Labs framework where models emit JSON limited to a catalog of your components.
- [mdocUI](https://github.com/mdocui/mdocui) - Lets a model drop Markdoc tags for charts, forms and cards inline with streamed markdown.
- [Next Gen UI Agent](https://github.com/RedHat-UX/next-gen-ui-agent) - Red Hat agent that turns other agents' data into cards, tables and charts in the chat.
- [Prefab](https://github.com/PrefectHQ/prefab) - Python DSL with 100+ components that agents or people use to declare UIs, rendered in React.
- [Superinterface](https://github.com/supercorp-ai/superinterface) - React components and hooks for assistant-driven chats and wizards inside your app.
- [Tambo](https://github.com/tambo-ai/tambo) - React SDK where you register components and the agent picks them and streams their props.
- [Thesys C1](https://www.thesys.dev/) - Hosted API that answers prompts with live UI components instead of plain text.
- [Vendo](https://github.com/runvendo/vendo) - Embedded agent that builds views and micro-apps for your users in a sandboxed part of your product.

## A2UI renderers and tools

- [A2UI Bridge](https://github.com/southleft/a2ui-bridge) - React adapters that render A2UI messages with the component library you already use.
- [A2UI Composer](https://github.com/a2ui-project/composer) - Client-side workbench to author, preview and debug A2UI surfaces live.
- [A2UI Debugger](https://github.com/mgechev/a2ui-debugger) - Logs agent-to-client A2UI messages, shows surface state and steps back in time.
- [A2UI for Rails](https://github.com/vicentereig/a2ui-rails) - Rails renderer that streams A2UI screens with Turbo Streams, driven by DSPy.rb.
- [A2UI SDK](https://github.com/easyops-cn/a2ui-sdk) - Community React renderer for the standard A2UI catalog, built on shadcn/ui.
- [a2ui-4k](https://github.com/Contextable/a2ui-4k) - A2UI rendering engine for Kotlin Multiplatform.
- [A2UI-Android](https://github.com/lmee/A2UI-Android) - Jetpack Compose renderer that turns A2UI messages into native Android views.
- [a2ui-react](https://github.com/zhama-ai/a2ui-react) - React implementation of the A2UI protocol for agent-generated interfaces.
- [a2ui-react-native](https://github.com/sivamrudram-eng/a2ui-react-native) - Renders A2UI surfaces as React Native components.
- [a2ui-swift](https://github.com/BBC6BAE9/a2ui-swift) - Swift SDK for rendering A2UI generative UI on Apple platforms.
- [a2ui-vue](https://github.com/shawnwang15/a2ui-vue) - Vue 3 renderer that lets agents draw interactive A2UI surfaces.
- [A2UI.Blazor](https://github.com/xuzeyu91/A2UI.Blazor) - .NET implementation of the A2UI protocol for Blazor apps.
- [AGenUI](https://github.com/AGenUI/AGenUI) - Native A2UI SDK with streaming rendering for iOS, Android and HarmonyOS.
- [Generative MUI](https://github.com/yessGlory17/generative-mui) - Renders A2UI output as Material UI components inside your own theme.
- [Maps Agentic UI Toolkit](https://github.com/googlemaps/a2ui) - Google Maps components and handlers that agents show through A2UI.
- [Rust A2UI](https://github.com/Liangdi/a2ui) - Rust A2UI with terminal and desktop renderers for ratatui, egui, Iced and more.

## UI kits for AI apps

- [Agentic UI](https://github.com/antdigital-ai/agentic-ui) - Ant Design components that show agent reasoning steps, tool calls and task progress.
- [Agents Kit](https://github.com/agents-ui/agents-kit) - Copy-in React components for chat, voice, tool approvals and generated results.
- [AI Elements](https://github.com/vercel/ai-elements) - Vercel shadcn/ui registry of message, reasoning and tool output components for the AI SDK.
- [AI Elements Vue](https://github.com/vuepont/ai-elements-vue) - Vue port of AI Elements built on shadcn-vue.
- [Ant Design X](https://github.com/ant-design/x) - Ant Design React kit for AI chat, prompts, thought chains and agent output.
- [assistant-ui](https://github.com/assistant-ui/assistant-ui) - React primitives for AI chat that render tool calls as your own components.
- [chat-ui](https://github.com/run-llama/chat-ui) - LlamaIndex React components for LLM chat with custom widgets for tool and event data.
- [ChatKit](https://github.com/openai/chatkit-js) - OpenAI embeddable chat UI with streaming and widgets the agent can render.
- [Expo AI Elements](https://github.com/muratcakmak/expo-ai-elements) - React Native chat components for streaming markdown, reasoning traces and tool calls.
- [GAIA UI](https://github.com/theexperiencecompany/gaia-ui) - Copy-in React components for building AI agent interfaces.
- [GPT-Vis](https://github.com/antvis/GPT-Vis) - AntV charts a model describes in its output and the app renders.
- [prompt-kit](https://github.com/ibelick/prompt-kit) - shadcn/ui components for prompts, messages, reasoning and tool output.
- [Svelte AI Elements](https://github.com/SikandarJODD/ai-elements) - Svelte port of AI Elements on shadcn-svelte.
- [Widgets](https://github.com/Gan-Tu/Widgets) - Schema-driven widget renderer for chat UIs, an open alternative to ChatKit widgets.

## Streaming renderers

- [htmlstream](https://github.com/Alphanimble/htmlstream) - Streams model-written HTML into the page as it arrives, in place of markdown.
- [llm-ui](https://github.com/richardgill/llm-ui) - React library that parses streamed LLM output and renders custom blocks smoothly.
- [markstream-vue](https://github.com/Simon-He95/markstream-vue) - Streaming markdown renderers for Vue, React, Svelte and Angular with diagrams and math.
- [Streamdown](https://github.com/vercel/streamdown) - Vercel drop-in react-markdown replacement that handles unfinished streamed markdown.
- [swift-artifact](https://github.com/1amageek/swift-artifact) - SwiftUI library that renders LLM artifact blocks such as tables, code and SVG in chat.
- [vue-stream-markdown](https://github.com/jinghaihan/vue-stream-markdown) - Vue component for rendering markdown as it streams from an LLM.

## Agent framework support

- [AG2 with CopilotKit](https://docs.copilotkit.ai/ag2/) - Connects AG2 agents to CopilotKit front ends over AG-UI.
- [Agno AG-UI](https://docs.agno.com/agent-os/interfaces/ag-ui/introduction) - Exposes Agno agents over AG-UI so AG-UI front ends can render them.
- [Amazon Bedrock AgentCore AG-UI](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/runtime-agui.html) - Runs AG-UI agent servers on AgentCore Runtime.
- [CrewAI with CopilotKit](https://docs.copilotkit.ai/crewai-flows) - Connects CrewAI flows to CopilotKit front ends over AG-UI.
- [Google ADK AG-UI](https://google.github.io/adk-docs/integrations/ag-ui/) - Connects ADK agents to AG-UI clients for chat and generative UI.
- [LangGraph generative UI](https://docs.langchain.com/langsmith/generative-ui-react) - Lets LangGraph nodes push React components to the client.
- [LlamaIndex with CopilotKit](https://docs.copilotkit.ai/llamaindex/) - Connects LlamaIndex agents to CopilotKit front ends over AG-UI.
- [Mastra with CopilotKit](https://mastra.ai/guides/build-your-ui/copilotkit) - Mastra guide for serving agents to a CopilotKit front end.
- [Microsoft Agent Framework AG-UI](https://learn.microsoft.com/en-us/agent-framework/integrations/ag-ui/) - Hosts Agent Framework agents behind AG-UI endpoints for web clients.
- [Pydantic AI AG-UI](https://ai.pydantic.dev/ui/ag-ui/) - Serves Pydantic AI agents as AG-UI apps with tools and shared state.
- [Strands Agents with CopilotKit](https://docs.copilotkit.ai/aws-strands) - Connects AWS Strands agents to CopilotKit front ends over AG-UI.

## Examples and demos

- [AG-UI Dojo](https://dojo.ag-ui.com/) - Live demos of AG-UI features such as tool-based generative UI across agent frameworks.
- [Agent Chat UI](https://github.com/langchain-ai/agent-chat-ui) - LangChain Next.js chat app for any LangGraph agent, with generative UI support.
- [Chatbot](https://github.com/vercel/chatbot) - Vercel Next.js chatbot template built on the AI SDK.
- [Flutter Hatcha](https://github.com/gskinnerTeam/flutter-hatcha-app) - Party-planning agent built with Flutter GenUI and Google ADK.
- [Gemini Chatbot](https://github.com/vercel-labs/gemini-chatbot) - Generative UI chatbot built with the AI SDK and Gemini.
- [Generative UI examples](https://github.com/CopilotKit/generative-ui) - CopilotKit examples for AG-UI, A2UI and MCP Apps side by side.
- [Generative UI Playground](https://github.com/CopilotKit/generative-ui-playground) - One app to try static, declarative and open-ended generative UI.
- [Generative UI Widget](https://github.com/thesysdev/genui-widget) - Thesys chat widget that renders forms, charts and cards for LangGraph or n8n bots.
- [Learnify](https://github.com/ahmedfahim21/Learnify) - Agentic tutor that builds each lesson as generated interactive UI.
- [Morphic](https://github.com/miurla/morphic) - AI answer engine that shows its results with generated UI.
- [Open AG-UI Canvas](https://github.com/ag-ui-protocol/open-ag-ui-canvas) - Research, planner and haiku canvas demos of the AG-UI protocol.
- [Open Generative UI](https://github.com/CopilotKit/OpenGenerativeUI) - CopilotKit showcase where an agent draws charts, 3D scenes and widgets in sandboxed iframes.
- [partialupdate](https://github.com/philholden/partialupdate) - Multi-user chat where the bot edits its own HTML, CSS and JavaScript.

## Research

- [Efficient Personalization of Generative User Interfaces](https://arxiv.org/abs/2604.09876) - Paper and dataset on learning user preferences from feedback on generated UIs.
- [Generative Interfaces for Language Models](https://arxiv.org/abs/2508.19227) - Paper where LLMs answer queries with generated interactive UIs instead of text.
- [Generative UI: LLMs are Effective UI Generators](https://arxiv.org/abs/2604.09577) - Google paper showing a prompted LLM can build custom UIs for almost any prompt.
- [Gradual Generation of User Interfaces](https://arxiv.org/abs/2601.17975) - Paper on staging GenUI customizations so users can discover them step by step.
- [Macaron A2UI Bench](https://github.com/MindLab-Research/Macaron-A2UI-Bench) - Benchmark that scores the A2UI JSON a model generates, with optional visual checks.
- [Macaron-A2UI](https://arxiv.org/abs/2605.24830) - Paper on a model that generates text plus lightweight UI actions for personal agents.

## Guides and reading

- [AG-UI Protocol: Bridging Agents to Any Front End](https://www.copilotkit.ai/blog/ag-ui-protocol-bridging-agents-to-any-front-end) - CopilotKit post explaining the AG-UI event model.
- [AI SDK generative user interfaces](https://ai-sdk.dev/docs/ai-sdk-ui/generative-user-interfaces) - AI SDK guide to rendering tool results as React components.
- [Enabling teachers to create learning interactives with generative UI](https://research.google/blog/the-future-of-practice-enabling-teachers-to-create-learning-interactives-with-generative-ui/) - Google Research on generative UI for classroom simulations.
- [Generative UI and Outcome-Oriented Design](https://www.nngroup.com/articles/generative-ui/) - Nielsen Norman Group essay on interfaces generated for each user and task.
- [Generative UI in Gemini and Search](https://research.google/blog/generative-ui-a-rich-custom-visual-interactive-user-experience-for-any-prompt/) - Google Research post on shipping generative UI in the Gemini app and Search.
- [Introducing A2UI](https://developers.googleblog.com/introducing-a2ui-an-open-project-for-agent-driven-interfaces/) - Google Developers post introducing the A2UI project.
- [Introducing AI SDK 3.0 with Generative UI](https://vercel.com/blog/ai-sdk-3-generative-ui) - Vercel post that brought streamed React components from tool calls to the AI SDK.
- [The Developer's Guide to Generative UI in 2026](https://www.copilotkit.ai/blog/the-developer-s-guide-to-generative-ui-in-2026) - CopilotKit overview of static, declarative and open-ended generative UI.

## Contributing

Contributions are welcome. Read the [contribution guidelines](contributing.md) first.

<!-- awesome:maintainer -->
Maintained by [Ian Wiedenman](https://github.com/ianwieds).
<!-- /awesome:maintainer -->
