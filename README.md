#for project folder structure 
#run command : - tree /F

#Folder Structure
## 📁 Project Structure

```text
industrial-thermal-monitoring/
│
├── README.md
├── requirements.txt
├── .gitignore
├── .env.example
│
├── backend/
│   ├── app.py
│   ├── config.py
│   │
│   ├── routes/
│   │   ├── anomaly_routes.py
│   │   ├── map_routes.py
│   │   └── facility_routes.py
│   │
│   ├── services/
│   │   ├── thermal_service.py
│   │   ├── classification_service.py
│   │   ├── satellite_service.py
│   │   └── gis_service.py
│   │
│   └── utils/
│       ├── preprocessing.py
│       └── coordinates.py
│
├── frontend
│
├── ml/
│   ├── train.py
│   ├── predict.py
│   ├── preprocess.py
│   │
│   ├── models/
│   │   └── thermal_classifier.pkl
│   │
│   └── notebooks/
│       └── model_training.ipynb
│
├── data/
│   ├── raw/
│   │   ├── thermal_anomalies/
│   │   ├── satellite_images/
│   │   └── industrial_facilities/
│   │
│   ├── processed/
│   │   ├── thermal_features.csv
│   │   └── classified_anomalies.csv
│   │
│   └── sample/
│       └── sample_anomalies.csv
│
├── database/
│   ├── schema.sql
│   └── database.py
│
├── gis/
│   ├── layers/
│   │   ├── industrial_sites.geojson
│   │   ├── thermal_anomalies.geojson
│   │   └── land_cover.geojson
│   │
│   └── processing/
│       └── spatial_analysis.py
│
├── scripts/
│   ├── download_data.py
│   ├── preprocess_data.py
│   └── generate_map_data.py
│
├── tests/
│   ├── test_model.py
│   ├── test_api.py
│   └── test_gis.py
│
└── docs/
    ├── architecture.md
    ├── methodology.md
    └── dataset.md
```

### Directory Overview

| Directory/File      | Purpose                                             |
| ------------------- | --------------------------------------------------- |
| `backend/`          | Backend API and business logic                      |
| `backend/routes/`   | API endpoints                                       |
| `backend/services/` | Thermal, classification, satellite and GIS services |
| `backend/utils/`    | Utility and preprocessing functions                 |
| `frontend/`         | Web-based GIS dashboard                             |
| `ml/`               | Machine learning training and prediction            |
| `ml/models/`        | Trained ML models                                   |
| `ml/notebooks/`     | ML experimentation and analysis                     |
| `data/raw/`         | Raw FIRMS, satellite and industrial data            |
| `data/processed/`   | Processed features and classifications              |
| `data/sample/`      | Small sample datasets for development/testing       |
| `database/`         | Database schema and database utilities              |
| `gis/`              | GIS layers and spatial analysis                     |
| `scripts/`          | Data download and preprocessing scripts             |
| `tests/`            | Unit and API tests                                  |
| `docs/`             | Architecture, methodology and dataset documentation |
