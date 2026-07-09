# ZenLab Perceptron — Backend

Backend API untuk prediksi kelulusan mahasiswa. Dibangun dengan FastAPI.

## Tech Stack

- **FastAPI** — framework API
- **Python 3.12+**
- **Scikit-learn** — model klasifikasi
- **Pandas / NumPy** — pemrosesan data

## Setup

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

## Menjalankan

```bash
uvicorn app:app --reload
```

API docs: `http://localhost:8000/docs`

## API Endpoints

| Method | Path | Deskripsi |
|--------|------|-----------|
| POST | `/api/predict` | Prediksi kelulusan |
| GET | `/api/metrics` | Metrik model |
| GET | `/api/dataset` | Data dataset |

## Struktur

```
├── app.py           # Entry point FastAPI
├── model/           # Model ML
├── dataset/         # Data latih
└── requirements.txt
```
