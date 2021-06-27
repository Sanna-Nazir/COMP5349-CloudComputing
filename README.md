# COMP5349: Cloud Computing

University of Sydney Coursework for COMP5349: Cloud Computing (Semester 1, 2020)

The assignment was completed as part of the COMP5329 unit of The University of Sydney by [Sanna Nazir](https://github.com/Sanna-Nazir) and [Anshu Kumar](https://github.com/anshukr5). 

There were two coding questions with two parts each, explained as below:

1. Vocabulary Exploration:
	
	1.1 You are asked to produce a few statistics of the vocabulary used in the corpus. Here, the vocabulary refers to the set of all the    words appearing in the corpus or in a subset of the corpus. No stemming or spelling check is needed to remove near duplicates or typos.
	The first set of workloads involves relatively small development and test data sets. There are four sets in total each with around 10K sentences. The matched development set and the matched test set contain sentence pairs in five genres. The mismatched development set and mismatched test set contain sentence pairs in five different genres. You are
	asked to find out:
		1. the number of common words between matched and mismatched sets
		2. the number of words unique to the matched sets
		3. the number of words unique to the mismatched sets

	1.2 The next set of workloads deals with the training data set. It contains sentence pairs from 5 genres. Among the vocabulary of the training set, there are common words appearing in all genres, and there could be words that only appear in one genre. You are asked to find out the distribution of common and unique words. To be specific, you are asked to find out:
		1. The percentages of words appearing in five genres, in four genres, in three genres, in two genres and in one genre
		2. The same percentages after removing a given list of stop words

2. Sentence Vector Exploration

Most text mining and NLP tasks start by converting the input document or sentence(s) into a vector. There are many ways to compute the vector representation of a sentence, from traditional vector space based TFIDF representation to simple averaging of word vectors
to complex neural models trained on very large corpus. A sentence vector is expected to be embedded with lots of semantic and syntactic information about the sentence. In this workload, you are asked to compare two sentence vector representation methods
based on their ability to captures the genre feature of sentences. The sentence vector representation methods are:
	
	2.1 TFIDF based vector representation. You should use the implementation provided by the Spark ML library. You can decide on the dimension of the vector.
	2.2 Pre-trained sentence encoder. You are recommended to use the Universal Sentence Encoder released by Google. The result would be a vector of 512 dimension. 

For each vector representation method, you are asked to encode every sentence in the training data set as a vector, then cluster all sentences into five clusters. Each cluster may contain sentences belonging to different genres. Ideally, there is one genre where most
sentences are from in that cluster. The cluster will be labelled with the genre that most sentences are from. After labeling each cluster, you are asked to compute the confusion matrix to show the accuracy of clustering using this particular vector representation. A confusion matrix shows for each label the percentage of correctly and incorrectly labelled data.


Further details of the assignment can be found in the ReadMe [here](./Final_Assignment/project_report.pdf).
Details to run each question code are present in the Readme of respective subfolders. 
