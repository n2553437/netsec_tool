<img width="868" height="869" alt="image" src="https://github.com/user-attachments/assets/216806b1-633d-4638-9a3c-58c9dab9e5c8" />
╔═══════════════════════════════════════════════════════════════════════════╗
║          Comprehensive Network Security Scanner v2.0                      ║
║                  Coded By:n2553437                                        ║
║                 email:n2553437@gmail.com                                  ║
║  Features: Packet Analysis • Vulnerability Scanning • OWASP Testing       ║
╚═══════════════════════════════════════════════════════════════════════════╝


  [!] No mode selected. Use -h for help

usage: netsec_tool.py [-h] [-c] [-s] [-full] [--count COUNT] [-t TARGET] [-p PORTS] [-w] [--packet-count PACKET_COUNT] [-e]

NetSec Toolkit - Comprehensive Network Security Suite

options:
  -h, --help            show this help message and exit
  -c, --capture         Packet capture mode
  -s, --scan            Vulnerability scan mode
  -full, --full         Full security assessment (scan + capture)
  --count COUNT         Number of packets to capture
  -t, --target TARGET   Target hostname or IP address
  -p, --ports PORTS     Port range (e.g., 1-1000 or 80,443,8080)
  -w, --web-scan        Enable web vulnerability scanning
  --packet-count PACKET_COUNT
                        Number of packets to capture in full mode
  -e, --export          Export results to files


═══════════════════════════════════════════════════════════════════════════
                              USAGE EXAMPLES
═══════════════════════════════════════════════════════════════════════════

Packet Capture:
  python netsec_tool.py -c --count 100 --export
  python netsec_tool.py -c --count 500

Vulnerability Scan:
  python netsec_tool.py -s -t example.com -p 1-1000 --export
  python netsec_tool.py -s -t 192.168.1.1 -p 80,443,8080
  python netsec_tool.py -s -t example.com -p 1-65535

Full Security Assessment:
  python netsec_tool.py -full -t example.com -p 1-1024 --packet-count 100 --export
  python netsec_tool.py -full -t example.com -p 80,443 --packet-count 50
