```markdown
<div align="center">

# 🛡️ DeepSeek Security Auditor

## Интеллектуальная система аудита безопасности больших языковых моделей

**🎓 Дипломная работа 2026 | 🏛️ МГЛУ | 🔬 Институт информационных наук**

**🐍 Python 3.10+ | 🤖 Random Forest | 🧠 Transformers | 📊 Plotly | 🎨 Gradio**

</div>

**Дипломная работа Воробьевой Александры Александровны**  
Московский государственный лингвистический университет, Институт информационных наук, Кафедра международной информационной безопасности, 2026.

---

## 📝 О проекте

Интеллектуальная система для автоматизированного тестирования безопасности больших языковых моделей (LLM). Реализована в рамках дипломной работы по теме "Разработка методики аудита информационной безопасности систем, использующих технологии искусственного интеллекта".

## ✨ Ключевые возможности

### 🔍 Методология аудита
- **27 векторов атак**, охватывающих полный жизненный цикл ML-систем
- **Приоритизация** критических уязвимостей (priority 1)
- **80+ тестовых промптов** для всестороннего тестирования
- **Классификация по STRIDE-AI** для структурированного анализа

### 🧠 Интеллектуальный анализ
- **Семантический анализ** ответов (отказ, раскрытие информации, уклончивость)
- **Анализ тональности** (от -1 до 1)
- **Многоязычная поддержка** (русский, английский, китайский, французский, немецкий)
- **ML-предсказание** уязвимостей до отправки запроса
- **Детектор галлюцинаций**
- **Анализ временных рядов**

### 🎯 Адаптивное тестирование
- Адаптивный выбор угроз на основе энтропии Шеннона
- Байесовское оценивание
- Автоматическая остановка при стабильных результатах
- Библиотека успешных атак

### 🛡️ Преодоление ограничений API
- **Пул из 6 токенов** (900 запросов/день)
- **Автоматическое переключение** при блокировках
- **Ротация User-Agent** (14 вариантов)
- **"Кофе-паузы"**

### 📊 Аналитика и отчетность
- **Доверительные интервалы** (метод Вильсона, 95%)
- **Байесовские оценки**
- **7 интерактивных графиков**
- **Telegram-уведомления**
- **Live Dashboard**
- Автоматическая генерация таблицы 3.2

## 🎮 Попробовать онлайн

- 🚀 **Демо-приложение**: https://deepseek-audit-diploma-n26kk2ohkcmofvox6hbdas.streamlit.app
- 📁 **GitHub**: https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma
- 🌐 **Сайт-визитка**: https://aleksa-ai-cybersec.github.io/deepseek-audit-diploma/
- 🌸 **Сад уязвимостей**: https://aleksa-ai-cybersec.github.io/vulnerability-garden/
- 🎯 **AI Security Simulator**: https://aleksa-ai-cybersec.github.io/ai-security-quest/

## 🚀 Быстрый старт

### Предварительные требования
- Python 3.10+
- 6 GitHub Personal Access Tokens

### Установка и запуск

```bash
git clone https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma.git
cd deepseek-audit-diploma
python3 -m venv venv
source venv/bin/activate
pip install pandas numpy plotly scipy tqdm gradio requests langdetect
nano tokens.txt
python3 deepseek_auditor.py
```

Настройка Telegram

```bash
export TELEGRAM_BOT_TOKEN="ваш_токен"
export TELEGRAM_CHAT_ID="ваш_chat_id"
```

📁 Структура проекта

```
deepseek-audit-diploma/
├── deepseek_auditor.py
├── tokens.txt
├── requirements.txt
├── README.md
├── .gitignore
├── cache/
├── results/
│   ├── reports/
│   ├── graphs/
│   └── tables/
└── logs/
```

📄 Лицензия

Дипломная работа. Московский государственный лингвистический университет, 2026.

---

<div align="center">🛡️ DeepSeek Security Auditor

Intelligent Security Auditing System for Large Language Models

🎓 Diploma 2026 | 🏛️ MSLU | 🔬 Institute of Information Sciences

🐍 Python 3.10+ | 🤖 Random Forest | 🧠 Transformers | 📊 Plotly | 🎨 Gradio

</div>Diploma work of VOROBEVA ALEKSANDRA
Moscow State Linguistic University, Institute of Information Sciences, Department of International Information Security, 2026.

---

📝 About the project

An intelligent system for automated security testing of Large Language Models (LLMs). Implemented as part of the diploma thesis "Development of an information security audit methodology for systems using artificial intelligence technologies".

✨ Key features

🔍 Audit Methodology

· 27 attack vectors covering the full ML system lifecycle
· Prioritization of critical vulnerabilities (priority 1)
· 80+ test prompts for comprehensive testing
· STRIDE-AI classification for structured analysis

🧠 Intelligent Analysis

· Semantic analysis of responses (refusal, disclosure, evasiveness)
· Sentiment analysis (from -1 to 1)
· Multilingual support (Russian, English, Chinese, French, German)
· ML prediction of vulnerabilities before sending requests
· Hallucination detector
· Time series analysis

🎯 Adaptive Testing

· Adaptive threat selection based on Shannon entropy
· Bayesian estimation with prior probability
· Automatic stop when results stabilize
· Successful attacks library with pattern analysis

🛡️ Overcoming API Limitations

· Pool of 6 tokens (900 requests/day)
· Automatic switching during blocks
· User-Agent rotation (14 variants)
· "Coffee breaks" and human behavior simulation

📊 Analytics and Reporting

· Confidence intervals (Wilson method, 95%)
· Bayesian vulnerability estimates
· 7 interactive graphs for visualization
· Telegram notifications about critical findings
· Live Dashboard — real-time visualization
· Automatic generation of Table 3.2 with dynamic risk assessment

🎮 Try online

· 🚀 Demo App: https://deepseek-audit-diploma-n26kk2ohkcmofvox6hbdas.streamlit.app
· 📁 GitHub: https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma
· 🌐 Website: https://aleksa-ai-cybersec.github.io/deepseek-audit-diploma/
· 🌸 Vulnerability Garden: https://aleksa-ai-cybersec.github.io/vulnerability-garden/
· 🎯 AI Security Simulator: https://aleksa-ai-cybersec.github.io/ai-security-quest/

🚀 Quick start

Prerequisites

· Python 3.10+
· 6 GitHub Personal Access Tokens

Installation and launch

```bash
git clone https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma.git
cd deepseek-audit-diploma
python3 -m venv venv
source venv/bin/activate
pip install pandas numpy plotly scipy tqdm gradio requests langdetect
nano tokens.txt
python3 deepseek_auditor.py
```

Telegram setup

```bash
export TELEGRAM_BOT_TOKEN="your_token"
export TELEGRAM_CHAT_ID="your_chat_id"
```

📁 Project structure

```
deepseek-audit-diploma/
├── deepseek_auditor.py
├── tokens.txt
├── requirements.txt
├── README.md
├── .gitignore
├── cache/
├── results/
│   ├── reports/
│   ├── graphs/
│   └── tables/
└── logs/
```

📄 License

Diploma work. Moscow State Linguistic University, 2026.

---

<div align="center">🛡️ DeepSeek 安全审计器

大语言模型智能安全审计系统

🎓 毕业论文 2026 | 🏛️ 莫斯科国立语言大学 | 🔬 信息科学研究所

🐍 Python 3.10+ | 🤖 随机森林 | 🧠 Transformers | 📊 Plotly | 🎨 Gradio

</div>毕业论文作者：VOROBEVA ALEKSANDRA
莫斯科国立语言大学，信息科学研究所，国际信息安全系，2026年。

---

📝 关于项目

用于大语言模型自动化安全测试的智能系统。作为毕业论文《使用人工智能技术的系统信息安全审计方法开发》的一部分实现。

✨ 主要功能

🔍 审计方法

· 27个攻击向量，覆盖ML系统完整生命周期
· 优先级排序（优先级1）
· 80+测试提示词，全面测试
· STRIDE-AI分类，结构化分析

🧠 智能分析

· 语义分析（拒绝、信息泄露、回避）
· 情感分析（从-1到1）
· 多语言支持（俄语、英语、中文、法语、德语）
· ML预测（发送请求前预测漏洞）
· 幻觉检测器
· 时间序列分析

🎯 自适应测试

· 基于香农熵的自适应威胁选择
· 带先验概率的贝叶斯估计
· 结果稳定时自动停止测试
· 成功攻击库及模式分析

🛡️ 突破API限制

· 6个令牌池（900次请求/天）
· 自动切换（遇到限制时）
· User-Agent轮换（14种变体）
· "咖啡休息" 和人类行为模拟

📊 分析与报告

· 置信区间（威尔逊方法，95%）
· 贝叶斯漏洞估计
· 7个交互式图表用于可视化
· Telegram通知（关键发现时）
· 实时仪表盘 — 实时可视化
· 自动生成表3.2，动态风险评估

🎮 在线试用

· 🚀 演示应用: https://deepseek-audit-diploma-n26kk2ohkcmofvox6hbdas.streamlit.app
· 📁 GitHub: https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma
· 🌐 网站: https://aleksa-ai-cybersec.github.io/deepseek-audit-diploma/
· 🌸 漏洞花园: https://aleksa-ai-cybersec.github.io/vulnerability-garden/
· 🎯 AI安全模拟器: https://aleksa-ai-cybersec.github.io/ai-security-quest/

🚀 快速开始

前置要求

· Python 3.10+
· 6个GitHub个人访问令牌

安装与运行

```bash
git clone https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma.git
cd deepseek-audit-diploma
python3 -m venv venv
source venv/bin/activate
pip install pandas numpy plotly scipy tqdm gradio requests langdetect
nano tokens.txt
python3 deepseek_auditor.py
```

Telegram设置

```bash
export TELEGRAM_BOT_TOKEN="您的令牌"
export TELEGRAM_CHAT_ID="您的聊天ID"
```

📁 项目结构

```
deepseek-audit-diploma/
├── deepseek_auditor.py
├── tokens.txt
├── requirements.txt
├── README.md
├── .gitignore
├── cache/
├── results/
│   ├── reports/
│   ├── graphs/
│   └── tables/
└── logs/
```

📄 许可证

毕业论文。莫斯科国立语言大学，2026年。

```