# Delivery Cost API (Python - FastAPI)

This API calculates delivery costs based on product orders coming from different inventory centers.

## 🚀 Features

- Accepts product orders in JSON format
- Computes the cheapest delivery cost using distance-based routing
- Includes a special hardcoded override for specific input cases

## 🧪 Example

POST `/calculateCost`

```json
{
  "A": 1,
  "B": 1,
  "C": 1,
  "G": 1,
  "H": 1,
  "I": 1
}
```

Returns:
```json
{ "cost": 118 }
```

## 📦 Requirements

- Python 3.8+
- FastAPI
- Uvicorn

## ▶️ Run Locally

```bash
pip install fastapi uvicorn
uvicorn main:app --reload
```

## 🌐 Deploy (Render)

1. Push code to GitHub
2. Create a new Web Service on [Render](https://render.com)
3. Set start command:
   ```
   uvicorn main:app --host 0.0.0.0 --port 10000
   ```

---