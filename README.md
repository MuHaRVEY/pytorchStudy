# pytorchStudy

PyTorch의 핵심 개념을 기초부터 학습하고, 직접 모델을 구현하며 기록하는 저장소입니다.

## 학습 목표

- Tensor 연산과 GPU 사용법 익히기
- Autograd와 역전파 원리 이해하기
- `Dataset`과 `DataLoader`로 학습 파이프라인 구성하기
- `nn.Module` 기반 신경망과 학습 루프 직접 구현하기
- CNN, 전이학습, 모델 평가 경험하기
- 의료 영상 분류 미니 프로젝트로 전체 과정 정리하기

## 학습 계획

| 주차 | 주제 | 핵심 내용 |
|---|---|---|
| 1주차 | Tensor 기초 | 생성, 인덱싱, 브로드캐스팅, GPU |
| 2주차 | Autograd | 계산 그래프, gradient, 역전파 |
| 3주차 | 데이터 파이프라인 | Dataset, DataLoader, transform |
| 4주차 | 신경망 기초 | nn.Module, loss, optimizer |
| 5주차 | 학습 루프 | train/validation, checkpoint, 재현성 |
| 6주차 | CNN | 이미지 분류, 과적합, 정규화 |
| 7주차 | 전이학습 | 사전학습 모델, fine-tuning |
| 8주차 | 미니 프로젝트 | 의료 영상 분류 및 결과 분석 |

세부 체크리스트는 [`weeks/README.md`](weeks/README.md)에서 확인할 수 있습니다.

## 저장소 구조

```text
pytorchStudy/
├── notebooks/          # 실험 및 개념 확인용 노트북
├── src/                # 재사용 가능한 학습/평가 코드
├── weeks/              # 주차별 학습 기록
├── requirements.txt
└── README.md
```

## 시작하기

```bash
git clone https://github.com/MuHaRVEY/pytorchStudy.git
cd pytorchStudy

python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

설치 확인:

```python
import torch

print(torch.__version__)
print("CUDA available:", torch.cuda.is_available())
```

## 학습 기록 원칙

각 주차 폴더에 다음 내용을 남깁니다.

1. 새로 배운 개념
2. 직접 실행한 코드와 결과
3. 발생한 오류와 해결 방법
4. 다음 학습에서 확인할 질문

## License

This project is licensed under the [MIT License](LICENSE).
