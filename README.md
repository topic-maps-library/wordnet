# Topic Map WordNet
This repository contains a project for Wandora application. The project is a collection of topic maps that build up the WordNet, a large lexical database for English. The WordNet has been developed at the Cognitive Science Laboratory of Princeton University and the topic map conversion is based on W3C's work on RDF version of the WordNet 2.0.

## Details

The topic map conversion of WordNet was originally published in WandoraWiki (http://wandora.org/wiki/Topic_map_conversion_of_WordNet). This version contains slightly modified version of the original project: The glossary is now included in the project as 12th layer and subject identifiers have been changed to comply Wandora's current core ontology.

The WordNet project includes 12 topic map layers, each containing part of the complete WordNet. Included topic map layers are
* Base layer (layer0) contains Wandora's base ontology. 
* Layer wordnet-basics (layer1) builds a simple instance-of hierarchy including all association types and classes, and attaches this hierarchy under Wandora's base ontology. Motivation of this layer is merely a navigational. It is easier to access WordNet when topics and associations are in Wandora's topic tree.
* Wordnet-synset (layer2) contains all words in WordNet divided into separate synset categories. Each word topic has single subject identifier, base name, and English variant name. This layer does not contain associations between word topics.
* Wordnet-similarity (layer3) contains all Similar to (wordnet) associations between word topics. Layer contains also association type and role topics. Also such word topics are included that play a role in Similar to (wordnet) associations. Included word topics are topic stubs. They have only one subject identifier that merges the stub to the full word topic in wordnet-synset layer. 
* Wordnet-part-meronym (layer4) contains all PartMeronymOf (wordnet) associations between word topics. Layer contains also association type and role topics. Also such word topics are included that play a role in PartMeronymOf (wordnet) associations. Included word topics are topic stubs. They have only one subject identifier that merges the stub to the full word topic in wordnet-synset layer. 
* Wordnet-member-meronym (layer5) contains all MemberMeronymOf (wordnet) associations between word topics. Layer contains also association type and role topics. Also such word topics are included that play a role in MemberMeronymOf (wordnet) associations. Included word topics are topic stubs. They have only one subject identifier that merges the stub to the complete word topic in wordnet-synset layer. 
* Wordnet-hyponym (layer6) contains all HyponymOf (wordnet) associations between word topics. Layer contains also association type and role topics. Also such word topics are included that play a role in HyponymOf (wordnet) associations. Included word topics are topic stubs. They have only one subject identifier that merges the stub to the complete word topic in wordnet-synset layer.
* Wordnet-classified-by (layer7) contains all ClassifiedByRegion (wordnet), ClassifiedByTopic (wordnet), and ClassifiedByUsage (wordnet) associations between word topics. Layer contains also association types and role topics. Also such word topics are included that play a role in listed associations. Included word topics are topic stubs. They have only one subject identifier that merges the stub to the complete word topic found in wordnet-synset layer. 
* Wordnet-attribute (layer8) contains all Attribute (wordnet) associations between word topics. Layer contains also association type and role topics. Also such word topics are included that play a role in Attribute (wordnet) associations. Included word topics are topic stubs. They have only one subject identifier that merges the stub to the complete word topic in wordnet-synset layer. 
* Wordnet-causes (layer9) contains all Causes (wordnet) associations between word topics. Layer contains also association type and role topics. Also such word topics are included that play a role in Causes (wordnet) associations. Included word topics are topic stubs. They have only one subject identifier that merges the stub to the complete word topic in wordnet-synset layer. 
* Wordnet-entailment (layer10) contains all Entails (wordnet) associations between word topics. Layer contains also association type and role topics. Also such word topics are included that play a role in Entails (wordnet) associations. Included word topics are topic stubs. They have only one subject identifier used to merge the stub to the complete word topic. 
* Wordnet-same-verb-group-as (layer11) contains all SameVerbGroup (wordnet) associations between word topics. Layer contains also association type and role topics. Also such word topics are included that play a role in SameVerbGroup (wordnet) associations. Included word topics are topic stubs. They have only one subject identifier used to merge the stub to the complete word topic. 
* Wordnet-glossary (layer12) contains textual description for all word topics i.e. each word topic contains an occurrence that describes the word.

## Usage

You can clone the repository and use enclosed topic maps in any application supporting XTM topic maps. To clone the repository project in Wandora use menu option File > Git > Clone remote repository... and enter repository's clone url to the dialog. 

## See
* https://en.wikipedia.org/wiki/Topic_Maps
* http://www.wandora.org
* http://wandora.org/wiki/Topic_map_conversion_of_WordNet#WordNet_license