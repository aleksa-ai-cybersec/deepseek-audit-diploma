---

```markdown
<div align="center">

# 🛡️ DeepSeek Security Auditor

## Интеллектуальная система аудита безопасности больших языковых моделей

<img src="https://img.shields.io/badge/Дипломная%20работа-2026-8A2BE2?style=for-the-badge" />
<img src="https://img.shields.io/badge/МГЛУ-Институт%20информационных%20наук-blue?style=for-the-badge" />

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![ML](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-orange?style=flat-square)](https://scikit-learn.org)
[![NLP](https://img.shields.io/badge/Deep%20NLP-Transformers-FF6F00?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co)
[![Dashboard](https://img.shields.io/badge/Live%20Dashboard-Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white)](https://plotly.com)
[![Interface](https://img.shields.io/badge/Interface-Gradio-8A2BE2?style=flat-square&logo=gradio&logoColor=white)](https://gradio.app)

</div>


**Дипломная работа Воробьевой Александры Александровны**  
Московский государственный лингвистический университет, Институт информационных наук, Кафедра международной информационной безопасности, 2026.

## 📝 О проекте

Интеллектуальная система для автоматизированного тестирования безопасности больших языковых моделей (LLM). Реализован в рамках дипломной работы по теме "Разработка методики аудита информационной безопасности систем, использующих технологии искусственного интеллекта".

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
- **Детектор галлюцинаций** — выявление фактических ошибок и противоречий
- **Анализ временных рядов** — тренды, аномалии, прогнозирование

### 🎯 Адаптивное тестирование
- Адаптивный выбор следующих угроз на основе энтропии Шеннона
- Байесовское оценивание с учётом априорной вероятности
- Автоматическая остановка тестирования при стабильных результатах
- Библиотека успешных атак с анализом паттернов

### 🛡️ Преодоление ограничений API
- **Пул из 6 токенов** (900 запросов/день)
- **Автоматическое переключение** при блокировках
- **Ротация User-Agent** (14 вариантов)
- **"Кофе-паузы"** и имитация человеческого поведения

### 📊 Аналитика и отчетность
- **Доверительные интервалы** (метод Вильсона, 95%)
- **Байесовские оценки** уязвимостей
- **7 интерактивных графиков** для визуализации
- **Telegram-уведомления** о критических находках
- **Live Dashboard** — визуализация в реальном времени
- Автоматическая генерация таблицы 3.2 с динамической оценкой рисков

## 🎮 Попробовать онлайн

  [![Streamlit App](https://img.shields.io/badge/🚀_Демо-Запустить_приложение-FF4B4B?style=for-the-badge&logo=streamlit)](https://deepseek-audit-diploma-n26kk2ohkcmofvox6hbdas.streamlit.app)
  [![GitHub](https://img.shields.io/badge/📁_Код-Репозиторий-181717?style=for-the-badge&logo=github)](https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma)
  [![Website](https://img.shields.io/badge/🌐_Сайт-Визитка-4285F4?style=for-the-badge&logo=google-chrome)](https://aleksa-ai-cybersec.github.io/deepseek-audit-diploma/)
  [![Garden](https://img.shields.io/badge/🌸_Сад_уязвимостей-Интерактивная_визуализация-FF69B4?style=for-the-badge&logo=star&logoColor=white)](https://aleksa-ai-cybersec.github.io/vulnerability-garden/)
  [![Quest](https://img.shields.io/badge/🎯_AI_Security_Simulator-Игровой_квест-9d4edd?style=for-the-badge&logo=playstation&logoColor=white)](https://aleksa-ai-cybersec.github.io/ai-security-quest/)

## 🚀 Быстрый старт

### Предварительные требования
- Python 3.10+
- 6 GitHub Personal Access Tokens (Classic) с правами `repo` и `read:packages`

### Установка и запуск

```bash
# Клонируйте репозиторий
git clone https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma.git
cd deepseek-audit-diploma

# Создайте виртуальное окружение
python3 -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate  # Windows

# Установите зависимости
pip install pandas numpy plotly scipy tqdm gradio requests langdetect

# Создайте файл с токенами
nano tokens.txt
# (вставьте 6 токенов, каждый с новой строки)

# Запустите аудит
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
├── deepseek_auditor.py      # Основной файл
├── tokens.txt               # Токены (не в репозитории!)
├── requirements.txt         # Зависимости
├── README.md                # Этот файл
├── .gitignore               # Игнорируемые файлы
├── cache/                    # Кэш ответов
├── results/                  # Результаты
│   ├── reports/              # Отчеты
│   ├── graphs/               # Графики
│   └── tables/               # JSON/CSV
└── logs/                     # Логи
```

📄 Лицензия

Дипломная работа. Московский государственный лингвистический университет, 2026.

---

<div align="center">🛡️ DeepSeek Security Auditor

Intelligent Security Auditing System for Large Language Models

<img src="https://img.shields.io/badge/Diploma%20Work-2026-8A2BE2?style=for-the-badge" />
<img src="https://img.shields.io/badge/MSLU-Institute%20of%20Information%20Sciences-blue?style=for-the-badge" />https://img.shields.io/badge/Python-3.10%2B-3776AB?style=flat-square&logo=python&logoColor=white
https://img.shields.io/badge/Machine%20Learning-Random%20Forest-orange?style=flat-square
https://img.shields.io/badge/Deep%20NLP-Transformers-FF6F00?style=flat-square&logo=huggingface&logoColor=white
https://img.shields.io/badge/Live%20Dashboard-Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white
https://img.shields.io/badge/Interface-Gradio-8A2BE2?style=flat-square&logo=gradio&logoColor=white

</div>Diploma work of VOROBEVA ALEKSANDRA
Moscow State Linguistic University, Institute of Information Sciences, Department of International Information Security, 2026.

📝 About the project

An intelligent system for automated security testing of Large Language Models (LLMs). Implemented as part of the diploma thesis "Development of an information security audit methodology for systems using artificial intelligence technologies".

✨ Key features

🔍 Audit Methodology

· 27 attack vectors covering the full ML system lifecycle
· Prioritization of critical vulnerabilities (priority 1)
· 80+ test prompts for comprehensive testing
· STRIDE-AI classification for structured analysis

🧠 Intelligent Analysis

· Semantic analysis of responses (refusal, information disclosure, evasiveness)
· Sentiment analysis (from -1 to 1)
· Multilingual support (Russian, English, Chinese, French, German)
· ML prediction of vulnerabilities before sending requests
· Hallucination detector — identifying factual errors and contradictions
· Time series analysis — trends, anomalies, forecasting

🎯 Adaptive Testing

· Adaptive selection of next threats based on Shannon entropy
· Bayesian estimation with prior probability
· Automatic testing stop when results stabilize
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

https://img.shields.io/badge/🚀_Demo-Launch_App-FF4B4B?style=for-the-badge&logo=streamlit
https://img.shields.io/badge/📁_Code-Repository-181717?style=for-the-badge&logo=github
https://img.shields.io/badge/🌐_Website-Landing_Page-4285F4?style=for-the-badge&logo=google-chrome
https://img.shields.io/badge/🌸_Vulnerability_Garden-Interactive_Visualization-FF69B4?style=for-the-badge&logo=star&logoColor=white
https://img.shields.io/badge/🎯_AI_Security_Simulator-Game_Quest-9d4edd?style=for-the-badge&logo=playstation&logoColor=white

🚀 Quick start

Prerequisites

· Python 3.10+
· 6 GitHub Personal Access Tokens (Classic) with repo and read:packages permissions

Installation and launch

```bash
# Clone the repository
git clone https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma.git
cd deepseek-audit-diploma

# Create a virtual environment
python3 -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate  # Windows

# Install dependencies
pip install pandas numpy plotly scipy tqdm gradio requests langdetect

# Create tokens file
nano tokens.txt
# (paste 6 tokens, one per line)

# Run the audit
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
├── deepseek_auditor.py      # Main file
├── tokens.txt               # Tokens (not in repository!)
├── requirements.txt         # Dependencies
├── README.md                # This file
├── .gitignore               # Ignored files
├── cache/                   # Response cache
├── results/                 # Results
│   ├── reports/             # Reports
│   ├── graphs/              # Graphs
│   └── tables/              # JSON/CSV
└── logs/                    # Logs
```

📄 License

Diploma work. Moscow State Linguistic University, 2026.

---

<div align="center">🛡️ DeepSeek 安全审计器

大语言模型智能安全审计系统

<img src="https://img.shields.io/badge/毕业论文-2026-8A2BE2?style=for-the-badge" />
<img src="https://img.shields.io/badge/莫斯科国立语言大学-信息科学研究所-blue?style=for-the-badge" />https://img.shields.io/badge/Python-3.10%2B-3776AB?style=flat-square&logo=python&logoColor=white
https://img.shields.io/badge/机器学习-随机森林-orange?style=flat-square
https://img.shields.io/badge/深度NLP-Transformers-FF6F00?style=flat-square&logo=huggingface&logoColor=white
https://img.shields.io/badge/实时仪表盘-Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white
https://img.shields.io/badge/界面-Gradio-8A2BE2?style=flat-square&logo=gradio&logoColor=white

</div>毕业论文作者：VOROBEVA ALEKSANDRA
莫斯科国立语言大学，信息科学研究所，国际信息安全系，2026年。

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
· 幻觉检测器 — 识别事实错误和矛盾
· 时间序列分析 — 趋势、异常、预测

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

https://img.shields.io/badge/🚀_演示-启动应用-FF4B4B?style=for-the-badge&logo=streamlit
https://img.shields.io/badge/📁_代码-仓库-181717?style=for-the-badge&logo=github
https://img.shields.io/badge/🌐_网站-名片页-4285F4?style=for-the-badge&logo=google-chrome
https://img.shields.io/badge/🌸_漏洞花园-交互式可视化-FF69B4?style=for-the-badge&logo=star&logoColor=white
https://img.shields.io/badge/🎯_AI安全模拟器-游戏任务-9d4edd?style=for-the-badge&logo=playstation&logoColor=white

🚀 快速开始

前置要求

· Python 3.10+
· 6个GitHub个人访问令牌（经典版），具有repo和read:packages权限

安装与运行

```bash
# 克隆仓库
git clone https://github.com/aleksa-ai-cybersec/deepseek-audit-diploma.git
cd deepseek-audit-diploma

# 创建虚拟环境
python3 -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate  # Windows

# 安装依赖
pip install pandas numpy plotly scipy tqdm gradio requests langdetect

# 创建令牌文件
nano tokens.txt
# （粘贴6个令牌，每行一个）

# 运行审计
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
├── deepseek_auditor.py      # 主文件
├── tokens.txt               # 令牌（不在仓库中！）
├── requirements.txt         # 依赖
├── README.md                # 本文件
├── .gitignore               # 忽略的文件
├── cache/                   # 响应缓存
├── results/                 # 结果
│   ├── reports/             # 报告
│   ├── graphs/              # 图表
│   └── tables/              # JSON/CSV
└── logs/                    # 日志
```

📄 许可证

毕业论文。莫斯科国立语言大学，2026年。

```

---