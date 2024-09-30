# Mermaid-DDOS
# DDoS Attack Sequence Diagram

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
