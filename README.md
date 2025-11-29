<div align="center">
  <img height="150" src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" />
</div>

###

<div align="center">
  <a href="https://www.linkedin.com/in/SEU-LINKEDIN" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="linkedin logo"/>
  </a>
  <a href="https://www.youtube.com/SEU-YOUTUBE" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Youtube&logo=youtube&label=&color=FF0000&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="youtube logo"/>
  </a>
  <a href="https://twitter.com/SEU-TWITTER" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Twitter&logo=twitter&label=&color=1DA1F2&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="twitter logo"/>
  </a>
</div>

###

<h1 align="center">🔐 Simulação de Malwares - Projeto Educacional</h1>

> ⚠️ **AVISO IMPORTANTE**: Este repositório é exclusivamente educacional. Execute apenas em ambientes controlados e isolados. O uso malicioso é crime.

---

<h3 align="left">👨‍💻 Sobre o Projeto</h3>

<p align="left">
Este projeto foi desenvolvido durante o bootcamp de Cybersegurança da DIO com o objetivo de entender, de maneira prática, como funcionam malwares e como podemos nos defender deles.<br><br>
Dois tipos de malware foram simulados:<br>
✔ Ransomware — criptografa arquivos e exige “resgate”<br>
✔ Keylogger — captura teclas digitadas no teclado<br><br>
Todos os testes foram feitos em ambiente seguro e isolado.
</p>

---

<h3 align="left">🎯 Objetivos de Aprendizado</h3>

- Entender criptografia simétrica
- Captura de eventos do sistema operacional
- Boas práticas de defesa e prevenção
- Consciência de segurança ofensiva e defensiva
- Python aplicado em cenários reais

---

<h3 align="left">🛠 Tecnologias Utilizadas</h3>

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="python logo"/>
  <img width="12"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-plain-wordmark.svg" height="40" alt="docker logo"/>
  <img width="12"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="40" alt="linux logo"/>
</div>

---

<h3 align="left">📁 Estrutura do Projeto</h3>

malware-simulado/
│
├── ransomware/
│ ├── ransomware.py
│ ├── decryptor.py
│ └── test_files/
│
├── keylogger/
│ ├── keylogger.py
│ ├── keylogger_email.py
│ └── log.txt
│
└── README.md

yaml
Copiar código

---

### 🦠 Ransomware Simulado

Como Funciona:

1. Gera uma chave criptográfica
2. Percorre arquivos da pasta alvo
3. Criptografa tudo usando Fernet (AES)
4. Cria um aviso de resgate

Instalação:

```bash
pip install cryptography
Execução:

bash
Copiar código
python ransomware.py
python decryptor.py  # para restaurar os arquivos
⌨️ Keylogger Simulado
Como Funciona:

Captura teclas digitadas

Salva em log.txt

Versão avançada envia por email

Instalação:

bash
Copiar código
pip install pynput
Execução:

bash
Copiar código
python keylogger.py
python keylogger_email.py
<h3 align="left">🛡 Segurança & Boas Práticas</h3>
Mantenha backups offline

Não clique em anexos suspeitos

Utilize 2FA

Gerenciadores de senha

Monitoramento de processos e antivírus

<h3 align="left">💡 Reflexões e Próximos Passos</h3>
Ética é fundamental em Cybersegurança

Ransomware é simples, porém devastador

Estudar: Forense Digital, Redes, Engenharia Reversa

<h3 align="left">⚖️ Responsabilidade Legal</h3>
Uso indevido configura crime segundo:

Lei 12.737/2012 (Carolina Dieckmann)

Art. 154-A do Código Penal

Execute apenas com permissão e em ambiente controlado.

<h3 align="left">📚 Referências</h3>
DIO - Bootcamp Cybersegurança

OWASP Top 10

NIST Cybersecurity Framework

Documentação oficial das bibliotecas

<h3 align="left">🔥 Minhas Estatísticas</h3> <div align="center"> <img src="https://github-readme-streak-stats.herokuapp.com/?user=SEU-USUARIO&hide_border=false" /> </div>
<h3 align="left">🤝 Contribuições</h3>
Contribuições, issues e sugestões são bem-vindas!

<h3 align="left">👨‍💻 Autor</h3>
Suas informações:

LinkedIn: https://www.linkedin.com/in/SEU-LINKEDIN

GitHub: https://github.com/SEU-USUARIO

Email: SEU-EMAIL

<div align="center">
"A segurança da informação não é um produto, é um processo." — Bruce Schneier
✨ Use seus conhecimentos para proteger, não atacar.

</div> ```
