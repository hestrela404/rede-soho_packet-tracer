# Diagrama da Topologia (Lógica)

```mermaid
graph TD
    subgraph "192.168.1.0/24"
        Server[("VM Server\n192.168.1.10\nDNS/HTTP/FTP")]
        PC1.comum["PC Comum\n192.168.1.11"]
        PC.pessoal.ele["PC Pessoal\n192.168.1.12"]
        Printer["Impressora SOHO\n192.168.1.20"]
    end
    
    subgraph "192.168.2.0/24"
        LaptopCorp.ela["Laptop Corporativo\n192.168.2.101"]
        SmartCorp.ela["Smartphone Corporativo\n192.168.2.102"]
        SmartPess.ela["Smartphone Pessoal Ela\n192.168.2.103"]
        SmartPess.ele["Smartphone Pessoal Ele\n192.168.2.104"]
        LaptopCorp.ele["Laptop Pessoal\n192.168.2.105"]
    end
    
    Gateway["Gateway\n192.168.1.1"]
    Switch0["Switch0"]
    
    Switch0 --- Server
    Switch0 --- PC1
    Switch0 --- PC2
    Switch0 --- Printer
    Switch0 --- LaptopCorp
    Switch0 --- SmartCorp
    Switch0 --- SmartPess
    Switch0 --- LaptopPess
    Switch0 --- Gateway
