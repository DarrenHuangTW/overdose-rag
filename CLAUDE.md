# Overdose RAG Project - Claude Code Documentation

## Project Overview
This is a knowledge-sharing project for the SEO team at Overdose Digital, demonstrating embedding models and RAG (Retrieval-Augmented Generation) concepts through practical examples.

## Repository Structure
```
overdose-rag/
├── OD_RAG.ipynb           # Main Google Colab notebook for presentation
├── rag.ipynb              # Original working notebook
├── speaker_notes.md       # Comprehensive presentation notes
├── requirements.txt       # Python dependencies for local setup
├── static/
│   ├── embedding vs generative models.jpg  # Generative vs embedding visual
│   ├── vectorization example.png          # Text-to-vector demonstration
│   ├── king queen.png                     # Famous vector arithmetic example
│   ├── cosine similarity.png              # Similarity calculation diagram
│   ├── chunk_embedding.png                # Chunking process visualization
│   ├── rag.png                           # Complete RAG pipeline diagram
│   ├── 100_embeddings.csv                # Pre-computed embeddings dataset
│   ├── 100_words.csv                     # Word categories dataset
│   └── quality_rater.txt                 # Google Quality Rater Guidelines
└── CLAUDE.md              # This documentation file
```

## Key Components

### 1. OD_RAG.ipynb - Main Presentation Notebook
**Purpose**: Clean, presentation-ready Colab notebook hosted on GitHub
**GitHub URL**: https://github.com/DarrenHuangTW/overdose-rag/
**Colab Link**: https://colab.research.google.com/github/DarrenHuangTW/od_rag_knowledge_share/blob/main/OD_RAG.ipynb

**Sections**:
- **Opening**: Generative vs Embedding models with visual comparison diagram
- **From Text to Numbers**: How AI converts language into mathematical coordinates (with examples)
- **2D/3D Visualization**: t-SNE plots showing semantic clustering by category
- **Measuring Similarity**: King-Queen vector arithmetic + cosine similarity concepts
- **From Words to Everything**: Embeddings at scale (sentences, documents, images, audio)
- **Breaking Down Large Content**: Chunking strategies and context window limitations
- **RAG Pipeline**: Complete retrieval-augmented generation workflow with real Google data
- **Discussion**: Real-world complexities including hybrid search strategies

### 2. Technical Implementation

**Embedding Model**: OpenAI text-embedding-3-small (1,536 dimensions)
**Vector Database**: ChromaDB with cosine similarity
**Visualization**: t-SNE dimensionality reduction (2D/3D)
**Demo Dataset**: 100 words across 4 categories (Animal, Food, Occupation, Weather)
**Real Document**: Google Quality Rater Guidelines (33 chunks, 600 chars each)

### 3. Key Demonstrations

**Similarity Examples**:
- Koala vs Kangaroo: 0.648 similarity (both Australian marsupials)
- "what is SEO" vs SEO definition: 0.773 similarity (semantic matching)

**RAG Query Example**:
- Query: "how many Search Quality Raters are there?"
- Retrieved: 3 most relevant chunks from Google Quality Rater Guidelines
- AI Generated Answer: "There are approximately 16,000 external Search Quality Raters."
- Demonstrates: Complete pipeline from document → chunks → vector search → LLM generation

**Visualization Insights**:
- Animal words cluster together (cats, dogs, elephants)
- Food items form distinct clusters
- Weather terms group separately
- Occupations cluster away from other categories

### 4. SEO Applications Demonstrated

**Content Strategy**:
- Semantic similarity reveals content relationships
- RAG enables intelligent content gap analysis
- Embedding-based search understanding

**Modern Search Reality**:
- Google's BERT = embedding model
- Featured Snippets powered by semantic understanding
- "People Also Ask" uses content relationship mapping
- Semantic search beyond exact keyword matching

### 5. Interactive Elements for Presentation

**Audience Participation**:
- Similarity guessing games
- Category clustering predictions
- Real-time embedding comparisons

**Visual Demonstrations**:
- 3D rotating word clusters
- Similarity score calculations
- RAG retrieval process walkthrough

## Technical Notes

### Dependencies
```python
openai>=1.0.0        # OpenAI API for embeddings and chat completion
chromadb>=0.4.0      # Vector database for RAG implementation
plotly>=5.15.0       # Interactive 3D visualizations
matplotlib>=3.6.0    # 2D plotting and static visualizations
scikit-learn>=1.3.0  # t-SNE dimensionality reduction
pandas>=1.5.0        # Data manipulation and CSV handling
numpy>=1.24.0        # Numerical computations
requests>=2.28.0     # HTTP requests for data downloads
nbformat>=4.2.0      # Jupyter notebook format compatibility
```

### Data Sources
- **100_embeddings.csv**: Pre-computed embeddings hosted on Google Drive
- **100_words.csv**: Word categories dataset with Animal, Food, Occupation, Weather (25 each)
- **Quality Rater Guidelines**: Real Google document downloaded from Google Drive
- **Visual Assets**: 6 custom diagrams explaining concepts and processes

### Presentation Flow
1. **Concept Introduction** (5 min): Generative vs Embedding models
2. **Technical Demo** (15 min): Vectorization → Visualization → Similarity
3. **RAG Walkthrough** (10 min): Complete search system demonstration
4. **SEO Applications** (10 min): Real-world use cases
5. **Interactive Q&A** (10 min): Audience engagement and discussion

## Key Takeaways for SEO Team

**Mindset Shift**:
- From keyword matching to semantic understanding
- From exact matches to conceptual relationships
- From guessing intent to measuring similarity
- From pure semantic search to hybrid approaches

**Practical Applications**:
- Content optimization using semantic analysis
- FAQ systems that understand question variations
- Competitor analysis through content vectorization
- User intent mapping via embedding similarities
- Product search requiring exact + semantic matching

**Real-World Complexities Covered**:
- Document processing challenges (PDFs, tables, layouts)
- Chunking strategy optimization techniques
- Embedding model selection for different use cases
- Scalability solutions for millions of documents
- Query transformation and enhancement methods
- Hybrid search: When keyword search beats semantic search

**Critical Insights**:
- Semantic search isn't always better than keyword search
- SKU/product queries need hybrid approaches to avoid wrong answers
- Production RAG systems require sophisticated orchestration
- Context windows apply to both generative and embedding models

## Success Metrics
- Team understands embedding vs generative AI distinction
- Clear grasp of how modern search engines work
- Practical ideas for applying semantic search concepts
- Excitement about AI-powered SEO strategies

## Repository Maintenance
- Notebook tested in Google Colab environment
- All external links validated and working
- Images hosted on GitHub for reliable access
- Documentation updated with latest insights

---

*This project bridges the gap between complex AI concepts and practical SEO applications, making embeddings and RAG accessible to marketing professionals.*