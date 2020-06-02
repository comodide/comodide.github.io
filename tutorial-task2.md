# CoModIDE Tutorial Task 2

Your task is to develop an ontology for describing the steps of a recipe, using CoModIDE and three provided patterns from the MODL pattern library.

The user story is as follows:

> This is a knowledge graph containing recipes, ingredients, and preparatory equipment. Types of Equipment can be added to the ontology without changing the subsumption hierarchy. These recipes discriminate between Preparation Steps and Timed Steps. They also have categories and estimated times to complete. An excerpt is provided.

>"Amazing Spaghetti" (30 minutes).
> 1. Grab 1 Tbsp of fennel
> 2. (Excerpt)...
> 3. Boil the spaghetti for 12 minutes.
> 4. (Excerpt)...
> 17. Enjoy!


The resulting ontology should be able to answer the following competency questions, derived from the story above.

1. What are the steps in example:recipeXX? (*Trajectory* Pattern)
2. How long will it take to complete example:recipeXX? (no pattern)
3. How long do I need to boil the pasta in the 3rd step? (*Temporal Extent* Pattern)
4. What types of equipment are needed to complete this recipe? (*Explicit Typing* Pattern)
5. How much fennel is needed in example:recipeXX? (*Quantities and Units*)

For this task, we recommend to use the following CoModIDE settings:

* **Entity naming:** use target namespace
* **Module annotations:** external
* **Edge creation axioms:** OWLSomeValuesFrom / OWLAllValuesFrom
* **Edge deletion policy:** delete property declarations
* **Send Telemetry:** your choice, but we would definitely appreciate if you would have it checked

Use the CoModIDE pattern library to drag and drop patterns, renaming classes as needed to suit the use case. If you need to reconnect object properties (i.e. change their `rdfs:domain or `rdfs:range), please drop back into the standard Protege tabs -- this feature is not fully implemented in CoModIDE, yet.

An example solution can be [downloaded here](tutorial-task2-solution.ttl) and [visualized here](http://www.visualdataweb.de/webvowl/#iri=https://comodide.com/tutorial-task2-solution.ttl)
