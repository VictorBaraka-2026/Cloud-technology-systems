## 📅 Day 1: November 6, 2026 | Navigation Basics
* **command:** `pwd` -> Print Working Directory
* **expectation:** To show me the working folder
* **command output:** `/root`
* **command:** `mkdir` -> Make Directory 
* **expectation** -> to create a folder 
* **output** -> `root@ubuntu:~/victry$`
* **command:** `ls` -> List everything 
* **expectation** Shows files inside a room
* **output** `filesystem  victry`
* **command:** `cd` -> Change Directory 
* **expectation** -> Steps inside a folder
* **output** -> `:~/victry$`
* **command:** `clear`
* **expectation** -> Clean the clutter off the screen
* **output** -> `root@ubuntu:~$`

## 📅 Day 1: November 6, 2026 | Navigation Basics

### 🧠 Core Concepts Learned
* **Network Switch Fundamentals:** Learned how a Layer 2 switch operates at the Data Link layer, utilizing MAC addresses to intelligently forward frames only to the intended destination, preventing network collisions.
* **CLI Navigation:** Mastered navigating between User EXEC mode (`Switch>`), Privileged EXEC mode (`Switch#`), and Global Configuration mode (`Switch(config)#`).

### 💻 Lab Verification & CLI Diagnostics

| Date | Command | Expectation (What it does) | Output / Results |
| :--- | :--- | :--- | :--- |
| Nov 6, 2026 | `enable` | Navigates from User EXEC mode to Privileged EXEC mode to unlock diagnostic commands. | `Switch>`<br>`Switch#` |
| Nov 6, 2026 | `show mac address-table` | Displays the switch's CAM table mapping physical ports to device MAC addresses. | `Vlan  Mac Address     Type     Ports`<br>`----  -----------     ----     -----`<br>`1     0060.2f6b.5501  DYNAMIC  Fa0/1`<br>`1     00d0.ba3c.77a2  DYNAMIC  Fa0/2` |
| Nov 6, 2026 | `show ip interface brief` | Provides a quick status summary of all physical interfaces (ports) and their protocol states. | `Interface       Status  Protocol`<br>`FastEthernet0/1  up      up`<br>`FastEthernet0/2  down    down`<br>`Gigabit0/1      down    down` |
| Nov 6, 2026 | `show running-config` | Dumps the active, volatile configuration currently running in the switch's RAM. | `Current configuration : 1054 bytes`<br>`!` <br>`hostname Switch`<br>`!`<br>`interface FastEthernet0/1`<br>`!` |

### 📸 Lab Network Topology
*(Upload a screenshot of your Packet Tracer topology to your repo and name it topology.png)*
![Network Topology](topology.png)

### 🛠️ Tools Used
* Cisco Packet Tracer (Network Simulation)
* Cisco IOS (Command Line Interface)

