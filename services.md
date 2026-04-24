# Serviços do Servidor VM (192.168.1.10)

O servidor virtual executa três serviços principais:

## DNS
- Resolve nomes localmente (ex.: `server.local` → `192.168.1.10`).

## HTTP
- Hospeda uma página web padrão (acessível via `http://192.168.1.10`).

## FTP
- Permite transferência de arquivos.
- Credenciais padrão do Packet Tracer (usuário/senha definidos na configuração do servidor).

## Testes sugeridos
1. **DNS** – De qualquer PC: `nslookup server.local 192.168.1.10`
2. **HTTP** – Abrir navegador e digitar `http://192.168.1.10`
3. **FTP** – Usar cliente FTP (ex.: linha de comando `ftp 192.168.1.10`)

**Nota:** A imagem da simulação mostra que todos os dispositivos têm o DNS apontado para `192.168.1.10`, portanto a resolução de nomes funcionará automaticamente.
