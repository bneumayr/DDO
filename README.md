# DDO
Domain Object Hierarchies inducing Multi-Level Models - Proof-of-Concept Prototype in F-Logic

This implementation of the DDO approach in F-Logic was developed and tested with Flora-2/ErgoLite Reasoner 2.0 (Pyrus nivalis) of 2018-10-14.

## How to run the prototype?
The Flora-2/ErgoLite system is necessary to run the prototype and is available at \url{http://flora.sourceforge.net/}.

1. Download the flr-Files into a directory and start Flora-2 from that directory.

2. Load the prototype either using

flora2 ?- [run_with_names].

or 

flora2 ?- [run_with_structures].

3. Query the multi-level model, for example, the following query will return all (obj,cls)-pairs where obj is a direct instance of cls. 

flora2 ?- ?obj [ iof -> ?cls ] .
