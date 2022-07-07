# linguistic-drift
The meaning of words is constantly changing as a reflection of the society's evolution and cultural shift. Several studies have been exploring and analyzing this phenomenon, however, we are still lacking of robust visualization techniques that would ensure a proper understanding of linguistic drifts. Therefore, the aim of this project is to build new dynamic and scalable visualization methodologies that provide relevant insights regarding the mutation of the words' meanings over time. 
The study made use of the PubMed dataset, from which several article's abstracts of biomedical nature were extracted (using NLP preprocessing techniques) and divided into 6 time bins (70s, 80s, 90s, 00s, 10s and 20s). For all the words related to each period of time, we implemeneted the Word2Vec algorithm to create word emdeddings in order to calculate the word's context and similarities over time.
We were then able to create 3 different types of visualizations and compare them to the current ones, presented in semantic shift literature.
# The Dataset
We used data from PubMed https://pubmed.ncbi.nlm.nih.gov for the research, which consists of a large corpora of citations and abstracts related to biomedical literature collected in the National Library of Medicine. 

We retrieved the data as xml files via the FTP connection provided by the National Library of Medicine, and have included only articles from 1970 onward due to the unavailability of digitized abstract data for articles prior to that time period. Therefore, the study only focuses on linguistic drift observed in the last 50 years.

Using the entirety of the PubMed corpus available would require high computational and storage capabilities, and as such, we decided to use 106 out of the available 1114 xml files, selected to represent samples from all 52 years, and whose word embeddings would not benefit from additional data. 
