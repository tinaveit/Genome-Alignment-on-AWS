# Remove bootstrap using R

# Import libraries
library(phylogram)
library(ape)

# Create tree using Newick's format 
myTree <- ape::read.tree(text='((Homo_sapiens:0.0793732,Mus_musculus:0.0844682)0.970633:0.2343059,((Lepisosteus_oculatus:0.130925,Amia_calva:0.189194)0.640456:0.0391649,(Oryzias_latipes:0.121261,((Kryptolebias_marmoratus:0.0513167,Nematolebias_whitei:0.0863117)0.703993:0.0258997,Nothobranchius_furzeri:0.1190887)0.515438:0.0293196)0.471387:0.2025449)0.389323:0.0935769)0.819953;')


# make sure that tree is looking good
plot(myTree)

# remove bootstrap
myTree$node.label <- NULL

# save new file
write.tree(myTree, file = "MyTreeNoBoots.tre") 
