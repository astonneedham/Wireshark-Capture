# Wireshark-Capture
**Description:** Install Wireshark to capture packets to detect HTTPS and IP addresses using a display filter. Use Wireshark capture packets not containing specific IP addresses.

**Functionality:** The IT manager wants to be able to capture ethernet network web traffic on the server and be able to detect certain IP addresses as well.

**Solution:** Use Wireshark to capture packets on a certain interface and use filters to observe website traffic.

## Task 1
- Install and set up Wireshark on Ubuntu:

![Image](https://github.com/user-attachments/assets/44bb61cb-d5b4-4468-bfed-e31a6c560cd0)|
|:--:|
|*Wireshark Installed*|

## Task 2
- Start a packet capture on an ethernet port and save it to file:

## Task 3
- Use a display filter to detect HTTPS packets:
- Enter tcp.port==443 or tcp.port==80 in display filter field

![Image](https://github.com/user-attachments/assets/8dba2ca8-5b4e-4579-ac38-d6f2a0b271d1)|
|:--:|
|*Wireshark HTTP filter search*|

## Task 4
- Visit a web page and detect its IP address using a display filter:
- Visit Google.com,DuckDuckGo.com and Cygwin.com

## Task 5
- Locate all HTTPS packets from a capture not containing IP address: 8.43.85.97
- !(ip.addr==8.43.85.97) and (tcp.port==443 or tcp.port==80)Use display filter

![Image](https://github.com/user-attachments/assets/70ff00b5-7b4b-48a1-8db9-ca077db12771)|
|:--:|
|*Wireshark Display Filter*|
