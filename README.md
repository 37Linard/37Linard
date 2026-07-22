# Gabriel Linard

Brasília, Brasil • Ciência da Computação (UniCEUB, formatura em 2027)

Gosto de entender sistemas de dentro para fora. Tenho experiência construindo software de base do zero — de kernel bare-metal e banco relacional a agentes de IA locais — além de estudar segurança ofensiva desenvolvendo minhas próprias ferramentas.

## Destaque: SO em Rust, do boot ao TCP/IP

**[SO---RUST](https://github.com/37Linard/SO---RUST)** — kernel x86_64 bare-metal escrito do zero, sem dependência de sistema operacional host.

- Boot real com `bootloader`, GDT/TSS/IDT, paginação e alocador de heap próprios.
- Multitarefa preemptiva com context switch real, syscalls via `int 0x80` e suporte a ring 3.
- Sistema de arquivos persistente sobre driver ATA PIO próprio, com sobrevivência a reboot.
- Compositor gráfico multi-janela com mouse PS/2, fonte bitmap desenhada à mão e shell rodando dentro da GUI.
- Driver de rede RTL8139 implementado do zero com ARP, ICMP, UDP e handshake TCP validado contra `TcpClient` do .NET.

Todo o projeto foi depurado com ferramentas reais — QEMU monitor, serial log e disassembly — até funcionar ponta a ponta.

## Outros projetos

| Projeto | O que é |
|---|---|
| [IA Ômega](https://github.com/37Linard/IA---Omega) | Agente de IA autônomo 100% local com Ollama, FastAPI e Next.js, sem dependência de API paga. |
| [MiniDB](https://github.com/37Linard/MiniDB) | Banco de dados relacional em C++20 com storage engine, buffer pool LRU, B+Tree e WAL. |
| [VulnLab](https://github.com/37Linard/vulnlab) | Aplicação Flask propositalmente vulnerável, cobrindo 8 falhas do OWASP Top 10 com exploits e testes documentados. |
| [Phishing Detector](https://github.com/37Linard/phishing-detector) | Extensão Chrome para detecção de phishing em tempo real com heurísticas locais. |
| [Obsidian Study Organizer](https://github.com/37Linard/obsidian-study-organizer) | Plugin de repetição espaçada com SM-2 para revisar problemas de LeetCode no Obsidian. |

## Agora

- Construindo uma distribuição Linux própria com Buildroot, kernel real, BusyBox e interface X11/Fluxbox.
- Desenvolvendo o **ClinScribe**, um ambient scribe clínico para transformar consultas em prontuários SOAP estruturados para médicos brasileiros.

---

[Email](mailto:gabrielinard37@gmail.com) · [GitHub](https://github.com/37Linard)
