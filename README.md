<div align="center">

<img src="./assets/banner.svg" alt="CYBERDARK CTF Writeups" width="100%"/>

<br/><br/>

```
 ██████╗██╗   ██╗██████╗ ███████╗██████╗ ██████╗  █████╗ ██████╗ ██╗  ██╗
██╔════╝╚██╗ ██╔╝██╔══██╗██╔════╝██╔══██╗██╔══██╗██╔══██╗██╔══██╗██║ ██╔╝
██║      ╚████╔╝ ██████╔╝█████╗  ██████╔╝██║  ██║███████║██████╔╝█████╔╝ 
██║       ╚██╔╝  ██╔══██╗██╔══╝  ██╔══██╗██║  ██║██╔══██║██╔══██╗██╔═██╗ 
╚██████╗   ██║   ██████╔╝███████╗██║  ██║██████╔╝██║  ██║██║  ██║██║  ██╗
 ╚═════╝   ╚═╝   ╚═════╝ ╚══════╝╚═╝  ╚═╝╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝
                    C T F   W R I T E U P S   C O L L E C T I O N
```

<img src="https://img.shields.io/badge/STATUS-ONLINE-00ff41?style=for-the-badge&labelColor=0a0e0a&logo=statuspage&logoColor=00ff41"/>
<img src="https://img.shields.io/badge/WRITEUPS-14-00ffff?style=for-the-badge&labelColor=0a0e0a&logo=hackthebox&logoColor=00ffff"/>
<img src="https://img.shields.io/badge/PLATFORMS-3-bf00ff?style=for-the-badge&labelColor=0a0e0a&logo=linux&logoColor=bf00ff"/>
<img src="https://img.shields.io/badge/FORMAT-PDF-ff5f57?style=for-the-badge&labelColor=0a0e0a&logo=adobeacrobatreader&logoColor=ff5f57"/>
<img src="https://img.shields.io/badge/LANG-ESPAÑOL-ffcc00?style=for-the-badge&labelColor=0a0e0a&logo=googletranslate&logoColor=ffcc00"/>

</div>

---

## `root@cyberdark:~$` **whoami**

```bash
> Operador:     Cyberdark Security
> Misión:       Documentar resolución de máquinas CTF
> Enfoque:      Enumeración · Explotación · Escalada de privilegios
> Estado:       ● SISTEMA ACTIVO
```

> [!IMPORTANT]
> Repositorio personal de **writeups** en formato PDF. Cada documento detalla el camino completo desde el reconocimiento inicial hasta la obtención de flags.

---

## `root@cyberdark:~$` **ls -la /**

```
/
├── 📁 MiraSoyRoot/     →  6 máquinas
├── 📁 Dockerlabs/      →  4 máquinas
├── 📁 CyberConquer/    →  4 máquinas
├── 📄 README.md
├── 📄 REPORT.md
└── 📁 assets/
```

---

## `root@cyberdark:~$` **cat writeups.db**

<details open>
<summary><b>🟢 MiraSoyRoot</b> — <code>6 targets compromised</code></summary>
<br/>

| `#` | `TARGET` | `STATUS` | `ACCESS` |
|:---:|:---|:---:|:---:|
| `01` | **Anonymous** | `PWNED` | [📄 Abrir PDF](./MiraSoyRoot/Machine%20-%20Anonymous%20-MiraSoyRoot.pdf) |
| `02` | **Arcode** | `PWNED` | [📄 Abrir PDF](./MiraSoyRoot/Machine%20-%20Arcode%20-MiraSoyRoot.pdf) |
| `03` | **Fuzzer** | `PWNED` | [📄 Abrir PDF](./MiraSoyRoot/Machine%20-%20Fuzzer%20-MiraSoyRoot.pdf) |
| `04` | **Mirasoyroot** | `PWNED` | [📄 Abrir PDF](./MiraSoyRoot/Machine%20-%20Mirasoyroot%20-MiraSoyRoot.pdf) |
| `05` | **Sabores Ocultos** | `PWNED` | [📄 Abrir PDF](./MiraSoyRoot/Machine%20-%20Sabores%20Ocultos%20-MiraSoyRoot.pdf) |
| `06` | **Time Traversal** | `PWNED` | [📄 Abrir PDF](./MiraSoyRoot/Machine%20-%20Time%20Traversal%20-MiraSoyRoot.pdf) |

</details>

<details open>
<summary><b>🔵 Dockerlabs</b> — <code>4 targets compromised</code></summary>
<br/>

| `#` | `TARGET` | `STATUS` | `ACCESS` |
|:---:|:---|:---:|:---:|
| `01` | **Domain** | `PWNED` | [📄 Abrir PDF](./Dockerlabs/Machine%20-%20Domain%20-Dockerlabs.pdf) |
| `02` | **Injection** | `PWNED` | [📄 Abrir PDF](./Dockerlabs/Machine%20-%20injection%20-Dockerlabs.pdf) |
| `03` | **Trust** | `PWNED` | [📄 Abrir PDF](./Dockerlabs/Machine%20-%20Trust%20-Dockerlabs.pdf) |
| `04` | **Upload** | `PWNED` | [📄 Abrir PDF](./Dockerlabs/Machine%20-%20Upload%20-Dockerlabs.pdf) |

</details>

<details open>
<summary><b>🟣 CyberConquer</b> — <code>4 targets compromised</code></summary>
<br/>

| `#` | `TARGET` | `STATUS` | `ACCESS` |
|:---:|:---|:---:|:---:|
| `01` | **Ecorp** | `PWNED` | [📄 Abrir PDF](./CyberConquer/Machine%20-%20Ecorp%20-CyberConquer.pdf) |
| `02` | **Enigma Codificado** | `PWNED` | [📄 Abrir PDF](./CyberConquer/Machine%20-%20Enigma%20Codificado%20-CyberConquer.pdf) |
| `03` | **Relámpago** | `PWNED` | [📄 Abrir PDF](./CyberConquer/Machine%20-%20Relampago%20-CyberConquer.pdf) |
| `04` | **Vías Ocultas** | `PWNED` | [📄 Abrir PDF](./CyberConquer/Machine%20-%20Vias%20Ocultas%20-CyberConquer.pdf) |

</details>

---

## `root@cyberdark:~$` **nmap --stats**

```diff
+ MiraSoyRoot .............. [████████████░░] 6/14  (42.9%)
+ Dockerlabs ............... [████████░░░░░░] 4/14  (28.6%)
+ CyberConquer ............. [████████░░░░░░] 4/14  (28.6%)
+ Total comprometidas ...... [██████████████] 14/14 (100%)
```

---

## `root@cyberdark:~$` **cat /etc/motd**

```
╔══════════════════════════════════════════════════════════════╗
║                                                              ║
║   "El conocimiento es la única herramienta que crece         ║
║    cuando se comparte."                                      ║
║                                                              ║
║              > Happy Hacking! <                              ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝
```

---

## `root@cyberdark:~$` **todo list --pending**

- [x] Organizar estructura de carpetas por plataforma
- [ ] Migrar writeups de PDF a Markdown
- [ ] Añadir sección de herramientas utilizadas
- [ ] Implementar verificación SHA-256 (`hashes.txt`)

> [!TIP]
> Consulta el [Informe de Auditoría](./REPORT.md) para análisis de seguridad y recomendaciones de mejora del repositorio.

---

<div align="center">

```console
root@cyberdark:~# echo "ACCESS GRANTED" && exit 0
ACCESS GRANTED
```

<sub>🛡️ <b>CYBERDARK SECURITY</b> — CTF Writeups Collection</sub>

</div>
