# Gabriel Linard

Brasília, Brasil — Ciência da Computação (UniCEUB, formatura 2027).

Gosto de entender sistemas de dentro pra fora: já implementei um SO bare-metal do zero, um banco de dados relacional com WAL e B+Tree, e um agente de IA que roda 100% local. Também estudo segurança ofensiva construindo as próprias ferramentas em vez de só usar as prontas.

## Destaque: SO em Rust, do boot ao TCP/IP

**[SO---RUST](https://github.com/37Linard/SO---RUST)** — kernel x86_64 bare-metal escrito do zero, sem depender de nenhum SO existente.

- Boot real via `bootloader` + GDT/TSS/IDT, paginação e heap allocator próprios
- Multitarefa preemptiva com context switch real (não cooperativo) + syscalls via `int 0x80` e ring3 genuíno
- Filesystem persistente sobre driver ATA PIO próprio, sobrevive a reboot
- Compositor gráfico multi-janela (mouse PS/2, fonte bitmap desenhada à mão) com shell rodando dentro da GUI
- Driver de rede rtl8139 escrito do zero: ARP, ICMP, UDP e **handshake TCP real** validado contra `.NET TcpClient`

Nenhuma dessas partes veio de tutorial copiado — cada uma foi debugada com ferramentas reais (QEMU monitor, serial log, disassembly) até funcionar de ponta a ponta.

## Outros projetos

| Projeto | O que é |
|---|---|
| [IA Ômega](https://github.com/37Linard/IA---Omega) | Agente de IA autônomo rodando 100% local (Ollama + FastAPI + Next.js) — sem depender de API paga |
| [MiniDB](https://github.com/37Linard/MiniDB) | Banco de dados relacional em C++20: storage engine, buffer pool LRU, B+Tree indexada, WAL |
| [VulnLab](https://github.com/37Linard/vulnlab) | App Flask propositalmente vulnerável — 8 falhas do OWASP Top 10, cada uma com exploit e teste documentado |
| [Phishing Detector](https://github.com/37Linard/phishing-detector) | Extensão Chrome que detecta phishing em tempo real via heurísticas locais, sem chamar API externa |
| [Obsidian Study Organizer](https://github.com/37Linard/obsidian-study-organizer) | Plugin de repetição espaçada (SM-2) pra revisar problemas do LeetCode dentro do Obsidian |

## Agora

- Construindo uma distro Linux própria via Buildroot (kernel real + Busybox, GUI X11/fluxbox) — depois de terminar o SO em Rust
- Desenvolvendo o **ClinScribe**, um ambient scribe clínico (transcrição de consulta → prontuário SOAP estruturado) para médicos brasileiros — projeto privado, pré-beta

---

[Email](mailto:gabrielinard37@gmail.com) · [GitHub](https://github.com/37Linard)
