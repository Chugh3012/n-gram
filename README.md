# n-gram

## Objective
1. Obtain the frequency of occurences of all the unique 3-grams, 5-grams and 7-grams system call sequences in the Training data for both Attack data (across all categories of attack) and Normal data.
2. Obtain the top 30% n-gram terms with the highest frequency of all the unique n-gram terms in the training data to create a data set.(This will be final training data used to train various classifiers)
3. Applying similar procedure to obtain final Test data set.

## Overview
Host-based intrusion detection systems (HIDSs), especially anomaly-based, have received much attention over the past few decades. Over time, however, the existing data sets used for evaluation of a HIDS have lost most of their relevance due to the substantial development of computer systems. To fill this gap, ADFA Linux data set (ADFA-LD) is recently released. Six types of attacks occur in ADFA-LD including two brute force password guessing attempts on the open ports enabled by FTP and SSH respectively, an unauthorised attempt to create a new user with root privileges through encoding a malicious payload into a normal executable, the uploads of Java and Linux executable Meterpreter payloads for the remote compromise of a target host, and the compromise and privilege escalation using C100 webshell. These types are termed as Hydra-FTP, Hydra-SSH, Adduser, Java-Meterpreter, Meterpreter and Webshell respectively.

Once we obtain the Training and Test data sets for unique n-gram we implement a simple k nearest neighbour (kNN) to develop new host-based anomaly detection systems (HADSs).

