PyTraceGraph
=============

Generate graphs from any trace files

requirements:
	pydot

usage:
Generate only call graphs: 
	python pytracegraph.py -n nodes.txt -e edges.txt -p MyParser.simpleParser -w example3.png

Generate reflexion model:
	python pytracegraph.py -n nodes.txt -e edges.txt -p MyParser.simpleParser -w example3.png -r call_trace.txt -rp MyReflexionBuilder.simpleReflexionBuilder

PyTraceGraph Class Diagram
-------

<img src="http://tomazeli.net/images/pytracegraph_arch.png" />
