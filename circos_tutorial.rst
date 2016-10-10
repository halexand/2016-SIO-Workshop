======================================
Using and Installing Circos
======================================


The goals of this tutorial are to:

*  install circos on your Ubuntu AWS system 
*  use circos to visualize our data **fill me in **

Note: Beyond this brief crash course , circos is very well-documented and has a great series of `tutorials  <http://circos.ca/documentation/tutorials/>` and `course <http://circos.ca/documentation/course/>` materials that are useful. 

Installing Circos
==================================================

Within your Amazon Instance make a directory called circos and navigate into it. There, we will download and extract the latest version of circos: 
::
    mkdir circos
    cd circos
    wget http://circos.ca/distribution/circos-0.69-3.tgz 
    tar -xvzf circos-0.69-3.tgz 

Circos runs within Perl and as such does not need to be compiled to run. So, we can just add the location of circos to our path variable. (Alternatively, you can also append this statement to the end of your ``.bashrc`` file)  
::
    export PATH=export PATH=~/circos/circos-0.69-3/bin:$PATH
    
    
It does, however, require quite a few additional modules 

References:
===========


Acknowledgements:
=================

