Input files:
np_node -> the modules are the nodes
np_edges -> the edges that connect the high-level model
np_dep.txt -> dependency between modules in txt format

Python Scripts:
pytracegraph.py -> the starting point of the application
Parser.py -> parsed the inputted text files
MyReflexionBuilder.py -> builds the reflexion model
node.py -> represents the module

Output Files:
np_high_level.png -> the theoretical high level model (When this is built change Node.py edge type to solid)
np_reflexion_model -> the final reflexion model

External libraries:
pydot-1.0.28
pyparsing-1.5.7

Commands:

	Build High-Level graph:
python pytracegraph.py -n nodes.txt -e edges.txt -p MyParser.simpleParser -w new_conceptual_model.png

	Build Reflexion model:
python pytracegraph.py -n nodes.txt -e edges.txt -p MyParser.simpleParser -w new_reflexion_model.png -r call_trace.txt -rp MyReflexionBuilder.simpleReflexionBuilder