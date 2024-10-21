# RAG-based-Chatbot-for-Landcover-Mapping
The proposed approach integrates remote sensing data with Large Language Models (LLMs) to analyze land cover,
emphasizing sustainable resource management. The workflow seamlessly incorporates response creation, retrieval augmentation, semantic segmentation, and image captioning. Leveraging the DeepLabV3 architecture with a ResNet34 encoder, the Segmentation Deep Neural Network, trained on the DeepGlobe dataset, demonstrates proficiency in classifying land use. The obtained results not only showcase the model’s linguistic precision in interpreting user inquiries but also include visualizations illustrating both successful and challenging scenarios.

# Retrieval Augmented Generation
The contextual information from the BLIP model and the percentage of class coverage are both transformed into embedding using the sentence-transformers
and all-MiniLM-l6-v2 model. Subsequently, the embodiment are incorporated into a vector database (FAISS) for retrieval augmented generation. This integration enhances data retrieval and augmentation processes, contributing to a more robust and comprehensive generation of results.

# Response Generation:
According to the user query, the context is retrieved from the vector database using the Retrieval Augmented Generation (RAG) pipeline. This retrieved context is then integrated into the language model (LLM), and a response is generated based on prompt tuning. This process ensures that the generated response aligns with the user’s query and the contextual information retrieved from the vector database.
