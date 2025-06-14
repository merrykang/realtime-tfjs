# 👉🧑🕺 손 모양, 얼굴, 포즈 인식 AI 기능 개발 프로젝트

- 실시간 웹캠 영상 분석을 통해 사용자의 손 모양, 얼굴, 포즈를 인식 및 예측하여 인터랙티브한 블록 코딩 학습 환경을 구현합니다.
- 멀티 플랫폼 및 저사양 기기에서도 안정적으로 작동하도록 WASM 백엔드 최적화와 오프라인 환경에 대응하여 사용성을 높이기 위해 노력하였습니다.

</br>

# 🗓️ Period
- 2023년 10월 ~ 2024년 1월 (개발)
- 2025년 3월 ~ 4월 (배포)

</br>

# 🤝 발주처 및 근무처 
로보로보 - 에듀테크 연구소

</br>

# ⚙️ Stacks

<table>
  <tr>
    <td><b>✔️ Language</b></td>
    <td>
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?&style=for-the-badge&logo=JavaScript&logoColor=black"/>
    </td>
  </tr>
  <tr>
    <td><b>✔️ Frontend</b></td>
    <td>
      <img src="https://img.shields.io/badge/React-61DAFB.svg?&style=for-the-badge&logo=React&logoColor=black"/>
    </td>
  </tr>
  <tr>
    <td><b>✔️ Backend</b></td>
    <td>
      <img src="https://img.shields.io/badge/Node.js-339933.svg?&style=for-the-badge&logo=Node.js&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><b>✔️ AI</b></td>
    <td>
      <img src="https://img.shields.io/badge/TensorFlow.js-FF6F00.svg?&style=for-the-badge&logo=TensorFlow&logoColor=white"/>
      <img src="https://img.shields.io/badge/Object--Detection-FF6F00.svg?&style=for-the-badge&logo=TensorFlow&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><b>✔️ Build & Deployment</b></td>
    <td>
      <img src="https://img.shields.io/badge/Electron-47848F.svg?&style=for-the-badge&logo=Electron&logoColor=white"/>
      <img src="https://img.shields.io/badge/AWS%20Lightsail-FF9900.svg?&style=for-the-badge&logo=Amazon%20AWS&logoColor=white"/>
    </td>
  </tr>
  <tr>
    <td><b>✔️ Environment</b></td>
    <td>
      <img src="https://img.shields.io/badge/Visual%20Studio-5C2D91.svg?&style=for-the-badge&logo=Visual%20Studio&logoColor=white"/>
      <img src="https://img.shields.io/badge/Git-F05032.svg?&style=for-the-badge&logo=Git&logoColor=white"/>
      <img src="https://img.shields.io/badge/Jira-0052CC.svg?&style=for-the-badge&logo=Jira&logoColor=white"/>
      <img src="https://img.shields.io/badge/Confluence-172B4D.svg?&style=for-the-badge&logo=Confluence&logoColor=white"/>
    </td>
  </tr>
</table>

</br>

# 📜 Outputs

### 1. 시뮬레이션 영상 (손 모양, 얼굴 인식)
- 사용자는 아래의 인식된 결과(얼굴 크기, 엄지 손가락 위치 등)를 활용하여 블록 코딩 작업을 수행할 수 있습니다.

<video src="https://private-user-images.githubusercontent.com/121994108/453796062-b12e5b29-1d99-46e7-a24f-e8c7988952e3.mp4?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDk2Mjc2NzEsIm5iZiI6MTc0OTYyNzM3MSwicGF0aCI6Ii8xMjE5OTQxMDgvNDUzNzk2MDYyLWIxMmU1YjI5LTFkOTktNDZlNy1hMjRmLWU4Yzc5ODg5NTJlMy5tcDQ_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNjExJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDYxMVQwNzM2MTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hNjZlNmMwZTBlYjZkZmQyYjQyY2VlN2EwZDI3ODQ5NTYzMDg2YTA0YjdhNDJiOWNjMzczMzA1MmFmMjAzOTlhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.wBrB4HtQ_3lG9g6sShd76GXO3DB9mZRz13ydNcPEFLw" width="300" controls></video>

### 2. 예측 결과 예시
- 아래는 손 모양 인식 모델이 반환하는 예측 결과 예시 JSON 구조입니다.
```json
{
  "detected": [
    {
      "box": {
        "height": 239.49,
        "width": 193.32,
        "xMin": 100.69,
        "xMax": 294.02,
        "yMin": 18.08,
        "yMax": 257.57
      },
      "keypoints": [
        { "x": 247.63, "y": 176.64, "z": -33.24, "name": "lips" },
        { "x": 234.39, "y": 97.83, "z": -4.72, "name": "rightEye" },
        { "x": 220.13, "y": 59.78, "z": 9.82, "name": "faceOval" }
        // ...
      ]
    }
  ]
}
```

</br>

# 🧰 핵심기능
## 👉 손 모양 인식
- 스미싱 : [번호 조회](#스미싱-및-보이스-피싱-번호-조회), [AI 문자 분석](#ai-문자-분석), [대응 방안 상세보기](#대응-방안-상세보기) 의 순서로 안내합니다.
- 보이스 피싱 : [번호 조회](#스미싱-및-보이스-피싱-번호-조회), [대응 방안 상세보기](#대응-방안-상세보기) 의 순서로 안내합니다.
- 메신저 피싱 : [링크 조회](#스팸-링크-조회), [AI 내용 분석](#ai-내용-분석), [대응 방안 상세보기](#대응-방안-상세보기) 의 순서로 안내합니다.

- 
## 🧑 얼굴 인식
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/092b0f9a-0409-4969-a229-477ca8d25b09">
</details>
<p>번호를 입력하고 조회합니다.</p>
</div>

## 🕺 포즈 인식
<div>
<details>
<summary>사진 보기</summary>










<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/63a08450-d39b-421f-af25-72be7d85c639">
</details>
<p>의심스러운 사이트 링크를 조회할 수 있습니다.</p>
</div>

### 📄 대응 방안 상세보기
조회와 결과 확인을 마친 후 사용자는 [매뉴얼 조회](#매뉴얼-조회), [체크리스트 조회](#체크리스트-조회), [주변 기관 찾기](#주변-기관-찾기)로 대응 방안을 안내받을 수 있습니다.
스팸 문자나 메신저를 이용한 메신저 피싱의 경우에는 [AI 내용 분석](#ai-내용-분석)을 통해 상세 내용을 입력하면 AI 문맥 분석을 통해 해당 내용이 스팸인지 아닌지를 알려드리고 대응 방안 상세보기 페이지로 이동할 수 있습니다.

### 📜 매뉴얼 조회
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/ca286c56-1b60-43d6-8bd9-125b98f00e46">
</details>
<p>사용자를 위한 금융 피싱 사기 대처 매뉴얼이 제공되며 우측 상단의 슬라이더를 이용해 글자 크기를 조절할 수 있습니다.</p>
</div>

### 📑 체크리스트 조회
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/5afdc0d8-33a7-4c8e-8dd9-b4a9434cd1a7">
</details>
<p>금융 피싱 사기가 발생했을 때 사용자가 취해야 하는 행동을 체크리스트로 안내하고 저장을 누르면 사용자의 계정에 저장됩니다.</p>
</div>

### 🚔 주변 기관 찾기
<div>
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/36d8a80a-0a79-49ae-b19a-a977812d063c">
</details>
<p>위의 네비게이션 바와 대응 방안 상세보기 페이지의 가까운 기관 찾기 버튼을 누르면 사용자의 주소 근처의 은행과 경찰서를 보여줍니다.</p>
</div>

### 💻 AI 내용 분석
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/4a182052-b3a6-44b2-9f13-5c0daa5b0aa9">
</details>
<p>스팸으로 의심되는 문자 번호를 조회해본 후 해당 번호가 기록에 존재하지 않는다고 했을 때,
해당 문자의 내용을 인공지능을 이용한 문맥 분석으로 해당 문자가 금융 피싱 사기에 연루되었는지를 판단할 수 있습니다.</p>
</div>

### 📰 유사 사례 검색
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/33ad0b63-1b6e-4036-afe3-8b520baddbc0">
</details>
<p>사용자가 입력 뿐만 아니라 태그로 빠르게 자신과 유사한 사례를 검색할 수 있습니다.</p>
</div>

## 👮 고객별 피싱 예방 기능
사용자는 계좌를 생성하고 위험 한계치를 함께 입력하여 자신의 스마트폰으로 언제든지 
Crime-Fin 카카오톡 맞춤형 긴급 알림을 수신해 자신의 자산 알림을 받을 수 있습니다. 
또한, 대시보드 페이지에서 사용자의 자산 현황을 한눈에 볼 수 있습니다.

### 💰 계좌 생성
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/97f5263b-e9de-4df0-b00e-c5d453c224d9">
<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/59c54ac6-5caf-4cfa-aef9-731568c5a7f2">
</details>
</div>
은행에 해당 계좌가 있는지 확인한 뒤, 1원 입금 인증 시스템을 통해 비밀 입금자명을 입력하면 인증이 완료됩니다. 

### 🚨 실시간 위험 알림
<div>
<details>
<summary>사진 보기</summary>

<span>
<img width="300" alt="위험알림" src="https://github.com/kb-final-team4/crimefin/assets/33799946/1fbedb94-34d8-40b6-bd11-6a544dedc415">
<img width="300" src="https://github.com/kb-final-team4/crimefin/assets/33799946/f30c765a-4826-4166-a04f-94ea3d97313d">
</span>
</details>
</div>
사용자가 미리 설정해놓은 위험 한도치를 넘어서게 되면 알림이 오게 됩니다.

### 📊 대시보드
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/dbff1bfc-fe30-41f8-a1b0-2e62da9c4437">
</details>
<p>도넛 차트에서 전체 구성 현황을 확인할 수 있고 우측 하단의 날짜 상세 조회를 이용하면 특정 날짜 구간의 거래내역 조회와 그래프를 볼 수 있습니다.</p>
</div>

## 👮 피싱 예방 테스트 
간단한 테스트로 피싱 체험을 통해 사용자가 피싱 사기에 항상 주의할 수 있도록 합니다.
### 🤹 메신저 피싱 테스트
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/49837223-8988-41ba-ae6c-5b36137c81fe">
</details>
</div>
역할을 고르고 각 역할에 맞는 상황을 랜덤하게 준비하여 피싱 사기범이 대화에서 어떻게 유도하고 어떤 대답을 해야 예방할 수 있는지를 체험해 볼 수 있는 테스트입니다.

### 🤹 보이스 피싱 대처 유형 테스트
<div>
<details>
<summary>사진 보기</summary>

<img src="https://github.com/kb-final-team4/crimefin/assets/33799946/4140adbd-c27f-4b28-8e2f-fea50b79abcf">
</details>
<p>간단한 상황 설명과 그 상황에서 자신이 할 법한 대답을 고르면 됩니다.</p>
</div>

---
# 🧐 Trouble Shooting

## 💻 오프라인 환경 지원

## 저사양 기기 지원

## 모델 로딩 로직 개선

## 멀티 플랫폼 지원



















**❗️문제 상황**

    사용자의 자산을 나타내는 대시 보드에서 도넛 차트와 막대 그래프가 업데이트 되지 않는 문제점 발생

**👨‍💻해결 방안 탐색**

1. Vue.js 라이프 사이클의 이해
2. 공식 API 문서 정독

**👍해결**

`$ref` 로 **dom** 요소에 직접 접근한 뒤 `refresh()` 메서드로 데이터 업데이트

### 2. **라우터 페이지 이동**

❗️**문제 상황**

    시작 페이지에서 여러 섹션을 나누어 다양한 컴포넌트를 표시한 후, 특정 페이지로 이동하면 하나의 컴포넌트만

    보이게 하는 것이 정상이다. 하지만 시작하는 vue인 App.vue에서 두개의 컴포넌트를 import한 뒤,

    페이지 이동버튼을 클릭했을 때 두 컴포넌트가 동시에 한 페이지로 이동하지 않는 문제 발생

**👨‍💻해결 방법**

**App.vue**에서는 하나의 컴포넌트만 보이도록 변경하였고, 시작 페이지에서 필요한 두 컴포넌트를 하나의 컴포넌트로 감싸서 import하는 방식으로 구현

**🤔문제 발생 이유 분석**

Vue.js의 라우팅 시스템에서는 `<router-view/>` 태그에 지정된 경로의 컴포넌트만을 렌더링.
 **App.vue**에서 두 컴포넌트를 따로 import하고 섹션을 나누었기 때문에, `<router-view/>`에 해당하는
영역이 없었던 것으로 예상

**📈결과**

한 페이지에 하나의 컴포넌트만 보이도록 수정한 결과 원활하게 페이지 이동이 가능.

### 3. **모달창 구현과 컴포넌트 간 데이터 전달**

**❗️문제 상황**

    Vue.js를 활용하여 모달창을 구현하면서 데이터를 주고받는 형식과 모달창을 띄우는 방법에 대한 어려움 발생

**👨‍💻해결 방법**

Vue의 **lifecycle**과 양방향 데이터 전달 방식에 대해 학습하고 이를 적용하여 문제 해결

**🤔문제 발생 이유 분석**

Vue.js의 특정 기능인 모달창 구현과 데이터 전달 방식에 대한 이해도가 충분하지 않았기 때문에, 이를 제대로 구현하는데 어려움이 있었음

**📈결과**

번호 조회, AI 조회 등 피싱 대응 기능에 대해 모달창으로 구현하며 페이지 이동 없이 결과를 볼 수 있도록 구현

---
## 📡 Back-End

### 1. **Session**

**❗️문제 상황**

    로그인에 성공한 사용자의 정보를 Session에 바인딩하는 것은 성공했지만, 페이지가 넘어갈 때 마다

    Session이 새로 생성되어 사용자의 정보를 활용할 수 없는 문제점 발생

**👨‍💻해결 방안 탐색**

1. Spring 공식 document를 보며 `HttpServletRequest` 와 `HttpSession` 에 대해서 공부
2. Front-End 와 Back-End의 포트번호가 달라 CORS를 설정하는 코드에 문제가 발생할것이라고 예상. 
   따라서 CORS(Cross-Origin Resource Sharing) 코드 부분 수정


**👍해결**

```java
@Override
public void addCorsMappings(CorsRegistry registry) {
	registry
				  .allowCredentials(true) //수정 사항!!
	}
}
```

위와 같이 `allowCredentials` 를 true로 설정하여 cookie, HTTP 기본 인증 등을 사용할 수 있도록 허용. 따라서 인증된 요청을 처리 가능

---
# 🤖 AI

### **1. Front → Back → AI 연결 과정**

**❗️문제 상황**

    클라이언트 측에서 사용자의 피싱 메시지를 바탕으로 AI 맥락 조회 기능을 사용하려 하는 상황에서

    JSON Parse 에러 발생

**👨‍💻 문제 인식**

JSON 데이터를 역직렬화 하는 동안 발생한 문제

즉, 클라이언트는 단일 객체 형태로 데이터를 보내지만,
Back-End에서는 `ArrayList<HashMap<String, Object>>` 유형으로 데이터를 기대하여 양자의
불일치로 문제 발생

**👍해결**

클라이언트 코드에 **Content-Type**헤더를 설정하고 클라이언트 코드에 데이터 변수에 저장되는 값 앞뒤에
대괄호 [] 를 추가하여 Back-End가 기대하는 데이터 유형으로 만들어서 해결

이 외에도 클라이언트가 데이터 유형을 Back-End가 기대하는 방식이 아닌 다른 방식으로 넘겨준 경우,
Back-End가 알아서 역직렬화 하도록 DTO를 만드는 방법을 탐색

### **2. 크롤링**

**❗️문제 상황**

    뉴스 기사를 크롤링하여 학습시킬 데이터를 csv 형태로 저장하려고 하는 상황에서

    timeout 및 connectionError 에러 발생

**👨‍💻 문제 인식**

일정 횟수 이상으로 크롤링 요청하여 웹페이지에서 해당 요청을 이상 있는 기계로 받아들여 요청을 차단하여 발생한 문제

**👍해결**

웹페이지에 해당 요청이 기계가 아닌 사람임을 알려주기 위해 **headers**에 **User-Agent**를 명시하여
요청 전송

