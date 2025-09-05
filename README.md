# 🤖 Robocode CI/CD Pipeline  

## 📌 Project Overview (English)  
Robocode is a programming game where the goal is to develop a robot battle tank that competes against others in an arena.  
It offers a fun and educational way to practice **Java programming** and **AI concepts**.  

This project sets up a **Continuous Integration (CI) pipeline** for a Robocode robot using **GitHub Actions**.  
The pipeline automatically builds and tests the robot code on every commit, ensuring issues are caught early.  

**Continuous Integration (CI)** is the practice of automating code integration, compiling, and testing to ensure correctness and quality.  

---

## 🏗️ CI/CD Pipeline Architecture  
The pipeline runs in multiple sequential stages:  

1. **Checkout & Java** → Clone repository and set up JDK 11.  
2. **Compile** → Build the robot code (`javac` or Maven/Gradle).  
3. **Checkstyle** → Validate code style with Google’s style rules.  
4. **SpotBugs** → Run static analysis to catch bugs.  
5. **Success** → Final status report if all stages pass.  

---

## 💻 Setup / Running Locally

1. Install Java 11 (JDK).
2. Download Robocode → robocode.sourceforge.io
3. Place your robot classes in the robots/ folder inside Robocode, or compile with javac.

---

🙌 Credits

This project was assigned by Prof. José Guilherme.
Special thanks for his guidance on implementing CI/CD practices in this project.

---

⚠️ Important Notes

Checkstyle → Uses google_checks.xml (requires Checkstyle 8.x or newer).
Java Version → Robocode requires Java 8+, this project uses Java 11.
SpotBugs → Runs on compiled classes (compile before running).

---

## 🇧🇷 Pipeline de CI/CD do Robocode
## 📌 Visão Geral do Projeto

Robocode é um jogo de programação onde o objetivo é desenvolver um tanque de batalha robótico para competir em arena contra outros tanques.
É uma forma divertida e educativa de praticar Java e Inteligência Artificial.
Este projeto configura um pipeline de Integração Contínua (CI) para um robô Robocode usando GitHub Actions.
A cada commit, o código é compilado e testado automaticamente, garantindo mais qualidade e detecção rápida de erros.

🏗️ Arquitetura do Pipeline CI/CD
O pipeline segue estas etapas sequenciais:

1. **Checkout & Java** → Clonar o repositório e configurar o JDK 11.
2. **Compilação** → Compilar o código do robô.
3. **Checkstyle** → Verificar estilo do código (padrão Google).
4. **SpotBugs** → Rodar análise estática para detectar erros.
5. **Sucesso** → Finalizar com relatório.

---

## 💻 Instalação / Execução Local

1. Instale o Java 11 (JDK).
2. Baixe e instale o Robocode → robocode.sourceforge.io
3. Coloque suas classes compiladas na pasta robots/.

---

## 🙌 Créditos

Projeto proposto pelo Prof. José Guilherme.
Agradecimento especial pela orientação na implementação do CI/CD.

---

## ⚠️ Observações Importantes

Checkstyle → Utiliza google_checks.xml (versões antigas podem falhar).
Java → Robocode requer Java 8+, aqui foi usado Java 11.
SpotBugs → Requer classes compiladas previamente.
