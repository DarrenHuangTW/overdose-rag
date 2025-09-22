# Overdose RAG Project - Claude Code Documentation

## Project Overview
This is a knowledge-sharing project for the SEO team at Overdose Digital, demonstrating embedding models and RAG (Retrieval-Augmented Generation) concepts through practical examples.

## Repository Structure
```
overdose-rag/
├── OD_RAG.ipynb           # Main Google Colab notebook for presentation
├── rag.ipynb              # Original working notebook
├── speaker_notes.md       # Comprehensive presentation notes
├── static/
│   ├── embedding vs generative models.jpg  # Visual comparison diagram
│   └── quality_rater.txt  # Google Quality Rater Guidelines (sample text)
├── 100_embeddings.csv     # Pre-computed embeddings dataset
└── CLAUDE.md              # This documentation file
```

## Key Components

### 1. OD_RAG.ipynb - Main Presentation Notebook
**Purpose**: Clean, presentation-ready Colab notebook hosted on GitHub
**GitHub URL**: https://github.com/DarrenHuangTW/overdose-rag/
**Colab Link**: https://colab.research.google.com/github/DarrenHuangTW/od_rag_knowledge_share/blob/main/OD_RAG.ipynb

**Sections**:
- **Opening**: Generative vs Embedding models explanation with visual diagram
- **Vectorization**: Text-to-numbers conversion using OpenAI's text-embedding-3-small
- **Visualization**: 2D/3D t-SNE plots showing semantic clustering
- **Similarity**: Cosine similarity calculations between concepts
- **Query vs Document**: Ranking documents by relevance
- **Chunking**: Text preprocessing for RAG systems
- **RAG**: Complete retrieval-augmented generation workflow
- **Discussion**: Advanced topics and considerations

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
- Answer: Found "~16,000 external Search Quality Raters" from document chunks
- Top similarity: 0.754 (chunk about rater process)

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
openai==1.x          # OpenAI API for embeddings
chromadb             # Vector database
plotly               # 3D visualizations
matplotlib           # 2D plotting
scikit-learn         # t-SNE dimensionality reduction
pandas               # Data manipulation
numpy                # Numerical computations
```

### Data Sources
- **100_embeddings.csv**: Pre-computed embeddings from Google Drive
- **Quality Rater Guidelines**: Downloaded from Google Drive as sample document
- **Categories**: Animal, Food, Occupation, Weather (25 words each)

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

**Practical Applications**:
- Content optimization using semantic analysis
- FAQ systems that understand question variations
- Competitor analysis through content vectorization
- User intent mapping via embedding similarities

**Future Considerations**:
- Multilingual and multimodal embeddings
- Domain-specific embedding models
- Efficient similarity search at scale
- Query transformation and contextualization

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