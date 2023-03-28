# internship_tasks

Some comments on my implementation: 
1) It is straightforward; it directly follows the pseudo-code in the attached article. 
2) The model itself does not include a predictive system. It just represents an inclusion of the graph into the Euclidean space. 
3) The hyperparameters used in my implementation are taken directly from the article.

---
4) I used a training method that was a little different than one in the article, because it was more effective in asymptotics.
Still, I believe that there are powerful changes that can be made with authors' approach
--- 
**UPD: An interesting observation. **

There is a paper "Distributed Representations of Words and Phrases and their Compositionality" 
(it is in that repo with name "word-to-vect arxiv"). It was published in 2013 and it builds a vector representation of words taken from some corpus.

Surprisingly when these words capture a relation in the world (like _"Lisbon is the capital of Portugal"_) the model prefers to represent them with similar shifts for each relation. 
i.e. the vector corresponding to the fact of Lisbon _being the capital_ of Portugal is almost the same to the same of Spain and Madrid. 

This is one-to-one similar to the approach taken by authors of "translating embeddings" and it is worth investigating their connections. 