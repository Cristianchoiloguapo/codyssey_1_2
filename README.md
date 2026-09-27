# COLOMBIANA COLD BREW - AI Native Basic 1-2

AI 이미지, 비디오, 오디오 도구를 활용해 제작한 10초 이내 브랜드 광고 프로젝트입니다.

## Project

- **Brand:** COLOMBIANA COLD BREW
- **Target:** 새벽까지 일하거나 공부하는 20-40대
- **Tone & Manner:** Colombian heritage / cinematic / warm / refreshing
- **USP:** 콜롬비아 산지의 신선함이 도시의 피곤한 일상까지 직접 찾아오는 경험
- **Core Message:** **Wake up with Colombia.**
- **Final Duration:** 약 9.2초
- **Aspect Ratio:** 16:9

## Story

1. 새벽 도시에서 지쳐 일하는 직장인
2. 창밖 도시가 콜롬비아 커피 산지로 변환
3. 커피 농부와 당나귀가 창가로 접근
4. 직장인이 얼음잔을 내밀고 농부가 콜드브루를 따라줌
5. 한 모금 마신 뒤 만족하고 리프레시됨
6. 제품 히어로샷과 브랜드 메시지

## Tools

- **ChatGPT Image Generation** - 스토리보드 키 비주얼 및 광고 콘셉트 제작
- **Google Veo 3.1 Fast via Codyssey Media API** - 6개 씬 영상 생성
- **CapCut** - 컷 편집, 브랜드 텍스트, AI TTS, 최종 MP4 출력

## Production Pipeline

`기획 -> 이미지 키 비주얼 -> 영상 생성 -> 컷 편집 -> 텍스트/TTS -> 최종 MP4`

Codyssey Media API의 비디오 엔드포인트는 비동기 방식으로 사용했습니다.

1. 영상 생성 요청
2. `jobId` 수신
3. 상태 polling
4. `completed` 확인
5. MP4 다운로드
6. CapCut에서 6개 씬 통합 편집

## Prompt Improvement Example

### Before

농부가 머그컵을 건네는 장면 중심으로 생성되어 제품 자체의 존재감이 약했습니다.

### After

농부가 **COLOMBIANA COLD BREW 병**을 들고, 직장인이 내민 **투명 얼음잔에 직접 콜드브루를 따라주는 장면**으로 수정했습니다.

### Why

제품 노출을 강화하고, "콜롬비아 산지에서 도시의 사용자에게 직접 전달된다"는 핵심 아이디어를 한 장면에서 명확하게 보여주기 위해 수정했습니다.

## Final Files

- `Colombiana_ColdBrew_Storyboard.pdf` - 스토리보드 / 기획 / 프롬프트 / 제작 기록
- `20260927_final result.mp4` - 최종 광고 영상
- `README.md` - 프로젝트 설명

선택적으로 `scene01.mp4` ~ `scene06.mp4`, 프롬프트 기록, Python 영상 생성 코드를 추가할 수 있습니다.

## Notes

AI 비디오를 씬별로 생성하면서 인물과 의상 디테일이 일부 달라지는 문제가 있었습니다. 이를 짧은 컷 편집과 동일한 이야기 흐름, 색감, 제품 노출로 보완했습니다. AI가 생성한 병 라벨의 글자가 흔들릴 수 있어 최종 히어로샷에서는 CapCut 텍스트를 사용해 브랜드명을 정확하게 표시했습니다.

## Security

`.env` 파일과 API Key는 GitHub에 업로드하지 않습니다.

---
AI Native Basic 1-2 / Multimodal Brand Advertisement
