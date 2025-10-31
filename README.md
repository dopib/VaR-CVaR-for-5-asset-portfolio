# VaR & CVaR для 5-активного портфеля — проект

**Кратко:** репозиторий с шагами для расчёта VaR (Historical, Parametric), CVaR (ES), EVT (POT/GPD), rolling-backtest и базовыми визуализациями. Код рассчитан на запуск в Google Colab.

---

## Содержание репозитория

* `notebooks/` — Jupyter/Colab notebooks (шаги 1–7).
* `data/` — входные CSV: `prices.csv`, `returns.csv`, `portfolio_returns.csv`.
* `results/` — артефакты: `var_es_comparison.csv`, `evt_var_es_results.json`, `report.pdf`, `figures/`.
* `src/` — вспомогательные скрипты (опционально): `feature_generation.py`, `pricer.py`, `backtest.py`.
* `requirements.txt` — зависимости.
* `README.md` — этот файл.
* `.gitignore` — предложенный шаблон.

---

## Быстрый старт (Google Colab)

1. Открой Google Colab.
2. Клонируй репозиторий (или загрузите ноутбуки прямо в Colab):

```
!git clone https://github.com/<your-username>/<repo-name>.git
%cd <repo-name>
```

3. Открой `notebooks/01_data_load.ipynb` и запусти ячейки по порядку. Последовательно выполнены шаги 1–7 проекта.

4. В `results/` появятся `report.pdf` и графики в `results/figures/`.

---

## Как воспроизвести локально (Linux / macOS / WSL / Colab terminal)

1. Создать виртуальное окружение:

```
python -m venv venv
source venv/bin/activate
```

2. Установить зависимости:

```
pip install -r requirements.txt
```

3. Запустить ноутбук через Jupyter или выполнить скрипты:

```
jupyter notebook
# или
python src/run_all.py
```

---

## Требуемые зависимости (`requirements.txt`)

```
yfinance
pandas
numpy
scipy
matplotlib
seaborn
fpdf
```

---




