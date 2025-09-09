# 🤖 Robocode CI/CD Pipeline

**Languages:** [English](README.md) • [Português (pt-BR)](README.pt-BR.md) • [中文（简体）](README.zh-CN.md)

---

## 📌 Project Overview / Visão Geral do Projeto / 项目概述

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| Robocode is a programming game where the goal is to develop a robot battle tank that competes against others in an arena. It offers a fun and educational way to practice **Java programming** and **AI concepts**.<br><br>This project sets up a **Continuous Integration (CI) pipeline** for a Robocode robot using **GitHub Actions**. The pipeline automatically builds and tests the robot code on every commit, ensuring issues are caught early.<br><br>**Continuous Integration (CI)** is the practice of automating code integration, compiling, and testing to ensure correctness and quality. | Robocode é um jogo de programação onde o objetivo é desenvolver um tanque de batalha robótico para competir em arena contra outros tanques. É uma forma divertida e educativa de praticar **Java** e conceitos de **IA**.<br><br>Este projeto configura um **pipeline de Integração Contínua (CI)** para um robô Robocode usando **GitHub Actions**. O pipeline compila e testa o código do robô automaticamente a cada commit, garantindo a detecção precoce de problemas.<br><br>**Integração Contínua (CI)** é a prática de automatizar integração de código, compilação e testes para garantir correção e qualidade. | Robocode 是一款编程游戏，目标是开发一个在竞技场内与其他机器人坦克对战的机器人。它为练习 **Java 编程** 和 **人工智能概念** 提供了有趣且教育性的方式。本项目使用 **GitHub Actions** 为 Robocode 机器人搭建 **持续集成 (CI) 管线**。该管线会在每次提交时自动构建并测试机器人代码，从而尽早发现问题。**持续集成 (CI)** 指的是自动化代码集成、编译与测试以确保正确性与质量的实践。 |

---

## 🏗️ CI/CD Pipeline Architecture / Arquitetura do Pipeline CI/CD / CI/CD 管线架构

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| The pipeline runs in multiple sequential stages:<br><br>1. **Checkout & Java** → Clone repository and set up JDK 11.<br>2. **Compile** → Build the robot code (`javac` or Maven/Gradle).<br>3. **Checkstyle** → Validate code style with Google’s style rules.<br>4. **SpotBugs** → Run static analysis to catch bugs.<br>5. **Success** → Final status report if all stages pass. | O pipeline segue estas etapas sequenciais:<br><br>1. **Checkout & Java** → Clonar o repositório e configurar o JDK 11.<br>2. **Compilação** → Compilar o código do robô (`javac` ou Maven/Gradle).<br>3. **Checkstyle** → Verificar estilo do código com as regras do Google.<br>4. **SpotBugs** → Rodar análise estática para detectar bugs.<br>5. **Sucesso** → Relatório final se todas as etapas passarem. | 管线按多个顺序阶段运行：<br><br>1. **检出 & Java** → 克隆仓库并设置 JDK 11。<br>2. **编译** → 构建机器人代码（使用 `javac` 或 Maven/Gradle）。<br>3. **Checkstyle** → 使用 Google 的编码风格规则验证代码风格。<br>4. **SpotBugs** → 运行静态分析以发现潜在缺陷。<br>5. **成功** → 所有阶段通过后给出最终状态报告。 |

---

## 💻 Setup / Instalação / 安装

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| 1. Install Java 11 (JDK).<br>2. Download Robocode → https://robocode.sourceforge.io<br>3. Place your robot classes in the `robots/` folder inside Robocode, or compile with `javac`. | 1. Instale o Java 11 (JDK).<br>2. Baixe e instale o Robocode → https://robocode.sourceforge.io<br>3. Coloque suas classes de robô na pasta `robots/` dentro do Robocode, ou compile-as com `javac`. | 1. 安装 Java 11（JDK）。<br>2. 下载 Robocode → https://robocode.sourceforge.io<br>3. 将你的机器人类放入 Robocode 的 `robots/` 文件夹，或使用 `javac` 进行编译。 |

---

## 🙌 Credits / Créditos / 致谢

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| This project was assigned by Prof. José Guilherme.<br>Special thanks for his guidance on implementing CI/CD practices in this project. | Projeto proposto pelo Prof. José Guilherme.<br>Agradecimento especial pela orientação na implementação do CI/CD. | 本项目由 José Guilherme 教授布置。特别感谢他在本项目 CI/CD 实施上的指导。 |

---

## ⚠️ Important Notes / Observações Importantes / 重要说明

| 🇺🇸 English | 🇧🇷 Português | 🇨🇳 中文（简体） |
|---|---|---|
| - **Checkstyle** → Uses `google_checks.xml` (requires Checkstyle 8.x or newer).<br>- **Java Version** → Robocode requires Java 8+, this project uses Java 11.<br>- **SpotBugs** → Runs on compiled classes (compile before running). | - **Checkstyle** → Utiliza `google_checks.xml` (requer Checkstyle 8.x ou superior).<br>- **Versão Java** → Robocode requer Java 8+, neste projeto usamos Java 11.<br>- **SpotBugs** → Executa sobre classes compiladas (compile antes de rodar). | - **Checkstyle** → 使用 `google_checks.xml`（需要 Checkstyle 8.x 或更高版本）。<br>- **Java 版本** → Robocode 要求 Java 8 及以上，本项目使用 Java 11。<br>- **SpotBugs** → 在已编译的类上运行（请先进行编译）。 |

---

## How to use these files / Como usar estes arquivos / 如何使用这些文件

Each file in the repository root corresponds to a language variant of this documentation. Keep the English `README.md` as the primary source. When you update core instructions, remember to update translations or mark them as needing review.
