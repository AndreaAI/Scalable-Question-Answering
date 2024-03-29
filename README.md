# Scalable Question Answering

This repository contains the Python code implemented to process the LC-QuAD dataset and create the different files that are considered as datasets in the repositories [NER](../../../Named-Entity-Recognition) and [NEL](../../../Named-Entity-Linking).

## About SQA challenge

SQA (Scalable Question Answering) challenge over Linked Data consists of being able to translate a user’s information request into a format that can be efficiently evaluated using standard Semantic Web query processing and inferencing techniques. 
Therefore, the main task is the following: given an RDF dataset and a large volume of natural language questions or keywords, return the correct answers (or SPARQL queries that retrieves those answers).

## About LC-QuAD dataset

LC-QuAD (Large-Scale Complex Questions Answering Dataset) consists of 5000 questions along with the corresponding SPARQL queries required to answer those questions over DBpedia. The dataset includes complex questions, i.e. questions in which the intended SPARQL query does not consist of a single triple pattern.

How it was created: The question generation problem was framed as a transduction problem, 
in which KB subgraphs generated by the seed entity are fitted into a set of SPARQL templates which are then converted 
into a Normalized Natural Question Template (NNQT). This acts as a canonical structure which is then manually transformed into an NLQ having lexical and syntactic variations. Finally, a review is performed to increase the quality of the dataset.

Relevance for other research areas:

**◊	Entity and Predicate Linking:** The dataset can be treated as a set of questions, along with a corresponding list of entities and predicates present in it. There are 5000 total questions, 615 predicates and 5042 entities in the dataset.

**◊	SPARQL Verbalization:** The dataset can also assist the task of SPARQL verbalization, which has attracted research interest in the Semantic Web community

## About SPARQL

SPARQL is an RDF query language—that is, a semantic query language for databases—able to retrieve and manipulate data stored in Resource Description Framework (RDF) format. It was made a standard by the RDF Data Access Working Group (DAWG) of the World Wide Web Consortium, and is recognized as one of the key technologies of the semantic web. 

Basic SPARQL queries contain a set of triple patterns called a basic graph pattern. Triple patterns are like RDF triples, i.e. subject-predicate-object, except that each of the elements may be a variable. SPARQL allows for a query to consist of triple patterns, conjunctions, disjunctions, and optional patterns.
