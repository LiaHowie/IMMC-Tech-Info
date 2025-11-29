---
draft:
note: A draft page will not be shown in the production site
---
Below are the current specs for the server's hardware

# Server 1
### Services
- Discord Bot
- File Hosting
- BungeeCord
- Lobby 
- Limited Time Events 
- Dimensions Filming Server 
- Other Personal Projects
### Specs
Dell PowerEdge T110 II (modified)

| Part | Model                               |
| ---- | ----------------------------------- |
| CPU0 | Intel Xeon CPU E3-1270 V2 @ 3.50GHz |
| RAM  | 16GiB (4x4GiB) DDR3 1600MHz         |
| PSU  | 305W                                |
| sda  | Hitachi HDS72105 (512GB)            |
| sdb  | ST4000VX016-3CV1 (4TB)              |
| sdc  | SPCC Solid State (256GB)            |
| sdd  | SPCC Solid State (256GB)            |
- 5TB total storage 
- sda
	- OS
	- Other Services
- sdd
	- File Hosting
- sdc/sdd paired in ZFS Pool
	- Minecraft Instances

---
# Server 2 
### Services 
- Survival 
- Creative 
- Story 
- Test Servers 
### Specs 
HP Z600 Workstation (modified)

| Part | Model                          |
| ---- | ------------------------------ |
| CPU0 | Intel Xeon CPU X5650 @ 2.67GHz |
| CPU1 | Intel Xeon CPU X5650 @ 2.67GHz |
| RAM  | 48 GiB (6x8GiB) DDR3 1333MHz   |
| PSU  | 650W                           |
| sda  | WDC WD2003FYYS-0 (2TB)         |
| sdb  | Patriot P210 102 (1TB)         |
| sdc  | Patriot P210 102 (1TB)         |
- 4TB total storage
- sda
	- OS 
	- Other Services 
-  sdb/sdc paired in ZFS Pool 
	- Minecraft Instances