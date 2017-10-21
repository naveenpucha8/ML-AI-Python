# Anomalous Payload-Based Network Intrusion Detection

We present a payload-based anomaly detector, we call PAYL, for intrusion detection. 
PAYL models the normal application payload of network traffic in a fully automatic, unsupervised and very effecient fashion. 
We first compute during a training phase a profile byte frequency distribution and their standard deviation of the application payload flowing to a single host and port. 
We then use Mahalanobis distance during the detection phase to calculate the similarity of new data against the pre-computed profile. 
The detector compares this measure against a threshold and generates an alert when the distance of the new input exceeds this threshold.
We demonstrate the surprising effectiveness of the method on the 1999 DARPA IDS dataset and a live dataset we collected on the Columbia CS department network. 
In once case nearly 100% accuracy is achieved with 0.1% false positive rate for port 80 traffic.

