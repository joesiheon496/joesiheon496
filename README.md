# Jo Siheon

AI Vision & NLP Researcher

[![Gmail](https://img.shields.io/badge/Gmail-josehan1234%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:josehan1234@gmail.com)

---

## Career

### 한양대학교 석사과정 — 응용 물리학과 연구실
`2021.03.02 ~ 2023.02.15`

- BERT를 이용한 딥러닝 기반 **특허 자동 분류**
- Contrastive Learning을 이용한 **유사 특허 검색**

### 팀바이오
`2023.03.10 ~ 2024.10.31`

- **nn-UNet** 기반 병변 이미지 탐색 (Medical Image Segmentation)
- **VoxelMorph**를 이용한 암 병변 크기 비교 (Deformable Registration)

### 지에스아이 (GSI)
`2024.01.15 ~ 재직중`

- **항만 자동화** 연구 — 컨테이너 착지 감지, 자동 라벨링, Anti-Lift 등

### 한양대학교 박사과정 — 전자공학부 CELOS
`2026.02.11 ~ 재학중`

- **Sensor Fusion** (Camera + LiDAR) Representation 연구

---

## Projects

### SensorFusion (`src/sensorfusion/`)

Ouster OS1 LiDAR와 카메라 데이터를 융합하는 5단계 파이프라인 GUI 애플리케이션.

| Tab | 기능 | 핵심 알고리즘 |
|-----|------|--------------|
| 1. Frame Extraction | OSF에서 프레임 추출/저장 | ouster-sdk ScanSource |
| 2. Intrinsic Calib | 체커보드 기반 카메라 내부 파라미터 산출 | Zhang's method (`cv2.calibrateCamera`) |
| 3. Extrinsic Calib | 2D-3D 대응점으로 카메라-LiDAR 외부 파라미터 산출 | PnP (`cv2.solvePnP`) |
| 4. Projection | 이미지 → 3D 포인트 클라우드 변환 / LiDAR+RGB 시각화 | Back-projection, `scipy.griddata` |
| 5. Perception | YOLOv8-Seg 기반 객체 탐지 및 3D 매핑 | Ultralytics YOLOv8 |

> 자세한 내용: [`src/sensorfusion/README.md`](src/sensorfusion/README.md)

### Landed Test Program (`GSI/landed_test_program/`)

YOLOv8 모델을 이용한 컨테이너 착지(landed) 여부 판별 GUI 프로그램.

- 동영상 프레임별 실시간 추론
- 신뢰도 임계값 슬라이더, 시크바, LANDED/NOT LANDED 상태 표시

> 자세한 내용: [`GSI/landed_test_program/README.md`](GSI/landed_test_program/README.md)

---

## Repository Structure

```
PHD/
├── src/
│   └── sensorfusion/          # LiDAR-Camera Sensor Fusion GUI (PyQt5)
├── GSI/
│   ├── landed_test_program/   # Container Landing Detection (YOLOv8)
│   ├── auto_labelling/        # SAM 기반 자동 라벨링 도구 (React + FastAPI)
│   ├── Anti_Lift/             # Anti-Lift 감지
│   ├── et_value_test/         # ET 값 테스트
│   ├── homography/            # Homography 변환
│   └── renewal_etals/         # ETALS 리팩토링
└── research/                  # 연구 자료
```

## Tech Stack

| 분야 | 기술 |
|------|------|
| **Language** | Python 3.10+, TypeScript |
| **GUI** | PyQt5 |
| **CV / 3D** | OpenCV, PyVista, PyVistaQt, ouster-sdk |
| **Deep Learning** | PyTorch, Ultralytics YOLOv8, BERT, nn-UNet, VoxelMorph |
| **NLP** | HuggingFace Transformers, Contrastive Learning |
| **Scientific** | NumPy, SciPy |
| **Frontend** | React |

## Getting Started

```bash
# SensorFusion
cd src/sensorfusion
pip install -r requirements.txt
python main.py

# Landed Test Program
cd GSI/landed_test_program
pip install -r requirements.txt
python landed_detection.py
```

---

## Contact

- **Email**: [josehan1234@gmail.com](mailto:josehan1234@gmail.com)
