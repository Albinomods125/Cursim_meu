📘 Curso Completo Pessoal: Cibersegurança & Criptografia

Um guia completo para estudo, com vídeos, sites, exercícios, códigos, ferramentas e métodos éticos.


---

🎥 Vídeos do YouTube

CrashCourse Computer Science

The Cyber Mentor

Tech With Tim

NetworkChuck


🌐 Sites e Cursos

OWASP

TryHackMe

Hack The Box

Cryptography.io

OverTheWire

Coursera: Cryptography I



---

💻 Exercícios e Projetos

🐍 Python — Criptografia AES

> Descrição: Este código demonstra criptografia simétrica AES em CBC mode.



<details>
<summary style="background-color:#2c3e50;color:white;padding:5px;border-radius:5px;cursor:pointer;">Mostrar código Python AES</summary>from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
from cryptography.hazmat.backends import default_backend
import os

key = os.urandom(32)
iv = os.urandom(16)
cipher = Cipher(algorithms.AES(key), modes.CBC(iv), backend=default_backend())
enc = cipher.encryptor()
plaintext = b"Mensagem secreta 16b"
ciphertext = enc.update(plaintext) + enc.finalize()
print("Texto cifrado:", ciphertext)

</details>🐍 Python — Hash SHA-256

> Descrição: Gera um hash SHA-256 de um texto.



<details>
<summary style="background-color:#27ae60;color:white;padding:5px;border-radius:5px;cursor:pointer;">Mostrar código Hash SHA-256</summary>import hashlib

texto = "meu texto para hash".encode('utf-8')
hash_obj = hashlib.sha256(texto)
print("Hash SHA-256:", hash_obj.hexdigest())

</details>💻 JavaScript — Servidor Express

> Descrição: Cria um servidor web simples usando Express.js.



<details>
<summary style="background-color:#2980b9;color:white;padding:5px;border-radius:5px;cursor:pointer;">Mostrar código Servidor Express</summary>const express = require('express');
const app = express();

app.get('/', (req, res) => {
    res.send('Olá, mundo!');
});

app.listen(3000, () => console.log('Servidor rodando na porta 3000'));

</details>💻 JavaScript — Hash SHA-256

> Descrição: Gera um hash SHA-256 em Node.js.



<details>
<summary style="background-color:#8e44ad;color:white;padding:5px;border-radius:5px;cursor:pointer;">Mostrar código Hash SHA-256 JS</summary>const crypto = require('crypto');
const texto = "meu texto para hash";
const hash = crypto.createHash('sha256').update(texto).digest('hex');
console.log("Hash SHA-256:", hash);

</details>
---

🔍 Meios Legais de “Quebra” de Criptografia

Conceitos: criptoanálise, engenharia reversa, pentesting autorizado.

Ferramentas: John the Ripper, Hashcat, Ghidra, Frida, Wireshark, CyberChef.

Recursos: Serious Cryptography, Cryptography I — Coursera, TryHackMe, Hack The Box.

import os

# Gera chave e vetor de inicialização (IV)
key = os.urandom(32)
iv = os.urandom(16)

# Cria cifrador AES
cipher = Cipher(algorithms.AES(key), modes.CBC(iv), backend=default_backend())
enc = cipher.encryptor()

plaintext = b"Mensagem secreta 16b"
ciphertext = enc.update(plaintext) + enc.finalize()

print("Texto cifrado:", ciphertext)

🐍 Python — Hash SHA-256

Descrição: Gera um hash SHA-256 de um texto.

import hashlib

texto = "meu texto para hash".encode('utf-8')
hash_obj = hashlib.sha256(texto)
print("Hash SHA-256:", hash_obj.hexdigest())

💻 JavaScript — Servidor Express

Descrição: Cria um servidor web simples usando Express.js.

const express = require('express');
const app = express();

app.get('/', (req, res) => {
    res.send('Olá, mundo!');
});

app.listen(3000, () => console.log('Servidor rodando na porta 3000'));

💻 JavaScript — Hash SHA-256

Descrição: Gera um hash SHA-256 em Node.js.

const crypto = require('crypto');

const texto = "meu texto para hash";
const hash = crypto.createHash('sha256').update(texto).digest('hex');
console.log("Hash SHA-256:", hash);


---

🔍 Meios Legais de “Quebra” de Criptografia

Conceitos: Criptoanálise, engenharia reversa, pentesting autorizado.

Ferramentas: John the Ripper, Hashcat, Ghidra, Frida, Wireshark, CyberChef.

Recursos: Serious Cryptography, Cryptography I — Coursera, TryHackMe, Hack The Box.

⚡ Exercícios Éticos

Python — Força Bruta Simples

Descrição: Simula ataque de força bruta em laboratório.

import hashlib

hash_obj = hashlib.sha256("senha123".encode()).hexdigest()
print("Hash gerado:", hash_obj)

wordlist = ["senha", "123456", "senha123"]
for word in wordlist:
    test_hash = hashlib.sha256(word.encode()).hexdigest()
    if test_hash == hash_obj:
        print("Senha encontrada:", word)

JavaScript — Decodificação

Descrição: Demonstra criação de hash SHA-256 em JS.

const crypto = require('crypto');
const texto = "mensagem secreta";
const hash = crypto.createHash('sha256').update(texto).digest('hex');
console.log("Hash SHA-256:", hash);


---

📆 Plano Semanal

1. Fundamentos de programação e criptografia


2. Análise estática de apps


3. Análise dinâmica e interceptação de tráfego


4. Projetos de segurança


5. Revisão e desafio final


6. Labs práticos (TryHackMe, Hack The Box)


7. Documentação técnica


8. Projeto final e portfólio




---

🛠 Ferramentas Recomendadas

Python (cryptography, PyCryptodome), Node.js, Burp Suite, Frida, JADX, apktool, Ghidra, Wireshark.


---

📂 Recursos Extras

E-books: "Serious Cryptography", "Cryptography Engineering". Comunidades: Reddit r/netsec, Stack Overflow. Podcasts: Darknet Diaries, Risky Business.

iv = os.urandom(16)
cipher = Cipher(algorithms.AES(key), modes.CBC(iv), backend=default_backend())
enc = cipher.encryptor()
plaintext = b"Mensagem secreta 16b"
ciphertext = enc.update(plaintext) + enc.finalize()
print("Texto cifrado:", ciphertext)

🐍 Python — Hash SHA-256

import hashlib
texto = "meu texto para hash".encode('utf-8')
hash_obj = hashlib.sha256(texto)
print("Hash SHA-256:", hash_obj.hexdigest())

💻 JavaScript — Servidor Express

const express = require('express');
const app = express();
app.get('/', (req, res) => {
    res.send('Olá, mundo!');
});
app.listen(3000, () => console.log('Servidor rodando na porta 3000'));

💻 JavaScript — Hash SHA-256

const crypto = require('crypto');
const texto = "meu texto para hash";
const hash = crypto.createHash('sha256').update(texto).digest('hex');
console.log("Hash SHA-256:", hash);


---

🔍 Meios Legais de “Quebra” de Criptografia

Conceitos: criptoanálise, engenharia reversa, pentesting autorizado.

Ferramentas: John the Ripper, Hashcat, Ghidra, Frida, Wireshark, CyberChef.

Recursos: Serious Cryptography, Cryptography I — Coursera, TryHackMe, Hack The Box.

⚡ Exercícios Éticos

Python — Força Bruta Simples

import hashlib
hash_obj = hashlib.sha256("senha123".encode()).hexdigest()
print("Hash gerado:", hash_obj)
wordlist = ["senha", "123456", "senha123"]
for word in wordlist:
    test_hash = hashlib.sha256(word.encode()).hexdigest()
    if test_hash == hash_obj:
        print("Senha encontrada:", word)

JavaScript — Decodificação

const crypto = require('crypto');
const texto = "mensagem secreta";
const hash = crypto.createHash('sha256').update(texto).digest('hex');
console.log("Hash SHA-256:", hash);


---

📆 Plano Semanal

1. Fundamentos de programação e criptografia


2. Análise estática de apps


3. Análise dinâmica e interceptação de tráfego


4. Projetos de segurança


5. Revisão e desafio final


6. Labs práticos (TryHackMe, Hack The Box)


7. Documentação técnica


8. Projeto final e portfólio




---

🛠 Ferramentas Recomendadas

Python (cryptography, PyCryptodome), Node.js, Burp Suite, Frida, JADX, apktool, Ghidra, Wireshark.


---

📂 Recursos Extras

E-books: "Serious Cryptography", "Cryptography Engineering". Comunidades: Reddit r/netsec, Stack Overflow. Podcasts: Darknet Diaries, Risky Business.


---



