``python from langchain_openai import ChatOpenAI


def main():
    # Create the LangChain ChatOpenAI model
    llm = ChatOpenAI(
        model="gpt-4o-mini",
        temperature=0
    )

    prompts = [
        "What is the capital of Tamil Nadu?",
        "Explain artificial intelligence in two simple sentences.",
        "What are three benefits of solar energy?"
    ]

    for i, prompt in enumerate(prompts, start=1):
        response = llm.invoke(prompt)

        print(f"\n--- Prompt {i} ---")
        print(f"Question: {prompt}")
        print("Answer:")
        print(response.content)


if __name__ == "__main__":
    main()
```
