# generative-ai-go
A quick overview of how to get started with the Go SDK to ask the model questions that mix text with images.

## Google AI SDK for Go - Multimodal LLMs

A quick overview of getting started with Google's AI Software Development Kit (SDK) for Go to interact with their latest family of multimodal Large Language Models (LLMs) via an API. Google offers a generous free tier for their API, making it accessible to developers. The Go SDK is part of the generative-ai-go repository, and its documentation can be found at [https://pkg.go.dev/github.com/google/generative-ai-go](https://pkg.go.dev/github.com/google/generative-ai-go).

## Task Overview

The goal is to utilize the Google AI SDK to ask the model questions that involve both text and images. Specifically, we'll ask the model to explain the difference between two images of turtles.

### Important Note

The LLM API being multimodal, the SDK provides helper types like `genai.ImageData` and `genai.Text` to wrap inputs in a type-safe way. When running the sample, the model's response is dumped as a JSON object. The relevant information is within the "Content" section, where the model provides detailed descriptions of the images.