# 🤖 Robocode 持续集成/持续交付（CI/CD）管线

**语言：** [English](README.md) • [Português (pt-BR)](README.pt-BR.md) • [中文（简体）](README.zh-CN.md)

---

## 📌 项目概述

Robocode 是一个编程游戏，目标是开发一款在竞技场与其他机器人坦克对战的机器人。它为练习 **Java 编程** 与 **人工智能概念** 提供了有趣且富有教育意义的方式。本项目使用 **GitHub Actions** 为 Robocode 机器人建立 **持续集成（CI）管线**，该管线会在每次提交时自动构建并测试机器人代码，从而及早发现问题并提高代码质量。

---

## 🏗️ CI/CD 管线架构

管线按下列顺序阶段运行：

1. **检出 & Java** → 克隆仓库并配置 JDK 11。
2. **编译** → 构建机器人代码（`javac` 或 Maven/Gradle）。
3. **Checkstyle** → 使用 Google 编码规范验证代码风格。
4. **SpotBugs** → 运行静态分析以发现潜在缺陷。
5. **成功** → 若所有阶段通过则生成最终状态报告。

---

## 💻 安装

1. 安装 Java 11（JDK）。
2. 下载 Robocode → https://robocode.sourceforge.io
3. 将机器人类放入 Robocode 的 `robots/` 文件夹，或使用 `javac` 进行编译。

---

## 🙌 致谢

本项目由 José Guilherme 教授布置，特别感谢他在本项目 CI/CD 实施上的指导。

---

## ⚠️ 重要说明

- **Checkstyle** → 使用 `google_checks.xml`（需要 Checkstyle 8.x 或更高版本）。
- **Java 版本** → Robocode 要求 Java 8 及以上，本项目使用 Java 11。
- **SpotBugs** → 在已编译的类上运行（请先进行编译）。
