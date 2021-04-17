# Information retrieval system implementation

## ℹ️ Project info
*   **Course**: PV211 Introduction to information retrieval
*   Semester: Summer semester 2021
*   **Author**: Adam Hospodka ([506521@muni.cz](mailto:506521@muni.cz))
*   **UČO**: 506521

## 🧭 Application overview

### Idea:
Ranking the documents for given queries using the standard *TF-IDF* approach with small tweaks.

###Steps:
1. List every word from every document using ```buildPairs()``` function
2. Remove duplicates using the ```uniq()``` function
3. Based on these pairs create inverted index using the ```buildInvertedIndex()``` function
4. Use knowledge of inverted index to build frequency index (inv. index with word frequencies) using the ```buildFrequencyIndex()``` function
5. Build index that contains length of each document using the ```buildDocumentsLengthIndex()``` function
6. Prepare *Pandas* DataFrame with document instances ready to be ranked using the ```buildRankingDf()``` function
7. Initialize the search with ```IRSystem.search()```
8. Clean the given query with the ```cleanQuery()``` function
9. Rank the relevant documents with the ```rank()``` function


