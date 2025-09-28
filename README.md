
📺 Vídeos do YouTube

CrashCourse Computer Science

The Cyber Mentor

Tech With Tim

NetworkChuck


🌐 Sites para estudo

OWASP

TryHackMe

Hack The Box

Cryptography.io

OverTheWire


📚 Cursos Online Gratuitos

Cybrary

FreeCodeCamp

Coursera: Cryptography I



---

💻 Exercícios e Projetos

🐍 Python — Criptografia AES

from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
from cryptography.hazmat.backends import default_backend
import os

key = os.urandom(32)
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

🔍 Meios Legais de “Quebra” de Criptografia (Estudo Ético)

📌 Conceitos

Criptoanálise, engenharia reversa, pentesting autorizado, ataques de força bruta em laboratório.


🛠 Ferramentas

John the Ripper, Hashcat, Ghidra, Frida, Wireshark, CyberChef.


📚 Recursos

Livro: Serious Cryptography.

Curso: Cryptography I — Coursera.

Labs: TryHackMe, Hack The Box.


⚡ Exercícios Éticos

Python — Ataque de Força Bruta Simples (Lab)

import hashlib

hash_obj = hashlib.sha256("senha123".encode()).hexdigest()
print("Hash gerado:", hash_obj)

wordlist = ["senha", "123456", "senha123"]

for word in wordlist:
    test_hash = hashlib.sha256(word.encode()).hexdigest()
    if test_hash == hash_obj:
        print("Senha encontrada:", word)

JavaScript — Decodificação Simples (Lab)

const crypto = require('crypto');

const texto = "mensagem secreta";
const hash = crypto.createHash('sha256').update(texto).digest('hex');
console.log("Hash SHA-256:", hash);


---

📆 Plano Semanal de Estudo

1. Fundamentos de programação e criptografia


2. Análise estática de apps


3. Análise dinâmica e interceptação de tráfego


4. Projetos de segurança


5. Revisão e desafio final


6. Participação em labs como TryHackMe e Hack The Box


7. Documentação e relatórios técnicos


8. Projeto final e portfólio




---

🛠 Ferramentas recomendadas

Python (cryptography, PyCryptodome)

Node.js + Express

Burp Suite Community

Frida, JADX, apktool

Ghidra, Wireshark



---

📂 Recursos Extras

E-books: "Serious Cryptography", "Cryptography Engineering"

Comunidades: Reddit r/netsec, Stack Overflow, GitHub Discussions

Podcasts: Darknet Diaries, Risky Business
