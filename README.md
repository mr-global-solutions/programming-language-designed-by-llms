# We asked LLMs what Programming Language they would design
## Intro
We ran an interesting experiment, asking major LLMs what kind of programming language they would design for machine-to-machine interaction.
## Prompt
```
You're an experienced software architect in charge of designing from scratch a new programming language - called NextLang - for the next generation of LLMs.

NextLang enables LLMs/AI tools to work with other AI tools (aka other machines), write software, and orchestrate complex architectures, without any kind of human intervention.

NextLang needs to be efficient for machine-to-machine interaction.

Explain why you would make certain architectural decisions while designing NextLang.

Help me to understand the main aspects of NextLang by describing it with examples and by comparing it with pre-existing human-readable programming languages.
```
## Models and Responses
* `Claude 3.7 Sonnet` in `Explanatory` mode
  * See [Claude full response](./claude/claude-response.md)
* `Grok 3` in `Think` mode
  * See [Grok full response](./grok/grok-response.txt)
* `Gemini 2.5 Pro (preview)`
  * See [Gemini full response](./gemini/gemini-results.md)
* `OpenAI o4-mini` in `Extendeed Thinking` mode
  * See [ChatGPT full response](./openai/openai-results.md)
* `Llama 4`
  * See [Llama full response](./llama/llama-results.md)
* `DeepSeek` in `DeepThink R1` mode
  * See [DeepSeek full response](./deepseek/deepseek-results.md)
## Claude - Quick Overview
### Architecture
* Semantic Precision
  * Executable constraints and requirements integrated into syntax
* Intent-Based Execution Model
  * Declarative specification of outcomes with optimization delegation
* Probabilistic Computation Framework
  * Native uncertainty quantification and confidence thresholds
* Controlled Self-Modification
  * Bounded evolutionary capabilities with invariant preservation
* Dynamic Context Adaptation
  * Resource-aware execution with environment-sensitive scaling
* First-Class Knowledge Representation
  * Ontological structures and inference rules as core constructs
### Differentiators
* Semantic Type System
  * Enhanced typing with metadata for privacy, staleness, and usage constraints
* Integrated Formal Verification
  * Built-in precondition/postcondition enforcement and invariant checking
* Cross-Domain Semantic Mapping
  * Standardised translation between AI domain representations
### Advantages
* Reduced Semantic Loss
  * Direct conceptual exchange between AI systems
* Adaptive Resource Allocation
  * Priority-based computation distribution
* Verification-First Architecture
  * Provable correctness as a primary design principle
## Grok - Quick Overview
### Architecture
* Minimalist Syntax
 * Streamlined, symbol-based syntax (e.g., `COND(x > 5, PRINT("greater"), PRINT("lesser"))`) reduces parsing complexity and speeds up code processing by LLMs
* Native Complex Data Structures
 * Built-in support for AI-relevant data types like graphs, trees, and matrices (e.g., `m1 = Matrix([[1, 2], [3, 4]]); result = m1.multiply(m2)`), integrated into the language core to avoid external library dependencies.
* First-Class Concurrency
 * Native asynchronous and parallel execution (e.g., `ASYNC PROCESS_DATA(input); SEND_RESULT(output)`) ensures efficient multitasking, with automatic thread management optimized for AI workflows.
* Strict Standardization
 * Enforces uniform syntax, semantics, and data formats to ensure interoperability across AI tools, avoiding the compatibility issues seen in languages like JavaScript with multiple dialects.
### Differentiators
* AI-Specific Primitives
 * Built-in functions for AI tasks like model training and inference (e.g., `model = TRAIN_MODEL(dataset, labels, epochs=10); prediction = INFER(model, new_data)`), unlike Python’s reliance on external frameworks like TensorFlow or PyTorch.
* Self-Modification Capabilities
 * Allows AI to dynamically optimize its own code (e.g., `new_function = OPTIMIZE_FUNCTION(existing_function, "speed")`), a feature absent in languages like C++ due to risks for human programmers.
* Native Communication Protocols
 * Embeds support for protocols like HTTP and WebSocket (e.g., `response = SEND_HTTP("https://api.example.com", "GET", null)`), eliminating the need for external libraries like Python’s requests.
### Advantages
* Robust Error Handling
 * Autonomous error recovery with retries and logging (e.g., `TRY FETCH_DATA(url) CATCH { RETRY(3, FETCH_DATA(url)) || LOG(error) }`) ensures resilience without human intervention, unlike Java’s manual try-catch blocks.
* Built-In Security
 * Native authentication and encryption (e.g., `SECURE_CONNECT("server.ai", credentials)`) ensure consistent security, reducing configuration errors compared to Python’s reliance on libraries like ssl.
* Modularity for Reusability
 * Reusable code blocks with machine-readable metadata (e.g., `MODULE DataProcessor(inputs: data, outputs: processed_data)`) enable AI to build complex systems efficiently, enhancing Java’s class-based modularity with AI-specific metadata.
