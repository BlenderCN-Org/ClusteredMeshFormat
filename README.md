# ClusteredMeshFormat
An experimental mesh format


A Blender addon that exports/imports to my clustered mesh format.


This format seperates vertices into a 3D grid, each grid cube is called a cluster. 


By doing this, vertices can be compressed to 1 byte per component, instead of the typical 4. This also allows indices to be referenced in "cluster space", saving space there too. This comes with some precision loss, but it's still very suitable for lower poly models!


*Note*: Because this format was created as an expariment, it only supports material indices. If you plan on using this, you'll have to create some material management/export system.