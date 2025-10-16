# 🚀 로봇 관제 시스템 (InfluxDB + Grafana + Dummy Data)

이 프로젝트는 모바일 로봇(UGV)과 로봇팔 데이터를 시뮬레이션하고, InfluxDB와 Grafana를 통해 실시간 관제 대시보드를 제공합니다.

## 실행 방법

### 1. 프로젝트 압축 풀기
```bash
unzip robot_monitoring_project.zip
cd robot_monitoring_project
```

### 2. Docker Compose 실행
```bash
docker-compose up -d
```

### 3. 서비스 접속
- InfluxDB: http://localhost:8086 (admin / admin123)
- Grafana: http://localhost:3000 (admin / admin123)

👉 Grafana에는 InfluxDB 데이터소스와 로봇 관제 대시보드가 자동으로 세팅됩니다.

### 4. (옵션) 더미 데이터 실행
```bash
pip install influxdb-client
python dummy_robot_data.py
```
