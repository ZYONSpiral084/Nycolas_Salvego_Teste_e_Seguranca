# 🤖 Robocode CI/CD Pipeline

**Idiomas:** [English](README.md) • [Português (pt-BR)](README.pt-BR.md) • [中文（简体）](README.zh-CN.md)

---

## 📌 Visão Geral do Projeto

Robocode é um jogo de programação cujo objetivo é desenvolver um tanque de batalha robótico que compete em uma arena contra outros tanques. É uma forma divertida e educativa de praticar **Java** e conceitos de **IA**. Este projeto configura um **pipeline de Integração Contínua (CI)** para um robô Robocode usando **GitHub Actions**. O pipeline compila e testa o código do robô automaticamente a cada commit, garantindo a detecção precoce de problemas.

**Integração Contínua (CI)** é a prática de automatizar a integração de código, compilação e testes para garantir correção e qualidade.

---

## 🏗️ Arquitetura do Pipeline CI/CD

O pipeline segue estas etapas sequenciais:

1. **Checkout & Java** → Clonar o repositório e configurar o JDK 11.
2. **Compilação** → Compilar o código do robô (`javac` ou Maven/Gradle).
3. **Checkstyle** → Verificar estilo do código com as regras do Google.
4. **SpotBugs** → Rodar análise estática para detectar bugs.
5. **Sucesso** → Relatório final se todas as etapas passarem.

---

## 💻 Instalação

1. Instale o Java 11 (JDK).
2. Baixe o Robocode → https://robocode.sourceforge.io
3. Coloque suas classes de robô na pasta `robots/` dentro do Robocode, ou compile-as com `javac`.

---

## 🙌 Créditos

Projeto proposto pelo Prof. José Guilherme. Agradecimento especial pela orientação na implementação do CI/CD.

---

## ⚠️ Observações Importantes

- **Checkstyle** → Utiliza `google_checks.xml` (requer Checkstyle 8.x ou superior).
- **Versão Java** → Robocode requer Java 8+, neste projeto usamos Java 11.
- **SpotBugs** → Executa sobre classes compiladas (compile antes de rodar).
