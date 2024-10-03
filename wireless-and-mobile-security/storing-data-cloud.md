storage area network - a hardware device compliled of a high number of fast disks

this is where data is stored , the cloud if you will, and to connect to this:
fibre channel - fast but expensive
ISCSI connector - cheaper option

Data should be stored within its own region - europe business in europe etc

for large amounts of data = binary large object storage - needs permissions to view - encrypts data ( RSA 2048 or BLOB storage )


when storing data in the cloud, multiple copies should be made and secured incase of data corruptiom, loss of data, comprimise of data
types of replication:
- LRS ( local redundant storage ) - having 3 different copies of data in the same physical location
- ZRS ( zone RS ) - 3 copies split into different zones within the same region
- GRS ( geo ) - 3 copies in the same physical location but an extra copy in an additional region
- G2RS ( GEO zone ) - 3 copies in 3 different physical location in one region, and an extra in secondary region


## security solutions
CASB ( cloud access security broker ) - software or hardware that sits between users and cloud service
App security - cloud WAF ( web application firewall ) and RASP ( runtime application self-protection = protects in real time like a IPS/IDS )
firewall

 
