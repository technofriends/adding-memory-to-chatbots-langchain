# Adding Memory to Chatbots

This Python notebook demonstrates how to add memory capabilities to chatbots using the Langchain library and OpenAI's language models. It covers various memory modules provided by Langchain, including `ChatMessageHistory`, `ConversationBufferMemory`, and `ConversationSummaryMemory`. By following along with this notebook, you will learn how to enhance your chatbots with memory, enabling them to provide more coherent and contextually relevant responses.

You can also go through the video tutorial on which this notebook is based at : https://youtu.be/2nWssLfXLZE

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [Notebook Overview](#notebook-overview)
3. [ChatMessageHistory](#chatmessagehistory)
4. [ConversationBufferMemory](#conversationbuffermemory)
5. [ConversationSummaryMemory](#conversationsummarymemory)
6. [Examples](#examples)
7. [Expected Outcomes](#expected-outcomes)
8. [Extending the Notebook](#extending-the-notebook)
9. [Conclusion](#conclusion)
10. [Additional Resources](#additional-resources)

## Prerequisites

To run this notebook, ensure that you have the following dependencies installed:

- Python 3.7 or higher
- Langchain library (version 0.1.26 or higher)
- OpenAI API key

Make sure to set up your environment with the required dependencies before running the notebook. You can install the Langchain library using pip:

```bash
pip install langchain openai langchain-openai python-dotenv 
```

Additionally, you will need to set up your OpenAI API key as an environment variable or provide it directly in the notebook.

## Notebook Overview

The notebook begins by importing the necessary libraries and setting up the OpenAI API key. It then demonstrates how to create a simple chatbot using Langchain and OpenAI's `ChatOpenAI` class. Langchain is a powerful library that provides a set of tools and components for building language-aware applications, while OpenAI's `ChatOpenAI` class allows you to interact with OpenAI's language models programmatically.

The chatbot is initialized with a system message and a human message template, which guide its responses and provide context for the conversation.

The notebook then proceeds to showcase different memory modules that can be added to the chatbot to enhance its conversational capabilities. These memory modules enable the chatbot to store and retrieve conversation history, generate summaries, and maintain context across multiple interactions.

## ChatMessageHistory

The `ChatMessageHistory` module allows the chatbot to keep track of the conversation history. It stores the user's messages and the chatbot's responses in a list of messages. The notebook demonstrates how to add user and AI messages to the history and retrieve the conversation history.

By utilizing the `ChatMessageHistory` module, the chatbot can refer back to previous messages and provide responses that are coherent with the ongoing conversation.

## ConversationBufferMemory

The `ConversationBufferMemory` module provides a sliding window buffer to store the conversation history. It allows the chatbot to remember a fixed number of recent messages, enabling it to maintain context within a limited scope.

The notebook shows how to create a `ConversationChain` using the `ConversationBufferMemory` and interact with the chatbot while maintaining a limited conversation history. This memory module is particularly useful when you want to keep the chatbot's memory focused on the most recent interactions.

## ConversationSummaryMemory

The `ConversationSummaryMemory` module enables the chatbot to generate a summary of the conversation history. It utilizes a language model to summarize the conversation based on the previous messages, allowing the chatbot to maintain a high-level understanding of the conversation's key points.

The notebook demonstrates how to create a `ConversationChain` with `ConversationSummaryMemory` and engage in a conversation with the chatbot while generating summaries of the conversation at each step. This memory module helps the chatbot to capture the essence of the conversation and provide more contextually relevant responses.

## Examples

Throughout the notebook, various examples are provided to showcase the capabilities of each memory module. Here are a couple of examples:

1. The chatbot is asked about Apple's mission statement, and it provides a detailed response. The response is then summarized using the `ConversationSummaryMemory` module, allowing the chatbot to generate a concise summary of the mission statement.

2. The chatbot is asked to compare Apple's mission statement with Google's. The `ConversationBufferMemory` module is used to maintain the context of the previous questions and responses, enabling the chatbot to provide a relevant comparison based on the limited conversation history.

These examples demonstrate how the different memory modules can be used to enhance the chatbot's conversational abilities and provide more coherent and contextually appropriate responses.

## Expected Outcomes

By running this notebook and exploring the different memory modules, you can expect to achieve the following:

1. Understand how to integrate memory capabilities into chatbots using Langchain and OpenAI.
2. Learn how to use the `ChatMessageHistory` module to store and retrieve conversation history.
3. Discover how the `ConversationBufferMemory` module can be used to maintain a sliding window buffer of recent messages.
4. Understand how the `ConversationSummaryMemory` module generates summaries of the conversation history using a language model.
5. Gain insights into how memory modules can enhance the chatbot's ability to provide coherent and contextually relevant responses.

By the end of the notebook, you will have a solid foundation in adding memory capabilities to chatbots and be equipped with the knowledge to apply these techniques to your own chatbot projects.

## Extending the Notebook

While the notebook provides a comprehensive overview of adding memory to chatbots using Langchain and OpenAI, there are numerous ways to extend and experiment with the concepts covered. Here are a few ideas:

1. Try different configurations of the memory modules, such as adjusting the buffer size in `ConversationBufferMemory` or experimenting with different summarization strategies in `ConversationSummaryMemory`.

2. Integrate additional memory modules provided by Langchain or explore custom memory implementations to suit specific use cases.

3. Extend the chatbot's capabilities by incorporating other language models or integrating external knowledge sources to enhance its responses.

4. Implement a user interface or deploy the chatbot as a web application to interact with it in a more user-friendly manner.

Feel free to explore and build upon the notebook to create even more sophisticated and powerful memory-enhanced chatbots.

## Conclusion

Adding memory capabilities to chatbots is a crucial step in creating more engaging and intelligent conversational agents. This notebook has provided a comprehensive guide on how to use Langchain and OpenAI to incorporate memory modules into your chatbots.

By leveraging the power of `ChatMessageHistory`, `ConversationBufferMemory`, and `ConversationSummaryMemory`, you can enable your chatbots to store and retrieve conversation history, maintain context, and generate summaries of the conversation. These memory modules enhance the chatbot's ability to provide coherent and contextually relevant responses, leading to more natural and meaningful interactions.

We encourage you to dive into the notebook, experiment with the different memory modules, and extend the chatbot's capabilities to suit your specific needs. With the knowledge gained from this notebook, you are well-equipped to create memory-enhanced chatbots that can engage users in more sophisticated and intelligent conversations.

## Additional Resources

To further expand your knowledge and explore related topics, you may find the following resources helpful:

- [Langchain Documentation](https://langchain.readthedocs.io/): Official documentation for the Langchain library, providing detailed information on its features and usage.
- [OpenAI API Documentation](https://beta.openai.com/docs/): Documentation for the OpenAI API, including guides on how to integrate OpenAI's language models into your applications.
- [Langchain GitHub Repository](https://github.com/hwchase17/langchain): The GitHub repository for the Langchain library, where you can explore the source code, contribute to the project, and find additional examples.
- [OpenAI Blog](https://openai.com/blog/): OpenAI's official blog, featuring articles and insights on artificial intelligence, language models, and related topics.

These resources will provide you with a deeper understanding of Langchain, OpenAI, and the broader field of natural language processing and conversational AI.
