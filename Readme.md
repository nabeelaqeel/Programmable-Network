### 1. What's the difference between the network's data model and its serialisation? Use your YAML and JSON files as the example.

Data Model : The underlying structure and organization of the network information 
Serialisation: The specific text format used to save that data structure into a file so it can be stored or read by a program.   

Example: topology.yaml and topology.json represent the exact same data model, but one is written in YAML format and the other in JSON format.  

### 2. Why was it better to catch the duplicate addresses in check() than with pingall? And what did IPv6 notice that IPv4 didn't?

Why check() is better: It inspects the network description before building and 
starting the network in Mininet, catching configuration errors instantly rather than failing 
later during runtime testing (pingall).   

What IPv6 noticed: IPv6 has Duplicate Address Detection (DAD). The kernel will flag as dadfailed for duplicated address


### 3. What does git diff give you that copying files into folders named topology-v2-final doesn't?

git diff automatically highlights the exact line-by-line changes (additions and deletions) between versions.
Copying files into folders like topology-v2-final only gives you static duplicate files without showing you what specific edits were made between them.