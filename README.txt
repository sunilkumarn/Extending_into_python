The project is done to extend the C module 'avl.c' into python so that it could be called from within python.
The 'swig' tool has been used for extending. Therefore before trying this out in your system you need to have swig installed.
'avl.i' is the interface file. The prototypes of all the functions that have used in 
'avl.c' have been placed here.
To extend the module into python: 
cd into the directory 'into_python' and Do :
$:make 
You will obtain a .so file in your directory. Now run the python interactive prompt andimport the module to use its functions:
python
>>>import avl
>>>avl.my_insert(10)
>>>avl.my_insert(20)....and so on.

If you want to clean up your directory ,do make remove.

