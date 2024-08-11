## KaKao Map API README

### 프로젝트 제목
KaKao Map API Integration for Android

### 소개
이 프로젝트는 안드로이드 앱에서 카카오맵 API를 연동한 예제입니다. 사용자가 지도를 표시하고 현재 위치를 추적하는 기능을 구현합니다.

### 설치
프로젝트 실행 및 설치 방법입니다.

1. 리포지토리를 클론합니다.
   ```bash
   git clone https://github.com/Rachel-3/KaKao_Map_API.git
   cd KaKao_Map_API
   ```

2. 필요한 의존성을 설치합니다.
   - 프로젝트의 `build.gradle` 파일에서 필요한 의존성을 확인하고 설치합니다.
   - `gradle-wrapper.properties` 파일이 포함되어 있어 자동으로 Gradle 환경이 설정됩니다.
   
3. `gradle.properties` 파일에 카카오맵 API 키를 추가합니다.
   - 프로젝트 루트 디렉토리에 `gradle.properties` 파일을 생성하거나, 기존 파일이 있는 경우 열어 다음 내용을 추가합니다.
   ```properties
   kakaoApiKey=YOUR_API_KEY
   ```

4. `AndroidManifest.xml` 파일에 카카오맵 API 키를 설정합니다.
   - `AndroidManifest.xml` 파일에서 다음과 같이 카카오맵 API 키를 참조합니다.
   ```xml
   <meta-data
       android:name="com.kakao.sdk.AppKey"
       android:value="${kakaoApiKey}"/>
   ```

5. 앱을 빌드하고 실행합니다.
   ```bash
   ./gradlew build
   ./gradlew installDebug
   ```

### 사용 방법
이 프로젝트는 간단한 안드로이드 애플리케이션으로, 다음 기능을 구현합니다.

- **지도 표시** : `MainActivity.java` 파일에서 카카오맵을 초기화하고 지도를 표시합니다.
- **현재 위치 추적** : 사용자의 현재 위치를 추적합니다.

#### 주요 파일 및 디렉토리
- `app/src/main/java/com/example/locationscanner/MainActivity.java` : 메인 액티비티 파일로, 카카오맵을 초기화하고 현재 위치를 추적하는 기능을 구현합니다.
- `app/src/main/res/layout/activity_main.xml` : 메인 액티비티의 레이아웃 파일입니다.
- `app/libs/libDaumMapAndroid.jar` : 카카오맵 API 라이브러리입니다.
- `app/src/main/jniLibs/` : 네이티브 라이브러리 파일들이 포함되어 있습니다.

### 기술 스택
- **언어** : Java
- **플랫폼** : Android
- **빌드 도구** : Gradle
- **라이브러리** : 카카오맵 API

### 라이선스
이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

### 연락처
문의사항은 다음 이메일로 연락주세요.

- **Author** : Chae-rim Yoon
- **Email** : cofla226@naver.com
