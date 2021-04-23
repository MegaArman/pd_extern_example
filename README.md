# pd_extern_example
Example external puredata objects in C. To build (Linux environments), simply run "Make" in the example's directory and open the PD patch to test it.

To summarize creating externs for PureData:

0. decide what you need at a conceptual level. An extern is useful if the PD GUI isn't allowing you to create an intuitive solution 
1. write the C code, you can use the helloworld example here as boilerplate
2. build your object with Make, can modify the helloworld example's
3. open a .pd patch that uses your object and wire it to what it needs to be wired to

NOTE: a pd object can't be named with spaces or hyphens, keep this in mind when calling gensym. You also need to name the functions with that symbol's name included, ex: ```helloworld_setup```

## helloworld 
you will see the pd patch contains a bang. Click the bang, then Window->Pd window to see the output. shows how to use inlets.

## counter
every time bang is hit, the outputted value increases. Shows how to use both inlets and outlets.

## References  

https://github.com/pure-data/externals-howto 

https://www.youtube.com/playlist?list=PLn3ODBv0ka5g_zKRpmgc58-Tj-Qn-P5qz
