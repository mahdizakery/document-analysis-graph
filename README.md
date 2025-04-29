# Document Analysis Graph: Educational Example with LangGraph and Tools

This project demonstrates how to use [LangGraph](https://github.com/langchain-ai/langgraph) with tool integration for document and image analysis, using Google Gemini models via LangChain. It is designed for educational purposes and showcases how to build a simple agent that can:

- Extract text from images using a vision-capable LLM
- Perform basic computations (e.g., division)
- Route tasks between an assistant and tool nodes in a graph structure

## Features
- **Vision Tool**: Extracts text from images (e.g., meal plans, notes)
- **Computation Tool**: Performs division operations
- **Graph-based Agent**: Uses LangGraph to manage control flow between assistant and tools
- **Notebook-based**: All code and examples are in a Jupyter notebook for easy experimentation

## Example Usage

1. **Extract Text from an Image**
   - Place an image (e.g., `Batman_training_and_meals.png`) in the project directory.
   - Run the notebook cell to extract text from the image using the `extract_text` tool.

2. **Ask Questions or Perform Calculations**
   - Example: "Divide 6790 by 5" or "What should I buy for the dinner menu according to the note?"
   - The agent will use the appropriate tool and return the answer.

## Getting Started

1. Clone the repository and install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Set up your Google API key (and Langfuse keys if using tracing):
   - Create a `.env` file with:
     ```
     GOOGLE_API_KEY=your_google_api_key
     LANGFUSE_PUBLIC_KEY=your_langfuse_public_key
     LANGFUSE_SECRET_KEY=your_langfuse_secret_key
     ```
3. Open `doc-analysis-graph.ipynb` in Jupyter and follow the cells.

## Educational Notes
- The project is structured to show how to combine LLMs, tool use, and graph-based control flow.
- The agent ("Alfred") is designed to be extendable with more tools or logic.
- The code is commented for clarity and learning.

## References
- [LangGraph Documentation](https://langgraph.langchain.com/)
- [LangChain Google GenAI](https://python.langchain.com/docs/integrations/chat/google_genai)
- [Google Gemini API](https://ai.google.dev/)
- [Hugging Face Agents Course](https://huggingface.co/learn/agents) – educational material

---

**For educational use only.**
