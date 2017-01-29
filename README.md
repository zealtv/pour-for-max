# pour-for-max
#### x-platform wrapper for syphon and spout

**Pre reqs**

Syphon and/or Spout max packages.  Download these from Max's inbuilt package manger. 

**Usage**

Use pour.maxpat as an abstraction and pass it a GL context e.g [pour myContext].
Internally, the object will check host OS and create a Syphon or Spout object as appropriate.

Textures or matrices are accepted in the first inlet and are passed directly to the Spout or Syphon object.

Bangs to the second inlet will clear the objects internal state, deleting the Syphon or Spout object inside.  
This is useful in some case where you need to save the patch in a clean state. 
