title: Machine learning for metadata standardization
author: Yuriy Sverchkov

----

# Machine learning for metadata standardization

## Metadata standardization

Often we encounter databases of items where these items are described by unstructured or semi-structured metadata.

For example
 * The sequence read archive (SRA)
 * Clinical notes
 * Others?

This creates a challenge for performing systematic tasks such as
 * finding items that fit certain parameters
 * creating summary statistics

Our goal is to develop a process to standardize the metadata to a structure that makes such tasks straightforward.

## Specific application: the SRA

The sequence read archive contains sequence reads associated with tissue samples

Example metadata:
-todo

## MetaSRA

A rule based system for
* Mapping metadata to ontology terms
* Determining cell type (?)

### Standardization goal:

show (metadata sample) -> (set of relation -to- ontology terms pairs)

### MetaSRA pipeline

Collect ontologies -> build text reasoning graph -> extract best paths to ontology terms

* Does not extract relations
* Domain-specific

## Research plan

1. Use ML or ML + domain agnostic rules to match/exceed the MetaSRA's performance on the ontology term extraction task
2. Extend our methods to the relation+term extraction task
3. Generalize to other domains

## Initial approach

Our task has variable-length input and variable-length output.
* There are approaches for handling this (looks like machine translation)
* We start with a simpler approach there we convert it to a simple classification task

### ML pipeline

1. Use a domain-agnostic text-matching pipeline to generate a set of candidate ontology term mentions for each sample
2. Extract features from the text reasoning path of each match
3. Apply off-the-shelf ML to classify the relation of each candidate mention

### Candidate mention text-matching pipeline

* Uses domain-agnostic rules from MetaSRA pipeline
* Focuses on maximizing recall (makes as many matches as possible, rather than trying to determine best)

### Features extracted

(paste from docs)

### Classifier performance

(specific terms binary task plot)

### Evaluation metrics for ontology terms

(insert definitions, and if possible, an illustration)

### Classifier performance - both plots

(specific terms and all terms plots)

### Classifier performance - multilabel task

(insert)

## Next steps?
