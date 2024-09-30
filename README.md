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

### Documentation

**Description of the Sequence Diagram:**

1. **Attacker Sends Command:**
   - The attacker sends a command to the compromised bots (BotNet) to start the attack.

2. **Bots Flood the Server:**
   - The bots in the BotNet flood the targeted WebServer with an overwhelming number of requests.

3. **Traffic Alert:**
   - The WebServer detects unusually high traffic and sends an alert to the Firewall.

4. **Firewall Response:**
   - The Firewall analyzes the traffic and blocks suspicious IP addresses to mitigate the attack.

5. **Server Responds:**
   - The WebServer responds to the BotNet with an error message due to the inability to process legitimate requests.

### Submission

1. Commit and push your changes to your GitHub repository.
2. Submit the link to your `DDoS_Attack_Sequence.md` file in your class's assignment submission portal.

This simplified version should meet the assignment requirements while being easy to understand!
