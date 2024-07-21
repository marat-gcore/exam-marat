# How to run automation tests

### Clone the repository

### The image "exam_srv" should be created

### Build image "marat-exam"
```python
docker build -t marat-exam .
```

### Build image "allure"
```python
docker build -t allure ./allure
```

### Run tests
```python
docker compose up
```

### Open allure report in browser
```python
http://localhost:8080
```