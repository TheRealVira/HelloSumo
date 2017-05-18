# Hello Sumo

Hello Sumo is a test project, based on the tutorial [Hello_Sumo](http://sumo.dlr.de/wiki/Tutorials).

## NOTE:
| File Extension | Definition |
| ------------- | ------------- |
| `.nod.xml`  | Nodes  |
| `.edg.xml`  | Edges  |
| `.net.xml`  | Network (combinding edges and nodes)  |
| `.rou.xml`  | Route (a vehicle, which drifes on a specified route on the network)  |
| `.sumocfg`  | Specifies the parameters for the simulation  |
| `.settings.xml`  | Specifies external (not actively changing the simulation) parameters, like the viewport as an example  |

While `.sumo.cfg` is not visible declared as an xml file, the content inside uses normal xml syntax.

## HowTo

| Task | Command |
| ------------- | ------------- |
| Creating a network (based on nodes and edges).  | `netconvert --node-files=[NAME].nod.xml --edge-files=[NAME].edg.xml --output-file=[NAME].net.xml`  |
| Starting the simulation | `sumo -c [NAME].sumo.cfg`  |
| Starting the simulation (with GUI)  | `sumo-gui -c [NAME].sumo.cfg`  |