# EXAONE 3.5 2.4B 공공업무 자동화 모델 분석 보고서

우정사업본부 폐쇄망 환경에서의 온프레미스 SLM 도입 타당성을 분석한 기술 보고서입니다.

## 분석 대상

| 항목 | 내용 |
|------|------|
| 모델 | EXAONE-3.5-2.4B-Instruct-GGUF (Q6_K) |
| 개발 | LG AI Research |
| 파라미터 | 2.4B (가중치 약 2.14B) |
| 컨텍스트 | 32,768 토큰 |
| 토크나이저 | SuperBPE 기반, Vocab 102,400 |
| 라이선스 | EXAONE AI Model License 1.1-NC (비영리/내부 업무 허용) |

## 주요 내용

1. **모델 선택 이유** -- 보안·비용·한국어 효율 3가지 기준 충족
2. **학습 파이프라인** -- 2단계 사전학습 + SFT + DPO 정렬
3. **아키텍처 분석** -- GQA, RoPE, 30-layer Decoder-only Transformer
4. **모델 파일 구성** -- config.json, tokenizer, GGUF 가중치 등
5. **활용 가능 업무** -- 문서 초안 생성, HWP 요약, RAG 검색, 폐쇄망 AI 비서
6. **한계 및 주의사항** -- 환각 위험, 추론 한계, 양자화 손실, 라이선스 제약

## 빠른 실행

```bash
ollama run exaone3.5:2.4b
```

## 참고 링크

- [Hugging Face 모델 페이지](https://huggingface.co/LGAI-EXAONE/EXAONE-3.5-2.4B-Instruct-GGUF)
- [EXAONE 3.5 GitHub](https://github.com/LG-AI-EXAONE/EXAONE-3.5)
- [기술 논문 (arXiv)](https://arxiv.org/html/2412.04862v3)
- [Ollama 라이브러리](https://ollama.com/library/exaone3.5:2.4b)

---

**작성자:** 송정욱 (우정사업본부) · **AI 전문인재 과정 1일차**
