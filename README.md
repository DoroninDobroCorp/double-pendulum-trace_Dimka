🇬🇧 [English](#-english) | 🇷🇺 [Русский](#-русский)

---

# 🇬🇧 English

# 🎯 Double Pendulum Trace

A high-performance, interactive double pendulum simulation that visualizes chaotic motion in real time. Built with React 19, TypeScript, and Vite; originally prototyped in [Google AI Studio](https://ai.studio/apps/drive/1Tk11TWfxa6wfZ8eXDiTltdFCR5V6uvKt).

## ✨ Features

The interface is split into **five synchronized panels**:

| Panel | Description |
|---|---|
| **Real Space** | Animates the double pendulum and traces the path of its tip |
| **Angle Phase Space** | Plots the trajectory in (θ₁, θ₂) space — click to set a new starting point |
| **Velocity Phase Space** | Plots the trajectory in (ω₁, ω₂) space — click to set a new starting point |
| **Angle Fractal** | Colors the (θ₁, θ₂) plane by chaos intensity — dark = stable, bright = chaotic. Supports zoom |
| **Velocity Fractal** | Colors the (ω₁, ω₂) plane by chaos intensity — dark = stable, bright = chaotic. Supports zoom |

### Controls

- **Click** on any phase-space or fractal panel to launch a simulation from that point
- <kbd>M</kbd> — double simulation speed
- <kbd>N</kbd> — halve simulation speed
- **Reset** button — randomize initial angles
- **Zero Velocity** button — reset angular velocities to 0
- **Tutorial (?)** — side-panel guide explaining every visualization

### Physics

- Equations of motion solved with a **4th-order Runge–Kutta** (RK4) integrator
- 40 integration steps per animation frame (scales with speed multiplier without losing precision)

## 🚀 Getting Started

**Prerequisites:** Node.js ≥ 18

```bash
# 1. Install dependencies
npm install

# 2. (Optional) Set your Gemini API key if using AI Studio features
#    Create a .env.local file with:
#    GEMINI_API_KEY=your_key_here

# 3. Start the dev server
npm run dev
```

Open the URL shown in the terminal (usually `http://localhost:5173`).

### Production Build

```bash
npm run build
npm run preview
```

## 🛠 Tech Stack

- **React 19** + **TypeScript**
- **Vite 6** — dev server & bundler
- **Canvas API** — all rendering is done on `<canvas>` elements for maximum performance

## 💡 Tips

> Use the angle fractal panel and click on a **dark region away from the center** — observe the pattern. Most orbits will eventually diverge; try to find one that doesn't!

---

# 🇷🇺 Русский

# 🎯 Трассировка Двойного Маятника

Высокопроизводительная интерактивная симуляция двойного маятника с визуализацией хаотического движения в реальном времени. Создано на React 19, TypeScript и Vite; прототип разработан в [Google AI Studio](https://ai.studio/apps/drive/1Tk11TWfxa6wfZ8eXDiTltdFCR5V6uvKt).

## ✨ Возможности

Интерфейс разделён на **пять синхронизированных панелей**:

| Панель | Описание |
|---|---|
| **Реальное пространство** | Анимация двойного маятника и трассировка траектории его конца |
| **Фазовое пространство углов** | Траектория в пространстве (θ₁, θ₂) — кликните, чтобы задать новую начальную точку |
| **Фазовое пространство скоростей** | Траектория в пространстве (ω₁, ω₂) — кликните, чтобы задать новую начальную точку |
| **Фрактал углов** | Окрашивает плоскость (θ₁, θ₂) по степени хаотичности — тёмное = стабильно, яркое = хаотично. Поддержка зума |
| **Фрактал скоростей** | Окрашивает плоскость (ω₁, ω₂) по степени хаотичности — тёмное = стабильно, яркое = хаотично. Поддержка зума |

### Управление

- **Клик** по любой фазовой или фрактальной панели запускает симуляцию из выбранной точки
- <kbd>M</kbd> — удвоить скорость симуляции
- <kbd>N</kbd> — уменьшить скорость вдвое
- **Reset** — случайные начальные углы
- **Zero Velocity** — обнулить угловые скорости
- **Tutorial (?)** — боковая панель с описанием каждой визуализации

### Физика

- Уравнения движения решаются методом **Рунге–Кутты 4-го порядка** (RK4)
- 40 шагов интегрирования за кадр анимации (масштабируется с множителем скорости без потери точности)

## 🚀 Быстрый старт

**Требования:** Node.js ≥ 18

```bash
# 1. Установить зависимости
npm install

# 2. (Опционально) Указать ключ Gemini API для функций AI Studio
#    Создайте файл .env.local:
#    GEMINI_API_KEY=ваш_ключ

# 3. Запустить dev-сервер
npm run dev
```

Откройте URL из терминала (обычно `http://localhost:5173`).

### Продакшен-сборка

```bash
npm run build
npm run preview
```

## 🛠 Стек технологий

- **React 19** + **TypeScript**
- **Vite 6** — dev-сервер и сборщик
- **Canvas API** — вся отрисовка выполняется на элементах `<canvas>` для максимальной производительности

## 💡 Совет

> Откройте фрактал углов и кликните по **тёмной области вдали от центра** — понаблюдайте за паттерном. Большинство орбит со временем расходятся — попробуйте найти ту, которая не расходится!
