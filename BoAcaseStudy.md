# Introduction #

Bus on Air (BoA) is a system aimed at developing a set of services for public transportation targeting both the end-users (passengers) and the suppliers (transportation agencies). We concentrate our analysis on the receiveBestPath service, i.e. the potential passenger arrives at the bus stop and has access to information on the best path to reach a destination, such as lines that cover a path, how long to wait, etc.


# Details #

The complete AEmilia architectural specification of the BoA system
(BoA.aem) along with its performance specification (BoA.rew) and the
performance results (BoA.val) have been reported in [Downloads/BoA-caseStudy.zip](http://code.google.com/p/panda-aemilia/downloads/detail?name=BoA-caseStudy.zip&can=2&q=#makechanges).

The detection tool gives as output the occurrence of three antipattern instances (i.e. Pipe and Filter Architectures, Extensive Processing, and Traffic Jam) that have been solved according to their solution specifications.
The solution of antipatterns gives rise to new AEmilia architectural specifications of the BoA system (BoA-P&F.aem, BoA-EP.aem, BoA-TJ.aem) that have been reported in [Downloads/BoA-caseStudy.zip](http://code.google.com/p/panda-aemilia/downloads/detail?name=BoA-caseStudy.zip&can=2&q=#makechanges). In the following we provide a graphical hint of such refactorings.

BoA - solution of the Pipe and Filter Architectures antipattern.

The behavior of Server\_Type is modified, since the retrieval of data from
servers to the database is conditioned by the presence of such data in the cache.

![http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/boa-pipeAndFilter.png](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/boa-pipeAndFilter.png)

BoA - solution of the Extensive Processing antipattern.

A further instance of Balancer\_Type (LBA, LBB: Balancer\_Type) has been added
to privilege the processing of fast requests despite slower ones.

![http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/boa-extensiveProcessing.png](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/boa-extensiveProcessing.png)

BoA - solution of the Traffic Jam antipattern.

The frequency of the database disk access is modified of 50%, from 150 MBps to 300 MBps, hence its processing power (data\_fetch\_rate) has been increased from 36.585 to 55.

![http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/boa-trafficJam.png](http://www.di.univaq.it/catia.trubiani/download/mmAEmilia/boa-trafficJam.png)