
### `ip-addressing.md`

```markdown
# Tabela de Endereçamento IP

| Dispositivo                     | IP Address    | Gateway       | DNS           | Sub-rede        |
|--------------------------------|---------------|---------------|---------------|-----------------|
| VM Server (DNS, HTTP, FTP)     | 192.168.1.10  | 192.168.1.1   | 192.168.1.10  | 192.168.1.0/24  |
| PC Comum                       | 192.168.1.11  | 192.168.1.1   | 192.168.1.10  | 192.168.1.0/24  |
| PC Pessoal_ele                 | 192.168.1.12  | 192.168.1.1   | 192.168.1.10  | 192.168.1.0/24  |
| Impressora SOHO                | 192.168.1.20  | 192.168.1.1   | 192.168.1.10  | 192.168.1.0/24  |
| Laptop Corporativo_ela         | 192.168.2.101 | 192.168.1.1   | 192.168.1.10  | 192.168.2.0/24  |
| Smartphone Corporativo_ela     | 192.168.2.102 | 192.168.1.1   | 192.168.1.10  | 192.168.2.0/24  |
| Smartphone Pessoal_ela         | 192.168.2.103 | 192.168.1.1   | 192.168.1.10  | 192.168.2.0/24  |
| Smartphone Pessoal_ele         | 192.168.2.104 | 192.168.1.1   | 192.168.1.10  | 192.168.2.0/24  |
| Laptop Corporativo_ele         | 192.168.2.105 | 192.168.1.1   | 192.168.1.10  | 192.168.2.0/24  |

**Observações:**  
- Todos os dispositivos usam o mesmo gateway (`192.168.1.1`) e o mesmo servidor DNS (`192.168.1.10`).  
- O roteador com o IP `192.168.1.1` não está desenhado no diagrama, mas é o ponto de saída para outras redes.  
- A comunicação entre as sub-redes `192.168.1.x` e `192.168.2.x` depende do roteador/gateway.
