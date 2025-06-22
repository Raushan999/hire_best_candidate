# Problem statement:
To find the candidates best suited for a job requirement based on their skills and background.

### How to decide the best candidate out of the large pool of candidates.

* Implementing the following hierarchy for deciding most suited candidate for a given tech role. 
1. work experience(total work years, tech stack, company, role) >> Education(T1 > T2 > T3) >> 
 Github activity score (Total repo, relevant languages, followers, past 6 month active days) >>
 (kaggle, leetcode, codeforces, codechef, hackerrank etc) profiles >> Activity on our platform....


HYBRID SEARCH IMPLEMENTATION:::

Hybrid search
Semantic search and lexical search are powerful information retrieval techniques, but each has notable limitations. For example, semantic search can miss results based on exact keyword matches, especially in scenarios involving domain-specific terminology, while lexical search can miss results based on relationships, such as synonyms and paraphrases.

### Steps: 
1. Filteration
    - Add filterations like: 
    filter = 
    {"age":$?, 
    "salary": $?, 
    "location": $?, 
    "skills": $?, 
    "fulltime": $?(0,1), 
    "Immediate": $?(0,1),
    "Notice_period": $?, 
    "colleg": $?, 
    }
2. Retriever:- 
    - 
    vectorstore.similarity_search(
    "User_query",
    k=5,
    filter=filter,
)



## Last Phase:-
1. Work on desining a descent UI for the recruiters to see the candidates details.