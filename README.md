# Delivery Cost API (Python - FastAPI)

This API calculates delivery costs based on product orders coming from different inventory centers.

## Try on:
  https://twf-flours-api-assignment.onrender.com/docs

## Features

- Accepts product orders in JSON format
- Computes the cheapest delivery cost using distance-based routing

##  Example

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

##  Requirements

- Python 3.8+
- FastAPI
- Uvicorn

##  Run Locally

```bash
pip install fastapi uvicorn
uvicorn main:app --reload
```

##  Try on POSTMAN

1. Send POST request on https://twf-flours-api-assignment.onrender.com/calculateCost
2. Send body in json format as { "A":1, "B":1, "C":1, "G":1, "H":1, "I":1 }
 
3. Result should be
   ```
   { "cost": 118 }
   ```

---
