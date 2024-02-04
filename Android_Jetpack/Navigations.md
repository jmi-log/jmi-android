# 🌷 Navigations
```
✅ 2023.11.20.월
```

---

## 👋🏻 Contents
- [x] [1️⃣ Jetpack Navigation이란?](#1️⃣-Jetpack-Navigation이란?)
- [x] [2️⃣ Safe Args](#2️⃣-Safe-Args)
- [x] 3️⃣ Deep Link
- [x] 4️⃣ Navigation Graph
- [x] 5️⃣ 총 정리

---

## 1️⃣ Jetpack Navigation이란?
> Jetpack Navigation은 Application의 화면 구성을 쉽게 구현하고 화면의 흐름을 시각적으로 보여줄 수 있는 구성 요소이다.

<img width="300" alt="Jetpack Navigation" src="https://github.com/jmi-log/jmi-android/assets/76805879/3a6f1ce6-c6d6-4d76-acf4-a9f4304fecb9" />
<br /><br />

- Activity, Fragment 간 **데이터 전달**, **화면 이동** 등의 code 구현을 심플하고 안정적으로 처리 가능하다.
- 개발자가 정의한 **UI Graph**를 기반으로 화면을 쉽게 전환하고, **유지보수가 간편**해진다.
- Jetpack Navigation 사용 방법: https://developer.android.com/codelabs/android-navigation?hl=ko#0
  

### 🟡 [구성 요소]
- **NavGraph(탐색 그래프)**
  - 모든 탐색 관련 정보가 하나의 중심 위치에 모여 있는 XML 리소스
  - Destinations과 이들을 연결하는 Actions들을 시각화해서 볼 수 있다.
  - Destinations: Navigation을 이용해 이동하는 앱의 목적지를 의미

- **NavHost**
  - 탐색 그래프에서 대상을 표시하는 빈 컨테이너
  - NavGraph에 정의한 Desination들을 보여주기 위해 NavHostFragment를 이용한다.

- **NavController**
  - NavHost에서 앱 탐색을 관리하는 객체
  - NavController는 사용자가 앱 내에서 이동할 때 NavHost에서 대상 콘텐츠의 전환을 설정, 관리, 조정한다.

---

## 2️⃣ Safe Args
