PyTraceGraph
=============

Generate graphs from any trace files

# Requirements #
	
	* graphviz 
	* pydot

# Usage #

**Generate only call graphs:**
	
`python pytracegraph.py -n nodes.txt -e edges.txt -p MyParser.simpleParser -w new_conceptual_model.png`

**Generate reflexion model:**

`python pytracegraph.py -n nodes.txt -e edges.txt -p MyParser.simpleParser -w new_reflexion_model.png`</br>
`-r call_trace.txt -rp MyReflexionBuilder.simpleReflexionBuilder`	 

PyTraceGraph Class Diagram
-------

![PyTraceGraph Class Diagram](http://tomazeli.net/images/pytracegraph_arch.png "Class Diagram")

