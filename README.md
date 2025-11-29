# 🔐 Simulação de Malwares - Projeto Educacional

Projeto desenvolvido durante o bootcamp de Cybersegurança da DIO para entender na prática como funcionam malwares e como se proteger deles.

> ⚠️ **AVISO IMPORTANTE**: Este repositório é exclusivamente educacional. Execute apenas em ambientes controlados e isolados. O uso malicioso é crime.

---

## 📌 Sobre o Projeto

Durante o curso, aprendi que a melhor forma de se defender de ameaças é entendendo como elas funcionam. Este projeto simula dois tipos comuns de malware:

- **Ransomware**: Criptografa arquivos e exige "resgate"
- **Keylogger**: Captura tudo que é digitado no teclado

Todos os códigos foram testados em ambiente seguro, sem causar danos reais.

---

## 🎯 Objetivos de Aprendizado

- Compreender criptografia aplicada a ataques
- Entender captura de eventos do sistema
- Aprender sobre prevenção e defesa
- Desenvolver consciência sobre segurança digital
- Praticar Python em cenários reais

---

## 🛠️ Tecnologias Utilizadas

- Python 3.x
- Biblioteca `cryptography` (para criptografia)
- Biblioteca `pynput` (para captura de teclado)
- Biblioteca `smtplib` (para envio de emails)

---

## 📁 Estrutura do Projeto

```
malware-simulado/
│
├── ransomware/
│   ├── ransomware.py
│   ├── decryptor.py
│   └── test_files/
│
├── keylogger/
│   ├── keylogger.py
│   ├── keylogger_email.py
│   └── log.txt
│
└── README.md
```

---

## 🦠 Ransomware Simulado

### Como Funciona

O ransomware percorre uma pasta, criptografa todos os arquivos encontrados e deixa uma mensagem de "resgate". Ele usa criptografia Fernet (AES) para tornar os arquivos ilegíveis.

**Fluxo de execução:**
1. Gera uma chave criptográfica única
2. Busca todos os arquivos na pasta alvo
3. Criptografa cada arquivo com a chave
4. Cria um arquivo de texto com instruções de "resgate"

### Instalação

```bash
pip install cryptography
```

### Como Usar

```bash
# Preparar ambiente de teste
mkdir test_files
cd test_files
echo "arquivo teste" > documento.txt

# Executar ransomware (APENAS EM test_files!)
python ransomware.py

# Para descriptografar
python decryptor.py
```

### O Que Aprendi

- Como funciona criptografia simétrica na prática
- A importância de manter backups offline
- Por que ransomware é tão efetivo (criptografia forte)
- Como implementar varredura recursiva de diretórios

---

## ⌨️ Keylogger Simulado

### Como Funciona

O keylogger captura todas as teclas digitadas e salva em um arquivo de texto. Versão avançada envia automaticamente por email.

**Recursos implementados:**
- Captura de teclas normais (letras, números)
- Tratamento de teclas especiais (Enter, Space, Tab)
- Ignora teclas de modificação (Shift, Ctrl, Alt)
- Salvamento contínuo em arquivo
- Envio automático por email (versão avançada)

### Instalação

```bash
pip install pynput
```

### Como Usar

```bash
# Versão básica (salva em arquivo local)
python keylogger.py

# Versão com email
python keylogger_email.py
```

### O Que Aprendi

- Como funcionam listeners de eventos do sistema
- Manipulação de arquivos em tempo real
- Automação de envio de emails com Python
- Por que senhas visíveis são perigosas
- Importância de usar gerenciadores de senha

---

## 🛡️ Defesas e Prevenção

Durante este estudo, identifiquei as principais formas de proteção:

### Contra Ransomware

**✅ Backups Regulares**
- Faça backup em dispositivos externos
- Mantenha uma cópia offline (disco desconectado)
- Teste a restauração periodicamente

**✅ Antivírus Atualizado**
- Windows Defender já oferece boa proteção
- Mantenha definições sempre atualizadas

**✅ Cuidado com Emails**
- Não abra anexos de remetentes desconhecidos
- Desconfie de urgências e ameaças
- Verifique extensões de arquivos (.exe, .js, .bat são suspeitos)

**✅ Atualizações do Sistema**
- Mantenha Windows e programas atualizados
- Patches corrigem vulnerabilidades exploradas

### Contra Keyloggers

**✅ Antivírus com Proteção de Teclado**
- Muitos antivírus detectam keyloggers
- Use proteção de digitação bancária

**✅ Gerenciadores de Senha**
- Evitam digitar senhas manualmente
- Preenchem automaticamente (sem captura)
- Exemplos: Bitwarden, LastPass, 1Password

**✅ Autenticação em Dois Fatores (2FA)**
- Mesmo com senha capturada, atacante não acessa
- Use apps como Google Authenticator ou Authy

**✅ Teclado Virtual**
- Para transações sensíveis, use teclado na tela
- Keyloggers baseados em software não capturam

**✅ Monitoramento do Sistema**
- Verifique processos em execução (Ctrl+Shift+Esc)
- Desconfie de programas desconhecidos

---

## 💡 Reflexões Pessoais

### O Que Este Projeto Me Ensinou

**1. Segurança não é paranoia, é necessidade**

Antes desse curso, eu subestimava o quão vulnerável um sistema pode ser. Agora entendo que qualquer descuido pode abrir portas para ataques sérios.

**2. Conhecimento é a melhor defesa**

Ao entender como ataques funcionam, consigo identificar padrões suspeitos no dia a dia. Agora penso duas vezes antes de clicar em qualquer link ou baixar arquivos.

**3. A simplicidade dos ataques é assustadora**

Não precisa ser um gênio da computação para criar malware. Com poucas linhas de código, dá pra causar estragos enormes. Isso me fez valorizar ainda mais profissionais de segurança.

**4. Prevenção é mais barata que recuperação**

Investir tempo em backups e boas práticas é infinitamente mais fácil do que tentar recuperar dados perdidos ou pagar resgates (que nem sempre funcionam).

**5. Ética é fundamental**

Com esse conhecimento vem uma responsabilidade enorme. Sei como atacar, mas escolho usar isso para proteger e educar outras pessoas.

### Próximos Passos

- Estudar análise de malware reversa
- Aprender sobre forense digital
- Me aprofundar em redes e firewall
- Contribuir com projetos open source de segurança

---

## ⚖️ Responsabilidade Legal

**Este projeto é educacional.** Uso indevido pode configurar crime:

- **Art. 154-A do Código Penal**: Invasão de dispositivo informático
- **Lei 12.737/2012** (Lei Carolina Dieckmann): Crimes informáticos
- **Marco Civil da Internet**: Violação de privacidade

Pena: até 5 anos de reclusão + multa

**Teste apenas em:**
- Seus próprios dispositivos
- Máquinas virtuais isoladas
- Ambientes controlados com permissão

---

## 📚 Referências e Materiais

- [DIO - Bootcamp Cybersegurança]([https://www.dio.me/](https://web.dio.me/track/santander-ciberseguranca-2025))
- [Documentação Cryptography](https://cryptography.io/)
- [Documentação pynput](https://pynput.readthedocs.io/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)

---

## 🤝 Contribuições

Este é um projeto educacional em constante evolução. Sugestões de melhorias são bem-vindas!

Se você também está estudando cybersegurança, fique à vontade para:
- Fazer fork do projeto
- Sugerir melhorias
- Compartilhar suas experiências
- Reportar bugs (caso encontre)

---

## 👨‍💻 Autor

Desenvolvido com 🧠 durante minha jornada de aprendizado em Cybersegurança.

**Conecte-se comigo:**
- LinkedIn: https://br.linkedin.com/in/michel-pascoal
- GitHub: https://github.com/michelbru

---

## 📝 Licença

Este projeto está sob a licença MIT - veja o arquivo LICENSE para detalhes.

---

## 🙏 Agradecimentos

- **DIO** por proporcionar o bootcamp
- Instrutores e mentores do curso
- Comunidade de cybersegurança brasileira
- Todos que contribuem com conhecimento open source

---

**"A segurança da informação não é um produto, é um processo."** - Bruce Schneier

*Lembre-se: use seus conhecimentos para o bem. A internet já tem hackers demais, precisamos de mais defensores.*
