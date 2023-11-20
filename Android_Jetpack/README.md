# 🌷 Android Jetpack
```
✅ 2023.11.20.월  
```

---

## 👋🏻 Contents
- [x] [1️⃣ Android Jetpack이란?](#1️⃣-Android-Jetpack이란?)
- [x] [2️⃣ Jetpack 라이브러리 사용 방법](#2️⃣-Jetpack-라이브러리-사용-방법)
- [x] [3️⃣ Jetpack 라이브러리 종류](#3️⃣-Jetpack-라이브러리-종류)

---

## 1️⃣ Android Jetpack이란?
> Jetpack은 개발자가 중요한 코드에 집중할 수 있도록 권장사항 준수, 상용구 코드 감소, 여러 Android 버전과 기기에서 일관되게 작동하는 코드 작성을 돕는 **라이브러리** 묶음입니다.

<img width="750" alt="Jetpack" src="https://github.com/jmi-log/jmi-android/assets/76805879/f728dfa8-8b76-432a-aba6-fdbd488c4a43" />
<br /><br />

- Jetpack은 위 사진에서 볼 수 있는 Android 라이브러리들을 사용할 수 있는 **라이브러리 묶음**이다.  
- 권장사항이 통합되어 있고 Android 앱의 **이전 버전과의 호환성**을 제공하기 때문에 버전에 관계 없이 다양한 버전의 Android 플랫폼에서 앱 실행이 가능하다.
- 전체 Jetpack 라이브러리: https://developer.android.com/jetpack/androidx/explorer?hl=ko 

---

## 2️⃣ Jetpack 라이브러리 사용 방법
> [참고 URL](https://developer.android.com/jetpack/getting-started?hl=ko)
- settings.gradle 파일을 열고 아래와 같이 dependencyResolutionManagement { repositories {...}} 블록에 google() 저장소를 추가
```
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        jcenter()
    }
}
```
<br />

- Jetpack 구성요소(예: LiveData, ViewModel과 같은 아키텍처 구성요소)를 모듈의 build.gradle 파일에 추가
```
dependencies {
    val lifecycle_version = "2.2.0"

    implementation("androidx.lifecycle:lifecycle-livedata-ktx:$lifecycle_version")
    implementation("androidx.lifecycle:lifecycle-viewmodel-ktx:$lifecycle_version")
    ...
}
```

---

## 3️⃣ Jetpack 라이브러리 종류
> [전체 라이브러리](https://developer.android.com/jetpack/androidx/explorer?hl=ko)
- [Navigations]()
