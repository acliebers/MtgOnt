# MtgOnt
[Magic: The Gathering](https://magic.wizards.com/en) is the premier trading card game, in which players collect, trade, and build decks of cards which they use to play against eachother in competitive games. As of February 2024, there are about 27,000 unique cards which players may use in the various formats of this game, and a [comprehensive rulebook](https://media.wizards.com/2024/downloads/MagicCompRules%2020240802.pdf) of over 200 pages. As such, there is a huge, constantly growing body of information about the game which most casual players only know a fraction of. This repo is intended to serve as a space for the development of a [BFO-conformant](https://github.com/BFO-ontology/BFO-2020) ontology of Magic: the Gathering with the aim of creating a knowledge graph containing representations of Magic cards and decklists for the purpose of querying and automated reasoning.  

# Scope 
MtgOnt asserts classes and relations corresponding to the entities described in the [Comprehensive Rules](https://media.wizards.com/2024/downloads/MagicCompRules%2020240802.pdf) as subclasses of existing classes within the top-level ontology, [BFO](https://github.com/BFO-ontology/BFO-2020), and/or the mid-level ontology suite extending from BFO, [CCO](https://github.com/CommonCoreOntology/CommonCoreOntologies). 

# Methods 
Definitions (and axioms) are derived from Magic's comprehensive Rules with an eye towards the BFO's realist ontological stance. This modeling strategy actually simplifies some of the rules descriptions contained in the Comprehensive Rules, which often refer to game-related entities like cards as representing other entities of particular classes when we can instead understand them simply as those entities. From an ontological standpoint, this is both a pragmatic and likely more accurate modeling method, because (a) it reduces the size of the ontology (and therefore prevents an explosion in the size of knowledge graphs using the ontology) and (b) it adheres to a loose standard of ontological parsimony. 

However, there is a concern in the offing which is worth considering. As much of the complexity of strategy games like Magic derives from complex interactions of cards on the basis of their encoding rules information, we must be careful to choose when and where it is important or permissible to engage in this simplification, and where it is important to allow the complexity of Magic's robust rules system to demand complexity of the MtgOnt. Similarly, the relationship between information that different cards (ad other game objects) bear and the game-mechanical roles/qualities/dispositions of those cards requires detailed analysis for the purpose of ontological elucidation/modeling. 


 
# Use of MtgOnt
As MtgOnt is extended from BFO and CCO (in the sense that all of the highest-level classes of MtgOnt are subclasses of classes asserted in BFO or CCO), it should be implemented only with BFO and CCO imported. A MIREOT containing necessary terms from both ontologies will be added to this repo at some point. 

MtgOnt is intended to be used to:

(1) Structure information about individual Magic: the Gathering cards

(2) Support symbolic reasoning about games of Magic: the Gathering

(3) Structure information about decks and strategies in the various formats of Magic: the Gathering 
     

