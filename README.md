# Resource Manager 🚀
> A headless, borderless, click-through hardware telemetry HUD designed to sit seamlessly over fullscreen games and applications.

Resource Manager is a lightweight, high-performance desktop utility written in Python that tracks critical system resources (CPU, GPU, RAM, and the highest contributing process) in a minimalist overlay. Utilizing low-level Windows API hooks, it features absolute mouse pass-through, global hotkey visibility toggles, and cross-session configuration persistence.

---

## ✨ Key Features

* **Headless Gaming HUD:** Completely strips away traditional OS title bars, close/minimize buttons, and window frames for a true minimalist aesthetic.
* **Win32 Input Pass-Through:** Leverages native `User32.dll` extended window styles (`WS_EX_TRANSPARENT`) to ensure mouse clicks pass directly through the HUD, preventing crosshair interruption during competitive gameplay.
* **Asynchronous Multi-Threading:** Isolates telemetry-scraping routines from the main UI thread, eliminating micro-stutters and frame-drops.
* **Taskbar & DWM Isolation:** Configured as a native Windows tool window (`WS_EX_TOOLWINDOW`), preventing it from populating space on the taskbar or window switcher menus.
* **Global Keyboard Hooks:** Instantly toggle panel visibility (`Alt + T`) or invoke the single-instance modal settings window (`Alt + Y`) from anywhere within the operating system.
* **State Persistence:** Automatically flushes position mapping coordinates and opacity parameters to a local `config.json` matrix file across app reboots.

---

## 🛠️ Architecture & Tech Stack

* **Core Language:** Python 3
* **GUI Engine:** Tkinter 
* **Low-Level OS Interface:** `ctypes` Wrapper (Invoking native Windows User32 Core Binary)
* **Telemetry Aggregators:** `psutil` (System Core Architecture), `nvidia-smi` CLI Parser (GPU Metrics Engine)
* **System Event Listeners:** `keyboard`, `pystray` (System Tray Routine Engine)
* **Packaging Compiler:** PyInstaller

---

## 🚀 Installation & Compilation

### Prerequisites
Ensure you have the required dependencies updated within your environment:
```bash
pip install --upgrade psutil pillow keyboard pystray

```
# Resource Manager 🚀
> A headless, borderless, click-through hardware telemetry HUD designed to sit seamlessly over fullscreen games and applications.

Resource Manager is a lightweight, high-performance desktop utility written in Python that tracks critical system resources (CPU, GPU, RAM, and the highest contributing process) in a minimalist overlay. Utilizing low-level Windows API hooks, it features absolute mouse pass-through, global hotkey visibility toggles, and cross-session configuration persistence.

---

## ✨ Key Features

* **Headless Gaming HUD:** Completely strips away traditional OS title bars, close/minimize buttons, and window frames for a true minimalist aesthetic.
* **Win32 Input Pass-Through:** Leverages native `User32.dll` extended window styles (`WS_EX_TRANSPARENT`) to ensure mouse clicks pass directly through the HUD, preventing crosshair interruption during competitive gameplay.
* **Asynchronous Multi-Threading:** Isolates telemetry-scraping routines from the main UI thread, eliminating micro-stutters and frame-drops.
* **Taskbar & DWM Isolation:** Configured as a native Windows tool window (`WS_EX_TOOLWINDOW`), preventing it from populating space on the taskbar or window switcher menus.
* **Global Keyboard Hooks:** Instantly toggle panel visibility (`Alt + T`) or invoke the single-instance modal settings window (`Alt + Y`) from anywhere within the operating system.
* **State Persistence:** Automatically flushes position mapping coordinates and opacity parameters to a local `config.json` matrix file across app reboots.

---

## 🛠️ Architecture & Tech Stack

* **Core Language:** Python 3
* **GUI Engine:** Tkinter 
* **Low-Level OS Interface:** `ctypes` Wrapper (Invoking native Windows User32 Core Binary)
* **Telemetry Aggregators:** `psutil` (System Core Architecture), `nvidia-smi` CLI Parser (GPU Metrics Engine)
* **System Event Listeners:** `keyboard`, `pystray` (System Tray Routine Engine)
* **Packaging Compiler:** PyInstaller

---

## 🚀 Installation & Compilation

### Prerequisites
Ensure you have the required dependencies updated within your environment:
```bash
pip install --upgrade psutil pillow keyboard pystray
