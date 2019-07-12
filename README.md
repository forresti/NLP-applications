# NLP-enabled applications, and their underlying technology 

## Semi-automated customer service (human in the loop at call center or on text chat)
* [Assist a human service representative in coming up with answers](https://venturebeat.com/2018/09/29/investing-in-ai-when-natural-language-processing-pays-off/) - Question Answering and Language Modeling (next sentence prediction)

## Fully-automated customer service (chatbot - with a text or voice interface)
* Question answering
* "Similar question finding" - seems like something we could do with today's NLP 

## Fuzzy procedural voice agent
* It seems like we should be able to train NLP to do the following. We have a fixed list of possible intents (check weather, order an item, or none of the above). We teach a model to recognize these intents in text strings. For this, perhaps we could formulate it as a Reading Comprhension task, where each of these intents is a potential interpretation of the sentence.
    * Then, if intent is "order an item," the next step is to recognize the name of the item based on an unscripted sentence.
    * Or, if the intent is "check weather," if it's not already clear which location is interested in, we would recognize a zip code in an unscripted sentence.

## Other chatbot stuff
* See figure 2 from the [CMU entrant](https://m.media-amazon.com/images/G/01/mobile-apps/dex/alexa/alexaprize/assets/pdf/2018/Tartan.pdf) to the Alexa Challenge 2018. It includes Intent, Topic, Sentiment, Named Entity Recognition, Neural Generation -- all things I believe today's DNN-enabled NLP can do.

## Phobias
* Could we use NLP to detect references to common phobias (e.g. spiders) or personalized phobias? Then, we could remove these from search results, or make it "click to look," or something like that? Intuitively, it seems like Topic Modeling could help us with this.

## Predict next letter, word, or sentence that the user will type (e.g. in google search or in an email)
* Language models do this
* Can be useful offline -- e.g. in MS Word on airplane, or on a the keyboard of a phone with poor internet

# An incomplete list of NLP datasets and tasks
* SQuAD
* RACE dataset
* Text classification datasets used in [XLNet paper](https://arxiv.org/pdf/1906.08237.pdf): IMDB, Yelp-2, Yelp-5, DBpedia, AG, Amazon-2, Amazon-5
* [Author Identification using BooksCorpus data](https://www.kaggle.com/jinsooyeo/author-identification-using-toronto-book-corpus) (and recommending similar authors)
* [GLUE](https://gluebenchmark.com/tasks)
    * [Multi-Genre Natural Language Inference (MNLI)](http://www.nyu.edu/projects/bowman/multinli/) - "crowd-sourced collection of 433k sentence pairs annotated with textual entailment information"
    * QNLI - GLUE page links to SQuAD 2.0?
    * [Quora Question Pairs (QQP)](https://data.quora.com/First-Quora-Dataset-Release-Question-Pairs)
    * [Recognizing Textual Entailment (RTE)](https://aclweb.org/aclwiki/Recognizing_Textual_Entailment)
    * [Stanford Sentiment Treebank (SST-2)](https://nlp.stanford.edu/sentiment/index.html) - [demo](http://nlp.stanford.edu:8080/sentiment/rntnDemo.html)
    * [Microsoft Research Paraphrase Corpus (MRPC)](https://www.microsoft.com/en-us/download/details.aspx?id=52398)
    * [Corpus of Linguistic Acceptability (CoLA)](https://nyu-mll.github.io/CoLA/)
    * [Semantic Textual Similarity Benchmark (STS-B)](http://ixa2.si.ehu.es/stswiki/index.php/STSbenchmark)
    * [WNLI - aka Winograd Schema Challenge (WSC)](https://cs.nyu.edu/faculty/davise/papers/WinogradSchemas/WS.html)
* [SuperGlue](https://super.gluebenchmark.com/tasks)
    * AX
    * [CommitmentBank (CB)](https://github.com/mcdm/CommitmentBank)
    * [Choice of Plausible Alternatives (COPA)](http://people.ict.usc.edu/~gordon/copa.html) - Causal Reasoning
    * [MultiRC](https://cogcomp.org/multirc/) - Reading Comprehension over Multiple Sentences. (Read a passage, then respond to a set of True/False statements.)
    * [Recognizing Textual Entailment (RTE)](https://aclweb.org/aclwiki/Recognizing_Textual_Entailment) - "This task requires to recognize, given two text fragments, whether the meaning of one text is entailed (can be inferred) from the other text."
    * [WiC: The Word-in-Context Dataset](https://pilehvar.github.io/wic/) - "The task is to identify if the occurrences of w in the two contexts correspond to the same meaning or not."
    * [Winograd Schema Challenge (WSC)](https://cs.nyu.edu/faculty/davise/papers/WinogradSchemas/WS.html) - 
