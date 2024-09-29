# Python-101

This is everything that i try to do with Python

## Virtual environment
```python -m venv <virtual environment name>```: một trong những cách để tạo Python virtual environment (không phải mạnh nhất, nhưng dễ dùng)

**Active Venv**

| OS     | Command                                                 |
|--------|---------------------------------------------------------|
| MAC hoặc Linux| ```source <virtual environment name>/bin/activate```| 
| Window, Wsl hoặc Git Bash | ```source <virtual environment name>/Scripts/activate```| 
| Command Prompt | ```<virtual environment name>\Scripts\activate.bat```| 

**Deadactive Venv**  
```deactivate```

## Dependencies  
**Install**   
```pip install requirements.txt```: Tải toàn bộ Python packages được liệt kê trong file requirements.txt

**Create**  
```pip install pipreqs```: Pipreqs là công cụ giúp liệt kê những Python packages trong environment hiện tại vào file requirements.txt  
```pipreqs --pip-version pip --force --upgrade```: Liệt kê tất cả Python packages đang dùng trong environment hiện và đưa vào requirements.txt
- **--pip-version pip**: Chỉ định rằng các Python package cần phải tương thích với phiên bản hiện tại của pip
- **--force**: Ghi đè lên file requirements.txt hiện có 
- **--upgrade**: Đảm bảo sẽ liệt kê phiên bản mới nhất của môi Python package vào requirement.txt (có thể gây lỗi, cân nhắc không dùng)