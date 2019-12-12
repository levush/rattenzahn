    The project rattenzahn wants to improve mausezahn as a stand alone tool
    which is compact and efficient and a good tool to be run on plastic
    routers like those supported by openwrt.
    So one can use an old plastic router, laptop or cheap embedded internet
    of shit device as a packet generator to do network measurements.
    
    Mausezahn has some flaws such as not sending packets if the payload file is
    too big or if it is not existent. Without payload file mz will segfault.
    At least this is what I found while using mausezahn for network tests
    floding a router with udp traffic in oder to find corrupted packets generated 
    by an overloaded router. Patterns in a payload file help to find causes for 
    corruptions in the software and/or hardware of a network device.
    Adding a parametric generator will help as counting patterns like 0x00, 0x01,
    0x02, ... 0xff, 0x00 are common for tests and so people don't need to write
    their payload files if the can just specify a simple pattern rule. 
    Also the performance should be improved as there are routers that contain
    test generators with better flooding performance.
    
    I know that there are "better" test generators but they are fat and blown
    and not as nice to the hardware as mz. 
    So I decided to improve mz to be rz, rattenzahn to be a small but effective 
    stand alone tool for network tests.   
 
    Especially the shell "mops" of mausezahn which is accessible using telnet 
    is very interesting and is something that needs to be improved and extended,
    as one can use an embedded device with rattenzahn as a network drone to do
    remote controlled network tests. Using an encrypted and authenticated 
    connection to mops is an important improvement, though.
    
    Hopefully rattenzahn, rz will be the better mausezahn.
    
    Levush, Tue Dec 10 2019

