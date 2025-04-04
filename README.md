# Frame SDK

The Frame SDK is a TypeScript-based client for interacting with the Frame API, enabling seamless image ingestion, embedding, and multimodal search by text or image. It provides an intuitive interface for managing documents, retrieving vector-based recommendations, and performing similarity searches.

## Features

- 📄 **Document Management** – Create, retrieve, and delete documents
- 🔎 **Vector Search** – Perform similarity-based searches on images and text
- 🧠 **Recommendations** – Get relevant image recommendations based on embeddings
- 🚀 **Easy Integration** – Simple API methods for quick adoption

## Installation

```bash
npm install frame-sdk
```

## Usage

```typescript
import { Client } from 'frame-sdk';

const client = new Client({
  apiKey: 'YOUR_API_KEY',
  baseURL: 'https://api.frame.com',
});

// Example usage
client.getDocuments().then(response => {
  console.log(response);
});
```

## API Methods

getDocuments(params?) – Retrieve a list of documents

getDocumentById(id) – Fetch a document by its ID

createDocuments(documents) – Upload new documents

deleteDocumentById(id) – Delete a document

searchDocuments(query) – Perform similarity search

getRecommendations(id, options?) – Get recommended documents

For full documentation, visit Frame Docs.
