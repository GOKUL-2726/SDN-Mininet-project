# SDN-Mini-project
# SDN Mininet Traffic Classifier

##  Project Description
This project demonstrates Software Defined Networking (SDN) using Mininet and Ryu Controller. It classifies network traffic into ICMP, TCP, UDP, and Other traffic types.

##  Tools Used
- Mininet
- Ryu Controller
- Python
- OpenFlow 1.3

##  How to Run

### Terminal 1:
ryu-manager ryu.app.simple_switch_13 traffic_classifier.py

### Terminal 2:
sudo mn --topo single,3 --controller=remote,ip=127.0.0.1,port=6653 --switch ovs,protocols=OpenFlow13

### Test:
h1 ping -c 3 h2

##  Output
- ICMP Traffic detected
- TCP Traffic detected
- UDP Traffic detected
- Other Traffic detected

##  Conclusion
This project successfully demonstrates traffic classification in an SDN environment.
