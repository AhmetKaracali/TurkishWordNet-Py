# WordNet

A WordNet is a graph data structure where the nodes are word senses with their associated lemmas (and collocations in the case of multiword expressions (MWEs)) and edges are semantic relations between the sense pairs. Usually, the multiple senses corresponding to a single lemma are enumerated and are referenced as such. For example, the triple
􏰀

w<sup>5</sup><sub>2</sub>,w<sup>7</sup><sub>3</sub>,r<sub>1</sub>

represents an edge in the WordNet graph and corresponds to a semantic relation r<sub>1</sub> between the second sense of the lemma w<sup>5</sup> and the third sense of the lemma w<sup>7</sup>. The direction of the relation is usually implicit in the ordering of the elements of the triple. For synonymy, the direction is symmetric. For hypernymy, as a convention, the first sense is an hyponym of the second.

The main lexical source for KeNet is the Contemporary Dictionary of Turkish (CDT) (Güncel Türkçe Sözlük) published online and in paper by the Turkish Language Institute (TLI) (Türk Dil Kurumu), a government organization. Among other literary and academic works, the TLI publishes specialized and comprehensive dictionaries. These dictionaries are often taken as an authoritative reference by other dictionaries. The online version of the CDT contains 65,944 lemmas. Although the TLI publishes a separate dictionary of idioms and proverbs, the CDT still contains some MWE entries that have idiomatic senses.

## Data Format

The structure of a sample synset is as follows:

	<SYNSET>
		<ID>TUR10-0038510</ID>
		<LITERAL>anne<SENSE>2</SENSE>
		</LITERAL>
		<POS>n</POS>
		<DEF>...</DEF>
		<EXAMPLE>...</EXAMPLE>
	</SYNSET>

Each entry in the dictionary is enclosed by <SYNSET> and </SYNSET> tags. Synset members are represented as literals and their sense numbers. <ID> shows the unique identifier given to the synset. <POS> and <DEF> tags denote part of speech and definition, respectively. As for the <EXAMPLE> tag, it gives a sample sentence for the synset.


For Developers
============
You can also see either [Java](https://github.com/olcaytaner/TurkishWordNet) 
or [C++](https://github.com/olcaytaner/TurkishWordNet-CPP) repository.
## Requirements

* [Python 2.8 or higher](#python)
* [Maven](#maven)
* [Git](#git)

### Python 

To check if you have a compatible version of Python installed, use the following command:

    python -V
    
You can find the latest version of Python [here](https://www.python.org/downloads/).

### Maven
To check if you have Maven installed, use the following command:

    mvn --version
    
To install Maven, you can follow the instructions [here](https://maven.apache.org/install.html).      

### Git

Install the [latest version of Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

## Download Code

In order to work on code, create a fork from GitHub page. 
Use Git for cloning the code to your local or below line for Ubuntu:

	git clone <your-fork-git-link>

A directory called DataStructure will be created. Or you can use below link for exploring the code:

	git clone https://github.com/olcaytaner/TurkishWordNet-Py.git

## Open project with Pycharm IDE

Steps for opening the cloned project:

* Start IDE
* Select **File | Open** from main menu
* Choose `TurkishWordNet-Py` file
* Select open as project option
* Couple of seconds, dependencies with Maven will be downloaded. 


## Compile

**From IDE**

After being done with the downloading and Maven indexing, select **Build Project** option from **Build** menu. After compilation process, user can run TurkishWordNet-Py.
