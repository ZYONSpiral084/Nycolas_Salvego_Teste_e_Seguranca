# 🤖 Robocode CI/CD Pipeline  

## 📌 Project Overview / Visão Geral do Projeto  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| Robocode is a programming game where the goal is to develop a robot battle tank that competes against others in an arena.<br>It offers a fun and educational way to practice **Java programming** and **AI concepts**.<br><br>This project sets up a **Continuous Integration (CI) pipeline** for a Robocode robot using **GitHub Actions**.<br>The pipeline automatically builds and tests the robot code on every commit, ensuring issues are caught early.<br><br>**Continuous Integration (CI)** is the practice of automating code integration, compiling, and testing to ensure correctness and quality. | Robocode é um jogo de programação onde o objetivo é desenvolver um tanque de batalha robótico para competir em arena contra outros tanques.<br>É uma forma divertida e educativa de praticar **Java** e **Inteligência Artificial**.<br><br>Este projeto configura um **pipeline de Integração Contínua (CI)** para um robô Robocode usando **GitHub Actions**.<br>A cada commit, o código é compilado e testado automaticamente, garantindo mais qualidade e detecção rápida de erros.<br><br>**Integração Contínua (CI)** é a prática de automatizar integração de código, compilação e testes para garantir correção e qualidade. |

---

## 🏗️ CI/CD Pipeline Architecture / Arquitetura do Pipeline CI/CD  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| The pipeline runs in multiple sequential stages:<br><br>1. **Checkout & Java** → Clone repository and set up JDK 11.<br>2. **Compile** → Build the robot code (`javac` or Maven/Gradle).<br>3. **Checkstyle** → Validate code style with Google’s style rules.<br>4. **SpotBugs** → Run static analysis to catch bugs.<br>5. **Success** → Final status report if all stages pass. | O pipeline segue estas etapas sequenciais:<br><br>1. **Checkout & Java** → Clonar o repositório e configurar o JDK 11.<br>2. **Compilação** → Compilar o código do robô.<br>3. **Checkstyle** → Verificar estilo do código (padrão Google).<br>4. **SpotBugs** → Rodar análise estática para detectar erros.<br>5. **Sucesso** → Finalizar com relatório. |

---

## 💻 Setup / Instalação  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| 1. Install Java 11 (JDK).<br>2. Download Robocode → [robocode.sourceforge.io](https://robocode.sourceforge.io)<br>3. Place your robot classes in the `robots/` folder inside Robocode, or compile with `javac`. | 1. Instale o Java 11 (JDK).<br>2. Baixe e instale o Robocode → [robocode.sourceforge.io](https://robocode.sourceforge.io)<br>3. Coloque suas classes compiladas na pasta `robots/` dentro do Robocode, ou compile com `javac`. |

---

## 🙌 Credits / Créditos  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| This project was assigned by Prof. José Guilherme.<br>Special thanks for his guidance on implementing CI/CD practices in this project. | Projeto proposto pelo Prof. José Guilherme.<br>Agradecimento especial pela orientação na implementação do CI/CD. |

---

## ⚠️ Important Notes / Observações Importantes  

| 🇺🇸 English | 🇧🇷 Português |
|-------------|--------------|
| - **Checkstyle** → Uses `google_checks.xml` (requires Checkstyle 8.x or newer).<br>- **Java Version** → Robocode requires Java 8+, this project uses Java 11.<br>- **SpotBugs** → Runs on compiled classes (compile before running). | - **Checkstyle** → Utiliza `google_checks.xml` (versões antigas podem falhar).<br>- **Java** → Robocode requer Java 8+, aqui foi usado Java 11.<br>- **SpotBugs** → Requer classes compiladas previamente. |
