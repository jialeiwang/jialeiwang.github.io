**Semantic Search (Invited Talk)**
----

ABSTRACT
------
Semantic search lies in the cross roads of information retrieval and natural language processing and is the current frontier of search technology.  In this presentation, we outline our technology regarding this search challenge.

**Keywords**: *semantic processing*,  *semantic ranking*, *query understanding*, *learning to rank*.
 
 SUMMARY
----
Semantic search [[2](http://www.nowpublishers.com/article/Details/INR-032)] is a challenging problem that has several parts. The first one consists in building a semantically annotated index with the help of a knowledge base. To achieve this, we first need to predict the language of each document and parse it accordingly to that language. Second, we need to extract all entities and concepts mentioned in the document with the help of the knowledge base. All the knowledge base infrastructure needs to be independent of the language and we instantiate each language in the lexicon of the knowledge base.

The second part is predicting the intention behind the query, which implies doing semantic query understanding, using the same semantic processing of documents. After, based on all this information, we must predict one or more possible intentions with a certain probability, which is particularly important for ambiguous queries. These scores will be one of the inputs for the final semantic ranking. For example, given the query ``bond'', possible results for query understanding are a financial instrument, the movie character, a chemical reaction, or a term for endearment.

Semantic ranking refers to ordering search results by relevance using semantic information. In a standard search engine, a rank is computed by using signals or features coming from the search query, from the documents in the collection being searched, and from the search context, such as the language and device being used. In our case, we add semantic relations between the entities and concepts found in the query with the same objects in the documents, that will come from different data sources. For this we use machine learning in several stages. The first stage selects the data sources that we should use to answer the query. In the second stage, each data source generates a set of answers using ``learning to rank.'' The third and final stage ranks these data sources, selecting and ordering the intentions as well as the answers inside each intention (e.g., news) that will appear in the final composite answer. All these stages are language independent, but may use language dependent features. For more details on the query processing phase see [[1](https://dl.acm.org/citation.cfm?id=3096472)].

SHORT BIOGRAPHY
------

Ricardo Baeza-Yates areas of expertise are web search and data mining, information retrieval, data science and algorithms. Since June 2016, he is CTO of NTENT, a semantic search technology company based in California, USA. Before he was VP of Research at Yahoo Labs, based in Barcelona, Spain, and later in Sunnyvale, California, from January 2006 to February 2016. He also is part time Professor at DTIC of the Universitat Pompeu Fabra, in Barcelona, Spain, as well as at DCC of Universidad de Chile in Santiago. Until 2004 he was Professor and founding director of the Center for Web Research at the later place. He obtained a Ph.D. in CS from the University of Waterloo, Canada, in 1989. He is co-author of the best-seller Modern Information Retrieval textbook published by Addison-Wesley in 2011 (2nd edition), that won the ASIST 2012 Book of the Year award. From 2002 to 2004 he was elected to the Board of Governors of the IEEE Computer Society and between 2012 and 2016 was elected for the ACM Council. Since 2010 is a founding member of the Chilean Academy of Engineering. In 2009, he was named ACM Fellow while in 2011 IEEE Fellow, among other awards and distinctions.

References
---

[[1](https://dl.acm.org/citation.cfm?id=3096472)] Ricardo Baeza-Yates, “Semantic Query Understanding,” SIGIR 2017 Industrial Track, Tokyo, Japan, 2017.
Hannah Bast, Björn Buchhold, and Elmar Haussmann,

[[2](http://www.nowpublishers.com/article/Details/INR-032)] “Semantic Search on Text and Knowledge Bases,” Foundations and Trends in Information Retrieval 10(2-3): 119-271 (2016).
