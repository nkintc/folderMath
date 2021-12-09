# Making the Folds

Fold objects are readily available as .obj files. Once successfully loaded into origami simulator, an object file at any particular fold percentage is readily available. But due to their simplistic nature and inherently planar structure, it is a non trivial process to import onto many programs. However, Blender is a robust program with interface to manipulate the mesh network.&#x20;

If an object file from origami simulator is directly loaded into a FDM slicing program such as Cura, the program will certainly throw an error which states that some (in this case, all) faces are [non manifold](https://community.ultimaker.com/topic/32250-not-manifold/). From the slicer's point of view, it is attempting to   create a tool path which traces out the volume of the sheet. However, the surfaces do not enclose a volume which incurs the non manifold error.&#x20;

However, once an obj is exported from origami simulator it can be opened in Blender which readily accepts mesh networks.&#x20;

![Extruded fold object saved as a blend object. ](<.gitbook/assets/image (2).png>)



Printed&#x20;

![](<.gitbook/assets/image (8).png>)

* Orient the model along a plane
  * since the exported fold file is only very partially in the process of being folded, most of the points remain mostly coplanar.&#x20;
* &#x20;

Select all nodes and edges, tab into edit mode and extrude

There are multiple options to extrude however in a direction normal to the selected plane

Each side is identical and once cut will mate toward one another.&#x20;
