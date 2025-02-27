# WebDeck FAQ에 오신것을 환영합니다!
`ctrl+f`를 사용하여 원하는 내용을 쉽게 검색할 수 있습니다.

## WebDeck이란 무엇일까요?

WebDeck은 브라우저와 터치스크린이 있는 모든 장치에서 컴퓨터를 제어할 수 있는 애플리케이션입니다. 물리적 장비가 필요한 Elgato의 StreamDeck과 달리 WebDeck은 사용자가 자신의 컴퓨터에서 호스팅하고 터치스크린이 있는 장치에서 접속하는 웹 애플리케이션을 사용합니다.
<div align="center">
  <img src="https://i.imgur.com/OLE1oWk.png" alt="WebDeck example image" width="375" height="257">
</div>


## WebDeck은 어떻게 설치하나요?

1. GitHub의 [Releases](https://github.com/Lenochxd/WebDeck/releases) 에서 최신 버전의 WebDeck을 다운로드하세요.

2. `WebDeck-win-amd64-portable.zip`의 압축을 컴퓨터의 원하는 위치에서 압축 풀기 하세요.

3. 압축을 푼 폴더의 `WebDeck.exe` 파일을 실행합니다.

4. 모바일 장치에는 특별히 설치할 것은 없습니다. 작업 표시줄 오른쪽의 WebDeck 아이콘을 클릭하여 QR 코드를 스캔하면 됩니다.


## 사용 언어는 어떻게 변경하나요?

영어 이외의 언어를 사용하려는 경우 다음과 같은 단계에 따라 애플리케이션의 언어를 변경할 수 있습니다:

1. 애플리케이션 설정(구성)에 접속합니다.

2.  "Language" 항목의 사용 가능한 옵션 중에 원하는 언어를 선택합니다. 현재는 영어, 프랑스어, 한국어를 지원합니다. 한국어 번역은 모든 설정을 다루고 있지 않을 수 있습니다. 설정 페이지를 웹 브라우저가 지원하는 번역(일반적으론 마우스 오른쪽 버튼을 클릭하고 '한국어로 번역' 항목을 찾을 수 있습니다.)을 선택하면 이 문제를 해결할 수 있습니다.

3. 앞으로는 사용자가 자신이 선호하는 언어로 애플리케이션을 쉽게 번역할 수 있도록 할 계획입니다.

이런 방식으로 언어 기본 설정에 따라 응용 프로그램의 언어를 사용자 정의할 수 있습니다.


## 사운드보드를 어떻게 설정하나요?

애플리케이션의 사운드보드를 구성하려면 다음 단계를 따르세요:

1. **VB-CABLE 드라이버 설치:**
   - [이 링크](https://download.vb-audio.com/Download_CABLE/VBCABLE_Driver_Pack43.zip)에서 드라이버를 다운로드합니다.
   - 다운로드 받은 파일을 압축 풀기 합니다.
   - `VBCABLE_Setup_x64.exe` 파일을 실행하세요. (관리자 권한이 필요할 수 있습니다.)
   - "Install Driver"를 클릭하세요.
   - 컴퓨터를 다시 시작합니다.

2. **VLC 미디어 플레이어 설치:**
   - VLC 미디어 플레이어가 컴퓨터에 설치되어 있지 않다면 [이 링크](https://www.videolan.org/vlc/download-windows.html)에서 다운로드하세요.
   - 안내에 따라 설치를 진행하세요.
   - VLC는 사운드보드에서 사운드를 재생하는데 필수적입니다. 하지만 사운드보드가 작동하기 위해 소프트웨어를 한 번이라도 작동시킬 필요는 없습니다. 설치만으로도 충분하며 완벽하게 작동 할 것입니다.

3. **WebDeck 설정 구성:**
   - WebDeck 설정을 엽니다.
   - "Soundboard" 항목까지 스크롤합니다.
   - 사용할 입력 마이크를 선택하세요.
   - 출력으로는 "CABLE Input (VB-Audio Virtual Cable)" 을 선택합니다.

4. **외부 소프트웨어 설정 구성:**
   - 사운드보드를 사용하려는 소프트웨어의 설정을 열고 마이크 입력으로 "CABLE Output (VB-Audio Virtual Cable)" 을 선택했는지 확인하세요.

5. **Discord 구성:**
   - Discord에서 사운드보드를 사용하려는 경우, "사용자 설정 > 음성 및 비디오(Settings > Voice & Video)" 에서 "자동으로 입력 감도 조절하기(Automatic Gain Control)" 기능을 비활성화하세요.
   - 노이즈 억제 기능을 사용하면 음질이 왜곡될 수 있으니 주의하세요.

6. **소리 추가:**
   - Q 키로 버튼을 추가합니다.
   - "사운드보드" 항목에서 "오디오 재생" 항목으로 이동합니다.
   - 오디오 파일을 **MP3 형식**으로 가져옵니다.

이제 애플리케이션의 사운드보드를 성공적으로 구성했습니다. 사운드를 재생하려면 관련 버튼을 누르세요.


## OBS Studio를 어떻게 설정하나요?

OBS 웹소켓을 구성하려면 다음 단계를 따르세요:

1. OBS Studio 를 열고 "도구 > WebSocket 서버 설정(`Tools > WebSocket Server Settings`)" 으로 이동합니다.

2. "WebSocket 서버 사용(Enable WebSocket server)" 체크박스가 선택되어 있는지 확인합니다.

3. WebDeck의 설정에서 OBS Studio 항목까지 스크롤합니다.

4. OBS에서 제공하는 임의로 생성된 서버 포트와 서버 비밀번호를 복사하여 WebDeck 설정에 입력하세요.

5. 설정을 저장하면 완료됩니다! 이제 OBS 가 WebDeck에 연결되었습니다!


## Spotify 계정을 연결하는 방법

Spotify 계정을 WebDeck에 연결하려면 다음의 간단한 단계를 따르세요:

1. [Spotify 개발자 대시보드](https://developer.spotify.com/dashboard)에서 Spotify 계정에 로그인합니다.

2. 파란색의 "앱 만들기(Create app)" 버튼을 클릭하여 새 애플리케이션을 만듭니다.

3. 다음과 같이 양식을 작성하세요:
   - 이름 및 설명(Name and Description): 원하는 이름과 설명을 적어주세요.
   - 리디렉션 URI(Redirect URI): `http://localhost:8888/callback`을 입력합니다.

4. 이용 약관에 동의하기 위해 확인을 선택하세요.

5. "저장(Save)"을 클릭하여 앱을 저장하세요.

6. 홈페이지에 접속한 후 오른쪽 메뉴에서 "설정(Settings)"을 클릭하세요.

7. "Client ID"를 복사하고 아래의 "View client secret" 를 클릭하여 클라이언트 비밀번호도 복사하세요. WebDeck을 구성하려면 이 정보가 필요합니다.

8. WebDeck에서 설정의 Spotify API에 "Spotify 사용자 이름(Username)", **Client ID**, **Client Secret** 를 입력하세요.

9. 구성을 저장하면 끝입니다! 이제 여러분의 Spotify 계정이 애플리케이션에 연결되었습니다!

Spotify를 WebDeck 애플리케이션에 인증하는데에 필요하므로 "Client ID"와 "Client Secret"을 안전하게 유지하세요.


## 애플리케이션을 재설정하고 싶습니다. 어떻게 하나요?

구성을 재설정하는 과정은 간단합니다. 다음과 같이 시도하세요:

1. 시스템의 애플리케이션을 실행한 폴더에 접근하세요.
2. `.config/config.json` 파일을 찾아 엽니다.
3. 이 파일을 삭제하거나 이름을 바꾸세요.
4. 애플리케이션을 다시 시작합니다.

이 단계가 완료되면 애플리케이션 설정이 기본값으로 재설정되므로 필요한 경우 초기 구성으로 다시 시작할 수 있습니다.


## 버튼에 Gif를 넣을 수 있나요?

물론입니다! 버튼을 만들거나 편집할때 '.gif' 파일을 버튼 이미지로 쉽게 추가할 수 있습니다.

버튼 이미지에 허용되는 파일 형식은 다음과 같습니다:
`.jpg`, `.jpeg`, `.png`, `.gif`, `.svg`, `.webp`, `.bmp`, `.ico`, `.tiff`, `.tif`, `.heif`, `.heic`, `.apng`, `.mng`


## 버튼 뒤의 배경을 어떻게 커스터마이징 할 수 있나요?

배경을 커스터마이징 하는것은 매우 쉽습니다. 다음의 간단한 단계를 따르세요:

1. 애플리케이션 설정을 엽니다.
2. 설정 메뉴 중 "배경 메뉴 열기" 버튼을 선택합니다.
3. 이 메뉴를 사용하면 색상이나 배경 이미지를 쉽게 추가할 수 있습니다. 사용자가 원하는 만큼 추가할 수 있습니다.
4. 페이지가 로드되면 선택한 배경 중에서 랜덤한 배경이 선택됩니다.
5. 특정 배경을 비활성화하려면 해당 배경 오른쪽에 있는 확인란을 선택하면 됩니다.
6. 배경을 제거하려면 해당 삭제 아이콘을 클릭합니다.

이렇게 하면 단 몇 번의 클릭만으로 버튼 배경을 원하는 대로 커스터마이징 할 수 있습니다.


## VLC 미디어 플레이어가 필요한 이유는 무엇입니까?

WebDeck은 사운드보드에서 사운드를 재생하려면 `python-vlc` 라이브러리가 필요합니다. 따라서 VLC 소프트웨어 인터페이스를 사용하지 않더라도 컴퓨터에 VLC 미디어 플레이어를 설치하는 것이 중요합니다. 안타깝지만 현재까지 이 요구 사항을 우회할 수 있는 대체 솔루션은 확인되지 않았습니다.

**참고:** 이 종속성은 현재 제한 사항이며 WebDeck 개발 팀은 향후 업데이트에서 사용자 경험을 간소화하기 위해 잠재적인 대안을 적극적으로 탐색하고 있습니다.


## 소프트웨어가 서버와 통신합니까?

맞기도 하지만 아니기도 합니다. 실제 WebDeck은 서버와 통신을 설정하지만 해당 서버는 사용자가 사용중인 컴퓨터입니다. 모바일 장치의 WebDeck은 단순한 웹 페이지이며, WebDeck이 연결하는 "서버"는 사용자가 사용중인 컴퓨터입니다. 이 두 장치간의 통신은 로컬 네트워크를 통해 이루어집니다. 즉, 여러분의 컴퓨터는 서버 역할을 하지만 이 서버에 대한 접근은 사용자 본인에게만 허용됩니다.

사용자의 컴퓨터가 아닌 **다른** 서버와 통신하는 소프트웨어에 관한 질문이라면 대답은 '아니오' 입니다. 최대한의 보안을 보장하기 위해 데이터가 네트워크 외부로 유출되지 않습니다. 집 외부로 전송되는 유일한 데이터는 Spotify에 대한 API 요청이지만 이 데이터는 전용 WebDeck 서버가 아니라 바로 Spotify 서버로 이동합니다.


## "열기" 버튼을 통해 소프트웨어 이외의 파일도 열 수 있나요?

당연합니다! 파일을 선택할 수 있는 옵션이 있으며 해당 파일은 해당 기본 응용 프로그램으로 열립니다. 예를 들어, 이미지 열기를 선택하면 일반적인 이미지 뷰어에서 자동으로 열립니다.


## 저는 개발자입니다. 페이지의 CSS 를 어떻게 커스터마이징 할 수 있나요?

개발자가 원하는 대로 페이지의 CSS를 커스터마이징하여 테마를 생성할 수 있습니다. 몇 가지 간단한 단계를 통해 이를 수행하는 방법은 다음과 같습니다:

1. 설정 > '테마 메뉴 열기' > '테마 폴더 열기'로 이동하여 애플리케이션의 `.config/themes/` 폴더에 접근합니다.
2. 새 CSS 파일을 수동으로 생성하거나 기존 파일을 복제하여 커스터마이징을 시작합니다.
3. 생성한 CSS 파일에서 필요에 따라 테마 정보를 편집하여 다음 구조를 따르는지 확인합니다.:

```css
/*
theme-name = MyTheme
theme-description = My custom theme description :)
theme-icon = https://i.imgur.com/qhaL1EU.png
theme-author-github = YourGithubHere
*/

/* ------------------------------------------------------ */
```

4. WebDeck 구성 페이지를 다시 로드합니다.

이 단계가 완료되면 설정에서 자신만의 테마를 선택할 수 있습니다. 필요에 따라 CSS를 자유롭게 수정하고 원하는 대로 페이지 모양을 커스터마이징 할 수 있습니다. 원하는 경우 .css 파일을 다른 사용자와 공유할 수도 있습니다.


## 제 백신에서 WebDeck이 악성 코드로 감지되는 이유는 무엇인가요?

저도 잘은 모르겠습니다만, WebDeck은 오픈 소스이기 때문에 악성코드가 걱정 되는 경우, 직접 확인해보시면 좋습니다.
그렇지만 걱정마세요, WebDeck은 분명히 악성 애플리케이션이 아닙니다.


## 소프트웨어를 직접 컴파일 할 수 있나요?

보안상의 이유로 실행 파일을 직접 컴파일 하려는 경우 다음 단계를 따르세요.

1. 소스 코드를 다운로드하고 압축을 풉니다.
2. 소스코드 폴더에서 터미널을 엽니다.
3. 가상 환경을 생성합니다.:\
`python -m venv webdeck`\
`webdeck\Scripts\activate.bat`
4. 종속성을 설치합니다.:\
`pip install -r requirements.txt`
5. 컴파일을 시작합니다.:\
`python setup.py build`
6. (선택사항) sigtool을 사용하여 실행 파일에 서명하려면 [이 링크](https://stackoverflow.com/a/52963704/17100464)에 제공된 지침을 따르세요.
7. `signtool sign /a /fd SHA256 /tr http://timestamp.digicert.com /td SHA256 WebDeck.exe`
8. `signtool sign /a /fd SHA256 /tr http://timestamp.digicert.com /td SHA256 update.exe`