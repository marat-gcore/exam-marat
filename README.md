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

### 4. Run tests
```python
docker compose up
```

### 5. Open allure report in browser
```python
http://localhost:8080
```