# Jo Siheon (조시헌)

**AI Vision Researcher — 3D Perception & Sensor Fusion**

Camera–LiDAR Sensor Fusion · Point Cloud Upsampling · Depth Estimation & 3D Reconstruction
<sub>(배경: Medical Image Analysis, NLP)</sub>

[![Gmail](https://img.shields.io/badge/Gmail-josehan1234%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:josehan1234@gmail.com)
[![GitHub Pages](https://img.shields.io/badge/Blog-joesiheon496.github.io-181717?style=flat&logo=github&logoColor=white)](https://joesiheon496.github.io/)

---

## 🔬 Research Interests

- **Camera–LiDAR Sensor Fusion** — 멀티모달 representation 학습 (박사과정 @ Hanyang CELOS)
- **Point Cloud Upsampling** — 희소 점군의 조밀 복원 (flow matching 등 생성 모델 기반)
- **Depth Estimation & 3D Reconstruction** — monocular / multi-view depth, point cloud
- <sub>(배경) Medical Image Segmentation·Registration, NLP 기반 특허 분류·검색</sub>

## 📝 Notes / Blog

논문·프로그램 정리 노트 → **[joesiheon496.github.io](https://joesiheon496.github.io/)**

- [Depth Anything 3 — 어떤 뷰에서든 3D 공간 복원](https://joesiheon496.github.io/posts/depth-anything-3/) *(paper)*
- [PUFM++ — Flow Matching으로 점군 업샘플링](https://joesiheon496.github.io/posts/pufm-plus-plus/) *(paper)*
- [Depth Anything 3 비디오 프레임 심도 테스터](https://joesiheon496.github.io/posts/depth-anything-3-video-tester/) *(program)*

---

## Career

### 한양대학교 박사과정 — 전자공학부 CELOS
`2026.02.11 ~ 재학중`

- **Sensor Fusion** (Camera + LiDAR) Representation 연구
- Point cloud upsampling

### 지에스아이 (GSI)
`2024.01.15 ~ 재직중`

- **항만 자동화** 연구 — 컨테이너 착지 감지, 자동 라벨링, Anti-Lift 등

### 팀바이오
`2023.03.10 ~ 2024.10.31`

- **nn-UNet** 기반 병변 이미지 탐색 (Medical Image Segmentation)
- **VoxelMorph**를 이용한 암 병변 크기 비교 (Deformable Registration)

### 한양대학교 석사과정 — 응용 물리학과 연구실
`2021.03.02 ~ 2023.02.15`

- BERT를 이용한 딥러닝 기반 **특허 자동 분류**
- Contrastive Learning을 이용한 **유사 특허 검색**

---

## Projects

### SensorFusion

Ouster OS1 LiDAR와 카메라 데이터를 융합하는 5단계 파이프라인 GUI 애플리케이션.

### Landed Test Program

컨테이너 착지(landed) 여부 판별 GUI 프로그램.

### Anti-Lift (항만 크레인 자동화)

항만 크레인 하역 과정에서 컨테이너와 함께 트럭 섀시가 들려 올라가는 상황(anti-lift)을 감지·방지하는 자동화 (GSI 항만 자동화 연구).

## Tech Stack

| 분야 | 기술 |
|------|------|
| **Language** | Python 3.10+, TypeScript |
| **CV / 3D** | OpenCV, Open3D, PyVista, PyVistaQt, ouster-sdk |
| **Deep Learning** | PyTorch, Depth Anything 3, Ultralytics YOLOv8, BERT, nn-UNet, VoxelMorph |
| **Methods** | Flow Matching, Contrastive Learning, Deformable Registration |
| **GUI** | PyQt5 |
| **NLP** | HuggingFace Transformers |
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
- **Blog**: [joesiheon496.github.io](https://joesiheon496.github.io/)
