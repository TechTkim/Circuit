# 구리 도선 꼬아 잇기 — AI 영상 생성 프롬프트

중학교 기술·가정 「센서 로봇 프로젝트」 수업용 실사 영상(약 24초, 16:9)을 AI 영상 생성 도구(Veo, Sora, Kling, Runway 등)로 만들기 위한 프롬프트입니다.
대부분의 도구는 한 번에 5~10초만 생성하므로 **8초 클립 3개**로 나눠 만든 뒤 이어 붙이는 것을 권장합니다.
영어 프롬프트가 한국어보다 결과가 안정적입니다.

> 참고: "도선은 처음부터 끝까지 직선"과 "한쪽 끝을 감는다"는 서로 충돌합니다.
> 아래 프롬프트는 **도선 몸체(피복 부분)는 직선 유지, 벗긴 3cm 구리 끝만 감긴다**로 정리했습니다.

---

## 공통 스타일 (모든 클립 끝에 붙이기)

```
Photorealistic educational video, strict top-down overhead camera, locked-off tripod shot, clean matte white workbench, bright soft even studio lighting with no harsh shadows, real copper metallic texture with subtle reflections, two thin insulated wires with about 3 cm of bare SOLID single-core copper conductor (one thick copper strand, not stranded), natural adult hands with five fingers each, slow deliberate realistic motion, high detail, sharp focus, 16:9, no other props, no text, no subtitles, no logos, no sparks, no soldering, no wire stripping.
```

## 공통 네거티브 프롬프트 (지원하는 도구만)

```
text, captions, watermark, logo, stranded wire, frayed strands, knot, tangled wire, coiled insulated wire, soldering iron, solder, sparks, fire, smoke, wire stripper, extra fingers, deformed hands, melting metal, warped wire, camera shake, dark lighting, cluttered background
```

---

## 클립 1 (0–8초) — 장면 1·2: 겹치기와 잡기

```
Top-down view of a white workbench. Two thin straight insulated wires lie horizontally, one entering from the left and one from the right, each with about 3 cm of bare solid copper at its tip. A pair of hands slowly slides the two bare copper ends toward each other so they lie side by side, parallel and overlapping by about 3 cm in the center of the frame. Then the left hand's thumb and index finger firmly pinch the overlapping copper section to hold it in place. The insulated parts of both wires stay perfectly straight.
```

## 클립 2 (8–16초) — 장면 3·4: 감기

```
Top-down view, same white workbench and same two wires held side by side with their bare solid copper ends overlapping in the center, the left fingers pinching the overlap. The right hand slowly wraps the bare copper tip of the right wire around the other straight copper conductor, making 4 to 5 tight, neat, evenly spaced turns that sit snugly against each other like a small spring. Then the hands rotate the wire and wrap the remaining copper tip of the left wire around the opposite side in the same tight neat way. The result is a clean, compact twisted splice, not a knot. The insulated parts of both wires remain straight in a single line.
```

## 클립 3 (16–24초) — 장면 5: 완성된 연결부 클로즈업

```
Top-down view of a white workbench with two straight insulated wires joined in one straight line by a finished twist splice in the center. The hands gently tug both wires outward to show the joint is mechanically firm and does not come apart, then move out of frame. The camera slowly and smoothly pushes in from directly above to a close-up of the copper joint: tight, uniform, evenly spaced coils of solid copper wrapped snugly around each other, no gaps, no loose ends sticking out, shiny realistic metal texture, sharp macro detail.
```

---

## 한국어 버전 (한국어만 받는 도구용, 하나로 합친 짧은 형)

```
흰색 실습 작업대를 바로 위에서 내려다보는 고정 탑뷰 실사 영상. 피복을 약 3cm 벗긴 가는 단선(굵은 구리선 한 가닥) 구리 도선 2개가 좌우에서 일직선으로 놓여 있다. 손이 두 구리 끝을 나란히 약 3cm 겹치고 손가락으로 겹친 부분을 단단히 잡는다. 한쪽 구리 끝을 다른 도선 둘레에 4~5바퀴 촘촘하고 일정한 간격으로 밀착해 감고, 반대쪽 끝도 같은 방식으로 감는다. 양쪽을 살짝 당겨 단단히 고정되었음을 보여준 뒤, 카메라가 천천히 연결부로 다가가 틈 없이 고르게 감긴 구리 코일을 선명하게 보여준다. 피복 부분은 끝까지 곧게 유지. 밝고 부드러운 조명, 실제 구리 금속 질감, 자연스러운 손, 16:9. 글자·자막·로고·납땜·불꽃·피복 벗기기 장면 없음, 매듭처럼 묶지 않음.
```

## 생성 팁
- 손가락 왜곡이 생기면 클립 2를 "hands partially out of frame, only fingertips visible"로 바꿔 다시 생성.
- 연선(여러 가닥)으로 나오면 "solid core copper wire, single thick strand, like 1.6 mm house wiring"을 앞쪽에 추가.
- 클립 간 연결이 어색하면 앞 클립의 마지막 프레임을 이미지로 넣어 다음 클립을 image-to-video로 생성.
