# Mermaid-DDOS
## Description
- In this sequence diagram, the attacker sends a command to the bots in the BotNet to start the DDoS attack. The bots then flood the WebServer with too many requests. The WebServer detects the high traffic and alerts the Firewall. The Firewall blocks suspicious IP addresses to reduce the attack. Finally, the WebServer responds to the bots with an error message because it can’t handle the overload.
## DDoS Attack Sequence Diagram

```mermaid
sequenceDiagram
    participant Attacker
    participant BotNet
    participant WebServer
    participant Firewall

    Attacker->>BotNet: Send attack command
    BotNet->>WebServer: Flood with requests
    WebServer->>Firewall: Alert of high traffic
    Firewall-->>WebServer: Block suspicious IPs
    WebServer-->>BotNet: Respond with error

