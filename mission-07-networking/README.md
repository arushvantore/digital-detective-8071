# Mission 7 — How computers communicate

## 1. Task / objective
Define core computer networking concepts, run safe connectivity and DNS lookup tests on a public domain (`example.com`), and trace how a web browser loads a website.

## 2. Work completed

### Task 7.1 — Understand core network concepts

| Concept | Explanation in your own words | Example |
| :--- | :--- | :--- |
| LAN (Local Area Network) | A small network connecting devices within one room, home, hostel, or office building. | Devices connected to the same hostel Wi-Fi router. |
| MAN (Metropolitan Area Network) | A medium-sized network spanning across a single city or large university campus. | A city-wide fiber network linking multiple college campuses. |
| WAN (Wide Area Network) | A massive network connecting LANs and MANs across countries and continents. | The global Internet. |
| DNS (Domain Name System) | The phonebook of the internet that translates human-readable website names into numeric IP addresses. | Translating `example.com` into `104.20.23.154`. |
| Router | A networking device that directs data packets between your local network and the wider internet. | A home/hostel Wi-Fi router forwarding web requests to the ISP. |
| Protocol | A shared set of rules that defines how devices format, send, and receive data over a network. | HTTPS for secure web pages or DNS for domain lookups. |
| Packet switching | Breaking large messages into small numbered packets that travel independently across the network and reassemble at the destination. | Streaming a video or loading a webpage over the internet. |
| Client-server model | A communication setup where a client device requests data or services and a remote server processes and responds to that request. | A web browser (client) requesting a webpage from GitHub's web server. |

---

### Task 7.2 — Observe basic network behavior
- **Connectivity test (`ping -c 3 example.com`):**
  - **What it does:** Sends 3 small ICMP echo test packets to `example.com` (`104.20.23.154`) and measures how many packets return and how many milliseconds the round trip takes.
  - **Observation:** `3 packets transmitted, 3 packets received, 0.0% packet loss` with an average round-trip time of `14.629 ms` (`min 6.203 ms`, `max 27.019 ms`).
- **DNS lookup (`nslookup example.com`):**
  - **What it does:** Queries the configured DNS resolver (`8.8.8.8` on port `53`) to find the public IP addresses mapped to the domain name `example.com`.
  - **Observation:** Returned public IPv4 addresses `104.20.23.154` and `172.66.147.243` for `example.com`.

---

### Task 7.3 — Trace how a website loads
1. **User enters URL on the client:** I type `https://example.com` into my web browser, which acts as the **client**.
2. **DNS lookup resolves the IP address:** Because computers locate machines by numeric IP addresses, my device queries a **DNS** server to translate `example.com` into `104.20.23.154`.
3. **Router forwards the request:** My local **router** sends the connection request out from my local network onto the internet toward that destination IP address.
4. **Connection and protocol handshake:** Using standard networking **protocols** (TCP/IP and TLS/HTTPS), my **client** establishes a secure connection with the remote web **server**.
5. **Client sends HTTP request:** Following the HTTPS **protocol**, my browser sends an HTTP `GET` request asking the **server** for the webpage files.
6. **Server responds with data packets:** The **server** processes the request and sends back the HTML, CSS, and media broken into small **packets** across the network.
7. **Browser renders the webpage:** My **client** browser reassembles the incoming packets and displays the finished `example.com` webpage on my screen.

## 3. Commands / tools used
- `ping -c 3 example.com`: Tested network reachability and round-trip latency (`14.629 ms` average, `0%` packet loss).
- `nslookup example.com`: Queried DNS (`8.8.8.8`) to translate `example.com` into its public IP addresses (`104.20.23.154`, `172.66.147.243`).
- Git (`git add`, `git commit`, `git push`): Committed and pushed Mission 7 to GitHub.

## 4. My understanding
Computers communicate over networks by following shared protocols, breaking data into packets, and using routers and DNS to locate remote servers. Tools like `ping` and `nslookup` verify whether a server is reachable and how domain names map to IP addresses.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-07-networking/README.md`

## 8. Commit details
Committed with message: "Document networking concepts and DNS/ping observations" and pushed to GitHub.
