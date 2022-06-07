## protein-protein network data

#### protein information
+ **node with go information**: go\_slim\_mapping.tab.txt
    + P for biological process(Bp) 
    + F for molecular function(Mf)
    + C for cellular component(Cc)
    + Since GO slims of Cc include some protein complexes information, only select Bp and Mf
+ **complex protein**: golden\_standard.txt
    + at leat 3 proteins in one complex protein


#### source data (for example: `COLLINS/`)
+ **node data with go tags**: collins\_go\_information.txt
+ **edge data**: collins.txt
+ **adj data**: Network\_collins.txt
    + node index by **node order** in collins\_go\_information.txt
+ **feature data**: Attribute\_collins.txt

#### generate graph embedding
+ **graph embedding**: collins\_attr\_vector.txt
+ **simiarity in node embedding with edge**: collins\_attr\_vector.txt
    + (node_1 node_2 similarity_score)
    + cosine similarity between nodes embedding
    + to build weight adj for finding cliques