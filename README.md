# Eggplant v1.0.0

 안녕하십니까?  **Eggplant** 프로젝트의 개발자 유이준입니다.  
위 마크다운 문서에서는 커서를 따라 흔들리는 3D 가지 웹 페이지(총칭 : Eggplant)에 관한 모든 정보들을 제공하고 있습니다.  
또한 모든 개발과 피드백의 근간은 위 문서에서 이루어지니, 참고해주시면 감사할 것 같습니다.  
추가로, 저작권은 <code>MPL 2.0 LICENSE</code>를 따르고 있으니 라이선스를 준수해주십시오.

## 목차
1. [Development - 업데이트 진행 사항](#release-notes)  
2. [Development - 업데이트 예정 사항](#upcoming-changes)  
3. [Development - 업데이트 논의 사항](#backlog)  
4. [GuideLines - 사용법](#사용법)  
5. [GuideLines - GitHub Pages 배포](#github-pages-배포)  
6. [GuideLines - 출처](#출처)  
7. [LICENSE](#-license-)

## < Development >
### Release Notes.
<pre><code>( 진행 완료 ) v0.0.1 Project Scaffolding   
( 진행 완료 ) v0.1.0 Procedural Eggplant Scene   
( 진행 완료 ) v0.2.0 Spring Bone Chain Motion   
( 진행 완료 ) v0.3.0 Shake Droplets And Credits   
( 진행 완료 ) **v1.0.0 DEPLOY**   </code></pre>  
---    
### Upcoming Changes.
<pre><code>1. Sketchfab 원본 모델(glb) 선택적 로드  </code></pre>  
---
### Backlog.
<code>업데이트 대기중입니다.</code>  

---
## < GuideLines >
### 사용법.
1. 페이지를 열면 이모지 모양으로 놓인 가지가 보입니다.  
2. 마우스(또는 손가락)를 움직이면 가지 꼭지가 커서에 붙고, 몸통은 스프링 관절처럼 늘어지며 흔들립니다.  
3. 빠르게 흔들다 멈추면 끝부분에서 물방울이 튀어나옵니다. (4.5초 쿨다운)  
4. 하단의 `???` 를 누르면 출처 팝업이 열리며, 2.5초 뒤 자동으로 사라집니다.  
---
### GitHub Pages 배포.
1. 저장소 루트에 `index.html` 을 둡니다. (빌드 과정 없음, three.js 는 jsDelivr CDN 에서 불러옵니다.)  
2. **Settings → Pages → Build and deployment** 에서 Source 를 `Deploy from a branch`, 브랜치 `main` / 폴더 `/(root)` 로 지정합니다.  
3. 잠시 뒤 `https://<사용자명>.github.io/<저장소명>/` 에서 확인합니다.  
* 로컬 확인  
    * `python -m http.server` 실행 후 `http://localhost:8000` 접속  
---
### 출처.
* 원작 : [🍆.ws](https://xn--gi8h42h.ws/) — Max van Leeuwen  
    * 동작(커서 추종·흔들림·물방울·`???` 팝업)을 참고해 코드를 새로 작성했습니다. 원작의 코드·모델·텍스처는 포함하지 않습니다.  
* 가지 모델 : three.js 로 코드에서 직접 생성 (Lathe·Tube 지오메트리 + SkinnedMesh 본 3개)  
    * 참고 모델 [Eggplant Emoji (animatezach)](https://sketchfab.com/3d-models/eggplant-emoji-531e2c549ae54b9189b460c2ff7e0e44) 는 **CC BY-NC-ND** (변경 금지) 라이선스라 리깅·수정본을 저장소에 넣을 수 없어 사용하지 않았습니다.  
---
## < LICENSE >
<pre><code>Mozilla Public License Version 2.0

Copyright (c) 2026 Yijun Yoo

This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this
file, You can obtain one at https://mozilla.org/MPL/2.0/.
</code></pre>  

전문은 저장소 루트의 [LICENSE](./LICENSE) 파일 또는 <https://mozilla.org/MPL/2.0/> 에서 확인하실 수 있습니다.
