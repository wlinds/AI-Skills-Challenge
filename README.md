# AI-Skills-Challenge-2024
Part of AI Skills Challenge through [LearnMicrosoftAI](https://learn.microsoft.com/)


# Summary

## What is Azure AI Services?
A portfolio of services that can be integrated into applications without specialist knowledge. Azure AI services *is also* the name for the multi-service resource created in the Azure portal that provides access to all Azure AI services with a single key and endpoint.

>As of July 2023, services previously known as Cognitive Services and Azure Applied AI Services are now part of AI Services.

## NLP | Azure AI Language Studio

- Azure AI Language (Available in Language Studio and API or SDK)
    - Understanding and analyzing text, train conversational language model
    - Either write code *or* author conversational model through Language studio

    Get started with NLP documentation:
    - [Text/document summarization](https://learn.microsoft.com/en-us/azure/ai-services/language-service/summarization/overview?tabs=document-summarization)
    - [Classification tasks](https://learn.microsoft.com/en-us/azure/ai-services/language-service/custom-text-classification/overview)
    - [Key-phrase extractions](https://learn.microsoft.com/en-us/azure/ai-services/language-service/key-phrase-extraction/overview)
    - [Sentiment analysis](https://learn.microsoft.com/en-us/azure/ai-services/language-service/sentiment-opinion-mining/overview?tabs=prebuilt)

- Azure AI Bot service: framework for developing, publishing, and managing bots
    - Use MS Bot Framework SDK to write code that controls conversation flow and integrates with a knowledge base.
    - Deploy to custom web chats, email, Teams

### Document Intelligence | Document Intelligence Studio
- Extract and manage data collection from scanned documents
- Create custom models with own labeled dataset or use pre-trained


### Azure AI Search
- Platform as a Service (Paas) solution where all infra is managed by Microsoft
- Azure AI Search index: Container of searchable documents.
- Programmable search engine built on [open source Apache Luence](https://lucene.apache.org)
- Knowledge mining (extract information from large volumes of unstructured data)
- Search results contain **only** your data.
- Index your documents in Azure Storage as JSON
- Supports PUSH & PULL via REST API
- Supports Cosmos DB, Azure SQL and Azure Storage



### Speech Studio
Speech recognition takes the spoken word (real-time or from file) and converts it into data that can be processed - often by transcribing it into text.

Azure Speech Studio offers:
    - Spech recognition, synthesis, real-time translations, transcibe

Available APIs:
- The Speech to text API
- The Text to speech API


### Computer Vision (CV) Services | Azure Vision Studio
Azure AI Vision provides prebuilt CV models based on [Florence](https://www.microsoft.com/en-us/research/project/projectflorence/) (Transformers)

- Image Analysis: images & video.
- Extracting description, tags, objects, text.
- Optical character recognition (OCR) - extracting text from images.
- Generating captions and descriptions of images.
- Detection of objects in images.
- Tagging visual features in images
- Basic face analysis (returning bounding box and coordinates of face)

Azure AI Face
- Pre-built models to detect, recognize and analyze faces

Azure AI Video Indexer
- Analyze video and audio content by running 30+ AI model ([Documentation](https://learn.microsoft.com/en-us/azure/azure-video-indexer/video-indexer-overview))


## Azure Machine Learning Studio
The fundamental idea of ML is to use data from past observations to predict unknown outcomes or values (inferencing).

All of Azure Machine learning relies on Python but you necessarily don't need to write any code yourself.

- Automated Machine learning (AutoML): Enables non-experts to quickly create ML models ([Documentation](https://learn.microsoft.com/en-us/azure/machine-learning/concept-automated-ml?view=azureml-api-2))

- Azure Machine learning designer:  drag-and-drop UI for no-code development of ML models ([Documentation](https://learn.microsoft.com/en-us/azure/machine-learning/concept-designer?view=azureml-api-2))
- Data metric visualization
- Notebooks: Write & run your own Python code in Jupyter Notebook
- Deploy models

#### Model Collections:
- Open source models curated by Azure AI
- Azure OpenAI models
- Transformers models from the HuggingFace hub

See all [available models here](https://ml.azure.com/registries/models) (sign-in and resource group (free to create) required for workspace).

Learn about the [fundamentals of Machine Learning here](https://github.com/wlinds/AI-Skills-Challenge/blob/main/Azure%20AI%20Fundamentals/01_fundamentals_of_ml.ipynb)

--- 

# Table of Contents
### [00: Introduction](<Azure AI Fundamentals/00_introduction.ipynb>)
- What is AI?
- Undertstanding ML, CV, NLP, DI, Knowledge Mining, GenAI
- Challenges & Risks
- Responsible AI
- Azure implementations

### [01: Machine Learning](<Azure AI Fundamentals/01_fundamentals_of_ml.ipynb>)
- Machine Learning as a function
- Supervised & Unsupervised ML
- Regression, binary classification, multiclass, clustering
- Evaluation metrics
- Deep Learning
- Azure Machine Learning

### [02: Azure AI Services](<Azure AI Fundamentals/02_fundamental_azure_ai_services.ipynb>)
- Resources
- Keys, Endpoints & APIs

### [03: Computer Vision](<Azure AI Fundamentals/03_computer_vision.ipynb>)
- Images & Pixel Processing
- Laplace filters
- Introduction: CNNs, Transformers & Multi-modal Models
- Azure AI Vision: OCR, Image classification, Object detection

### [04: Facial Recognition](<Azure AI Fundamentals/04_facial_recognition.ipynb>)
- Face Detection & Face Analysis
- Responsible AI Use
- Face Service
- Tips for more accurate results

### [05: OCR](<Azure AI Fundamentals/05_OCR.ipynb>)
- Uses of OCR
- Azure AI Vision's OSCR Engine (Read API):
    - Images, PDFs TIFFs

### [06: Text Analysis](<Azure AI Fundamentals/06_text_analysis.ipynb>)
- Tokenization
    - Normalization
    - Stopwords
    - n-grams
    - Stemming
- Frequency Analysis
- Sentiment Analysis
- Semantic Language Models
- Entity Recognition
- Language Detection
- Key Phrase Extraction

### [07: Question Answering](<Azure AI Fundamentals/07_question_answering.ipynb>)
- Azure AI Language REST API
- Microsoft Bot Framework SDK

### [08: Conversational Language](<Azure AI Fundamentals/08_conversational_language.ipynb>)
- Utterance, Entities, Intents
- Authoring, Training, Predicting

### [09: Azure AI Speech](<Azure AI Fundamentals/09_auzre_ai_speech.ipynb>)
- Real-time transcription
- Speech synthesis

### [10: Document Intelligence](<Azure AI Fundamentals/10_document_intelligence.ipynb>)
- Text extraction
- Prebuilt & Custom models

### [11: Azure AI Search](<Azure AI Fundamentals/11_azure_ai_search.ipynb>)
- Knowledge mining
- Automate data ingestion steps
- JSON serialization
- OData expression language

### [12: Generative AI](<Azure AI Fundamentals/12_generative_ai.ipynb>)
- Natural language (NLP)
    - Determine eentiment & classifying
    - Summarizing
    - Comparing for semantic similarity
    - Generating new natural language
- Image generation
- Code generation
- Transformer models
    - Encoders & Decoders
    - Tokenization
    - Embeddings
    - Attention
- Azure OpenAI
- Microsoft Copilot
- Prompt Engineering

### [13: Azure OpenAI](<Azure AI Fundamentals/13_azure_openai.ipynb>)
- OpenAI Models
- Intro to OpenAI Service & Workloads
- OpenAI Studio
- GitHub Copilot
- Microsoft AI principles

### [14: Responsible GenAI](<Azure AI Fundamentals/14_responsible_genai.ipynb>)
- Identifying potential harms
- Content filters

### [15: Prepare to develop AI solutions](<Azure AI Fundamentals/15_prepare_to_dev_on_Azure.ipynb>)
- AI-related terms & definitions
- Responsible AI
    - Fairness
    - Reliability and safety
    - Privacy and security
    - Inclusiveness
    - Transparency
    - Accountability

### [16: Create & consume AI services](<Azure AI Fundamentals/16_create_consume.ipynb>)
- Options for Azure resources
- Rest API
- SDK

### [17: Secure Azure AI services](<Azure AI Fundamentals/17_secure_azure.ipynb>)
- Authentication & Security
- Azure Key Vault
- Entra ID
- Service principal
- Managed identities

### [18: Monitor Services](<Azure AI Fundamentals/18_monitor.ipynb>)
- Metrics & Alerts
- Azure Event Hub
- Azure log analytics

### [19: Deploy Azure AI services in containers](<Azure AI Fundamentals/19_deployment.ipynb>)
- Containerization