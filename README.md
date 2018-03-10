# ryu-exercises
ryu simple exercises


Exercise1:
===========

Description: Layer2 Switch

This sample application available in the RYU apps.
Simple Layer2 Switch application, supports Openflow 1.3 Protocol.

The Openflow flow table Match constraints are 
in_port, eth_dst, eth_src


run the topology:
------------------------
sudo mn --controller=remote,ip=127.0.0.1 --mac --switch=ovsk,protocols=OpenFlow13 --topo=single,4 



run the exercise1 ryu app:
---------------------------
ryu-manager ex1_simple_switch_13.py



Exercise2:
===========

Description: Layer3 Switch

Update the simple layer2 switch application(Exercise1) with Layer3 Match constraints.

The Openflow flow table Match constraints are 
eth_type, ipv4_src, ipv4_dst


run the topology:
------------------------
sudo mn --controller=remote,ip=127.0.0.1 --mac --switch=ovsk,protocols=OpenFlow13 --topo=single,4 



run the exercise1 ryu app:
---------------------------
ryu-manager ex2_L3Match_switch.py





Exercise3:
===========

Description: Layer4 Switch

Update the simple layer2 switch application(Exercise1) with Layer4 Match constraints.

The Openflow flow table Match constraints are 
eth_type, ipv4_src, ipv4_dst, ip_proto, tcp_src/udp_src, tcp_dst/udp_dst


run the topology:
------------------------
sudo mn --controller=remote,ip=127.0.0.1 --mac --switch=ovsk,protocols=OpenFlow13 --topo=single,4 


run the exercise1 ryu app:
---------------------------
ryu-manager ex3_L4Match_switch.py




Exercise4:
===========

Description: Flow Timeout exercise

ex3_L4Match_switch.py is updated with the flow timeouts.

hard_timeout = 30
idle_timeout = 10 

run the topology:
------------------------
sudo mn --controller=remote,ip=127.0.0.1 --mac --switch=ovsk,protocols=OpenFlow13 --topo=single,4 


run the exercise1 ryu app:
---------------------------
ryu-manager ex4_flow_timeout.py




Exercise5:
===========

Description: Flow Priority exercise


run the topology:
------------------------
sudo mn --controller=remote,ip=127.0.0.1 --mac --switch=ovsk,protocols=OpenFlow13 --topo=single,4 


run the exercise1 ryu app:
---------------------------
ryu-manager ex5_flow_priority.py


Exercise6:
===========

Description: Multiple Tables 


run the topology:
------------------------
sudo mn --controller=remote,ip=127.0.0.1 --mac --switch=ovsk,protocols=OpenFlow13 --topo=single,4 


run the exercise1 ryu app:
---------------------------
ryu-manager ex6_multiple_tables.py



Exercise7:
===========

Description: ARP Proxy.  This application, builds and responds the ARP Response packets.  


run the topology:
------------------------
sudo mn --controller=remote,ip=127.0.0.1 --mac --switch=ovsk,protocols=OpenFlow13 --topo=single,4 


run the exercise1 ryu app:
---------------------------
ryu-manager ex7_arp_proxy.py

