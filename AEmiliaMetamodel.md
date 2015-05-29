# Introduction #

The metamodel (mmAEmilia.ecore) is composed by a set of meta classes and some external packages:

- **DataType**: it contains the data types (e.g. Integer, Real, Boolean, etc.) supported by the AEmilia ADL.

- **Expressions**: it contains the expressions (e.g. Arithmetical Expressions such as plus, minus, div, mult, etc. or Mathematical Expressions such as min, max, abs, mod, etc.) that can be specified in the AEmilia ADL.

- **Headers**: it contains the headers for both the ArchiType (AT\_Header) and the ElemType (ET\_Header) as well as for behavioral equations supported by the AEmilia ADL.

- **Behavior**: it contains a set of behavioral equations, their actions and the rates (exponential, immediate, passive) that can be specified in the AEmilia ADL.


To code the constraints imposed by the AEmilia ADL (e.g. each local interaction must be involved in at least one attachment), we implemented a set of [OCL rules](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/AEmiliaMetamodelConstraints.ocl) that allow us to validate the AEmilia specification and its corresponding model.


# Details #

The AEmilia metamodel: core elements and inner packages.


![http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmilia.png](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmilia.png)


![http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmiliaHeaders.png](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmiliaHeaders.png)

![http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmiliaBehavior.png](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmiliaBehavior.png)

![http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmiliaExpressions.png](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmiliaExpressions.png)

![http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmiliaDataType.png](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/mmAEmiliaDataType.png)