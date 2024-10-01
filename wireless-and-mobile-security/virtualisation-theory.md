### cloud concepts

hypervisor - install and run VMS inside of it
  type1 - run directly on hardware - VMwareESX
  type2 - needs OS to run - virtual box

sandboxing - malware isolated test environment
to protect a VM - IDS, scanning, patching

the problem with VM's are that they are easy to replicate
replicating a VM is copying, exporting and importing it = this can lead to VM escape attack which is a vulnerability inside hypervisor allowing attacker to break out of VM
to combat this employ patching

a system sprawl is when the vm takes more system resources than they should
vm moitoring should be in place here, ensuring it is patched and up to date
