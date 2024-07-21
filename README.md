## How to run automation tests

### The image "exam_srv" should be already created

### 1. Clone the repository

### 2. Build image "marat-exam"
```python
docker build -t marat-exam .
```

### 3. Build image "allure"
```python
docker build -t allure ./allure
```

### 4. Run web server container
```python
docker compose up -d webserver
```

### 5. Run tests container
```python
docker compose up automation-tests
```

### 6. Run allure container
```python
docker compose up -d allure-report
```

### 7. Open allure report in browser
```python
http://localhost:8080
```

### 8. Clean containers
```python
docker compose down
```