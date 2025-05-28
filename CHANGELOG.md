## [LATEST] 2025/05/28 - [v1.0.1](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v1.0.1)

### NOTE

1. 브라우저의 쿠키를 이용해 로그인할 수 있습니다.
   - 현재 크롬과 엣지 브라우저에서 쿠키를 가져올 수 없는 버그가 존재하여 임시로 비활성화하였습니다. 크롬 사용자께서는 도움말을 참고하여 사용해 주시기 바랍니다.
   - 엣지 브라우저의 경우, 보안상 안전하다고 판별된 쿠키 추출 확장 프로그램이 없어 사용하지 않으시는 것을 추천드립니다.
   - 쿠키를 추출할 때 **본 프로그램이 아닌** 해당 **브라우저**에서 '로그인 상태 유지'가 체크된 상태로 SOOP에 로그인되어 있어야 합니다.
   '로그인 상태 유지'를 체크하지 않고 로그인할 경우, 녹화 시 비로그인 상태로 인식될 수 있습니다. 

### FEATURE

* `OPTION` | 브라우저 쿠키로 로그인 기능 추가 [#31](https://github.com/HO-Silverplate/multi_downloader/issues/31)

### BUGFIX

* `DASHBOARD` | 로그인/로그아웃 이후에도 세션이 갱신되지 않아 변화가 반영되지 않는 문제 

## 2025/05/11 - [v1.0.0](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v1.0.0)

### NOTE

1. 이제 녹화 중에도 설정을 변경할 수 있습니다.
   - 녹화 중인 스트리머를 삭제할 수는 없으며, 녹화 중에 선호 화질을 변경하면 다음 녹화부터 적용됩니다.
   - 파일 출력 옵션과 각종 타임아웃 값 변경 또한 이미 시작된 녹화에는 영향을 미치지 않습니다.
2. 이제 스트리머별로 하위 폴더를 생성하도록 설정할 수 있습니다. 설정할 경우 각 스트리머의 녹화본은 해당 스트리머의 폴더에만 저장됩니다.
3. 목록 관리에서 스트리머의 순서를 변경할 수 있습니다.
4. 대시보드에서 방송의 썸네일을 확인할 수 있습니다.
5. 자동 업데이트 기능을 추가했습니다. 업데이트 알림은 비활성화할 수 있지만, "긴급 업데이트"는 항상 알림을 띄웁니다.
6. 비밀번호가 설정된 방송이 일반 방송중 상태로 인식되는 문제를 해결했습니다.
   - 비밀번호가 설정된 방송 녹화는 아직 지원하지 않고 있습니다.

### FEATURE

* `OPTION` | 설정 탭 진입 제한 해제
* `OPTION` | 스트리머 위젯 순서 변경 기능 추가
* `OPTION` | 스트리머별 폴더 생성 기능 추가
* `DASHBOARD` | 썸네일 추가
* `APP` | 자동 업데이터 추가

### BUGFIX

* `DASHBOARD` | 비밀번호 설정 방송 코드 부여(-100)

---

## 2025/05/04 - [v0.3.7](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.7)

### NOTE

1. 이제 스트리머별로 선호 녹화 화질을 지정할 수 있습니다. 녹화가 시작된 이후에는 변경할 수 없으니 신중히 지정하세요.
2. 로그인이 필요한 스트림을 지속적으로 녹화하려 시도하던 오류를 해결했습니다.

### FEATURE

* `OPTION` | 스트리머 목록 관리에서 스트림 화질 지정 기능 추가
* `DASHBOARD` | 방송 상태 라벨에 녹화 중인 화질 표시

### BUGFIX

* `DASHBOARD` | 상태 코드 -6 처리 누락 확인 및 추가

---

## 2025/05/01 - [v0.3.6](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.6)

### NOTE

1. 설정 파일에 문제가 발생할 시 설정을 초기화합니다.

### BUGFIX

* `CONFIG` | 최초 실행 시 컨픽에 문제가 발생하면 제거 후 다시 덤프하도록 처리

---

## [STABLE] 2025/03/26 - [v0.3.5](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.5)

### NOTE 

1. 방송 상태 체크 쓰레드가 제대로 갱신되지 않는 문제를 해결했습니다.
2. VOD 검색 시에 인덱스가 갱신되지 않고 누적되는 문제를 해결했습니다.

### BUGFIX

* `DASHBOARD` | 체크 쓰레드의 생성 순서를 변경하여 설정 미반영 문제 해결
* `VOD` | VOD 인덱스 갱신 반영


---

## [LATEST] 2025/03/15 - [v0.3.4](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.4)

### NOTE 

1. 방송 상태 체크 쓰레드가 제대로 활성화되지 않는 문제를 해결했습니다.

### BUGFIX
* `DASHBOARD` | v0.3.2의 변경점 미반영된 것으로 확인됨, Merge하여 해결.
* `APP` | 로그 방식 변경, 불필요한 로그 메시지 제거

---

## 2025/03/15 - [v0.3.3b](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.3b)

### NOTE

1. 스트리머 방송 상태 정보를 잘못 인식하는 문제를 해결했습니다. (v0.3.3만 해당, 이전 버전은 해당 없음)

### BUGFIX

* `DASHBOARD` | 조건문 오기로 인한 방송 녹화 불가 문제

---

## 2025/03/13 - [v0.3.3](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.3)

### NOTE

1. 설정 변경사항이 UI에 정상적으로 반영되지 않는 문제를 해결했습니다.
2. 불필요한 리소스를 정리했습니다. 

### BUGFIX

* `OPTION` | .ts형식 출력 옵션, 에러 시 자동 중단 설정값이 UI에 미반영되는 문제

---

## 2025/01/28 - [v0.3.2](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.2)

### NOTE

1. 시스템 트레이로 최소화한 이후 프로그램이 더 이상 체크를 하지 않는 문제를 해결했습니다.
2. 이제 설정창에서 닫기 버튼을 눌러 시스템 트레이로 최소화하면 자동으로 변경된 설정을 저장하고 대쉬보드 탭으로 이동합니다.

### BUGFIX

* `APP` | 설정 탭에서 다른 탭으로 이동할 때 프로그램이 체크를 멈추는 문제

> *눈칫밥*

---

## 2025/01/15 - [v0.3.1](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.1)

### NOTE

1. 대시보드에서 스트리머 상태를 갱신 중일 때 프로그램이 잠시 멈추는 문제를 해결했습니다.
2. 설정에서 저장 버튼을 일일히 누를 필요 없이 자동저장되도록 변경하였습니다.
3. 설정을 초기값으로 되돌릴 수 있는 버튼을 추가했습니다.

### FEATURE

* `OPTION` | 설정이 자동저장되도록 변경(저장 시점: 옵션 탭으로부터 이동/앱 종료)

### BUGFIX

* `DASHBOARD` | 스트리머 체크가 동기식으로 진행되어 UI스레드를 멈추는 문제 [#26](https://github.com/HO-Silverplate/multi_downloader/issues/26)
* `OPTION`| 스트리머 목록 관리 메뉴에서 삭제된 스트리머가 이미 등록되었다고 표시되는 문제
* `APP` | 경고 다이얼로그의 메뉴힌트가 제대로 표시되지 않는 문제 [#1](https://github.com/HO-Silverplate/multi_downloader/issues/1)

> *박카스 디카페, 펩시제로 제로카페인 라임맛, 두찜 까만찜닭*

---

## 2025/01/10 - [v0.3.0](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.3.0)

### NOTE

1. SOOP VOD와 다시보기를 검색 및 다운로드할 수 있는 VOD탭을 추가했습니다.
3. 이제 2차 비밀번호 로그인이 가능해졌습니다.
2. 설정의 스트리머 목록에서 스트리머 닉네임을 같이 표출하도록 변경했습니다.

### FEATURE

* `VOD` | VOD 다운로더 탭 추가 [#21](https://github.com/HO-Silverplate/multi_downloader/issues/21)
* `OPTION` | 2차 비밀번호 로그인 추가
* `OPTION` | 스트리머 목록 관리에서 스트리머 닉네임 확인 가능

> *삼시세끼 잘 챙겨먹음*

---

## 2024/12/22 - [v0.2.6g beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.2.6g-beta)

### NOTE

1. 오류 처리를 개선했습니다. 이제 스트림 종료를 더 일관적으로 처리합니다.
2. 리먹스 스레드를 수정했습니다. 이제 작업 중단을 요청하면 진행중이던 작업 파일을 덮어쓰지 않고 제거합니다.
3. 리먹스가 진행중임을 확인할 수 있도록 버튼 상태를 변경하도록 개선하였습니다.

4. 더욱 편리한 사용을 위해 "시스템 트레이로 최소화"와 "부팅 시 자동 시작" 옵션을 추가했습니다.
    * 시스템 트레이로 최소화:  
        활성화하면 창을 닫을 때 종료되는 대신 시스템 트레이로 최소화됩니다.  
        시스템 트레이 아이콘을 더블클릭하면 프로그램 윈도우를 다시 표시하고, 우클릭하여 완전히 종료할 수 있습니다.  

        아이콘에 표시되는 숫자를 통해 현재 몇 명의 방송을 녹화 중인지 간편하게 확인할 수 있습니다. 8명 이상은 "+"로 표시됩니다.

    * 부팅 시 자동 시작:  
        활성화하면 윈도우의 시작 프로그램에 다중녹화기를 등록합니다.  
        시작 프로그램에 등록된 후에는 컴퓨터를 부팅할 때마다 자동으로 다중녹화기를 실행합니다.
5. 모든 스트리머들의 녹화 여부를 일괄적으로 체크할 수 있는 버튼을 추가했습니다.

* 0.2.6 -> 0.2.6b : 부팅 시 자동 시작될 경우 영상의 저장 위치가 임시 폴더로 지정되는 문제를 고쳤습니다.
* 0.2.6b -> 0.2.6c : 파일 이름 길이의 제한을 늘렸습니다.
* 0.2.6 -> 0.2.6d/e : 빌드의 VLC 누락 문제를 해결했습니다. (d: 빌드에 VLC 플러그인 포함, e: VLC 의존성 제거)
* 0.2.6 -> 0.2.6f : 설정 적용 이후 녹화가 시작되지 않는 문제를 수정했습니다.
* 0.2.6 -> 0.2.6g : 저장 경로 설정이 항상 초기화되는 문제를 수정했습니다.

### BUGFIX

* `DOWNLOAD` | 오류가 발생했을 때 스트림이 제대로 종료되지 않던 문제 [#25](https://github.com/HO-Silverplate/multi_downloader/issues/25)
* `REMUX` | 리먹스를 중간에 중단하면 FFmpeg가 강제로 종료되어 파일이 깨지던 문제 [#24](https://github.com/HO-Silverplate/multi_downloader/issues/24)

### FEATURE

* `DOWNLOAD` | "전체 체크" 버튼 추가
* `OPTION` | "시스템 트레이로 최소화" 옵션 및 시스템 트레이 아이콘 추가 [#20](https://github.com/HO-Silverplate/multi_downloader/issues/20)
* `OPTION` | "부팅 시 자동 시작" 옵션 추가 [#20](https://github.com/HO-Silverplate/multi_downloader/issues/20)
* `REMUX` | 리먹스 실행 상태에 따라 버튼의 상태 변경 [#22](https://github.com/HO-Silverplate/multi_downloader/issues/22)

> *초콜릿 청크 쿠키, 테라 큰캔, 기린 이치방 시보리 작은캔, 칙촉, 참쌀선과, 박카스 디카페, 에이스 씬에스프레소, 일드프랑스 미니브리치즈*

---

## 2024/12/08 - [v0.2.5 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.2.5-beta)

### BUGFIX

* `CONFIG` | 기본 컨픽의 기본 출력 경로가 잘못 기입되어 바로 출력할 수 없던 문제 [#19](https://github.com/HO-Silverplate/multi_downloader/issues/19)

* `APP` | 탭바 위에서 스크롤하면 필수 설정을 완료하지 않아도 다른 탭으로 이동할 수 있던 문제 [#2](https://github.com/HO-Silverplate/multi_downloader/issues/2)

> *햇반, 계란말이, 고추장아찌, 깍두기, 깻잎지*

---

## 2024/11/25 - [v0.2.4 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.2.4-beta)

### BUGFIX

* `CONFIG` | 계정 정보가 정상적으로 컨픽에 등록되지 않던 문제 [#18](https://github.com/HO-Silverplate/multi_downloader/issues/18)

### FEATURE

* `OPTION` | 이제 계정 정보를 SOOP 로그인에 이용하고, 컨픽에는 기록하지 않음.
* `AUTH` | 이제 단일 세션으로 모든 작업을 실행.
* `AUTH` | 이제 세션의 쿠키 정보를 데이터 폴더에 저장합니다.

> *육개장 큰컵, 수제 샌드위치, 유부초밥, 오븐스파게티, 코카콜라 뚱캔, 제육볶음*

---

## 2024/11/21 - [v0.2.3 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.2.3-beta)

### BUGFIX

* `DOWNLOAD` | 스트리머가 방송을 종료했을 때 녹화가 정상적으로 종료되지 않던 문제 [#17](https://github.com/HO-Silverplate/multi_downloader/issues/17)
* `DOWNLOAD` | 네트워크 문제가 발생했을 때 대기하지 않고 강제로 종료되던 문제 [#17](https://github.com/HO-Silverplate/multi_downloader/issues/17)
* `OPTION` | 오류가 발생하면 자동으로 해당 스트리머의 체크 여부를 비활성화할 수 있는 옵션 추가

> *신라면(봉), 멸균우유*

---

## 2024/11/19 - [v0.2.2 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.2.2-beta)

### FEATURE

* `OPTION` | 자동 REMUX 옵션 추가

---

## 2024/11/17 - [v0.2.1 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.2.1-beta)

### BUGFIX

* `AUTH` | 자동 로그인이 체크되어 있어도 로그인하지 않는 문제 [#9](https://github.com/HO-Silverplate/multi_downloader/issues/9)

### FEATURE

* `REMUX` | 출력된 영상의 메타데이터를 정리하고 컨테이너를 변경하는 REMUXER 탭 추가

>*후랑크, 아이스티, 도미노피자*

---

## 2024/11/17 - [v0.2.0 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.2.0-beta)

### FEATURE

* `REMUX` | 영상 종료 시 자동으로 메타데이터 정리 [#3](https://github.com/HO-Silverplate/multi_downloader/issues/3)

> *햇반, 갓김치, 불고기, 토마토카레참치, 컵커피, 싸이버거세트, 프레첼, 감자칩*  
*핫식스 더 킹, 테라(작은캔), 편의점 닭강정, 훈제란*  

---

## 2024/11/16 - [v0.1.1 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.1.1-beta)

### FEATURE

* `OPTION` | 파일명 형식 커스터마이징 옵션 추가 [#8](https://github.com/HO-Silverplate/multi_downloader/issues/8)

> *조기구이, 소고기뭇국*

---

## 2024/11/15 - [v0.1.0 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.1.0-beta)

### FEATURE

* `DOWNLOAD` | .ts 형식 단일파일, 또는 세그먼트 폴더 출력 기능 추가 [#7](https://github.com/HO-Silverplate/multi_downloader/issues/7)
* `OPTION` | 출력파일 형식 옵션 추가 [#7](https://github.com/HO-Silverplate/multi_downloader/issues/7)

>*홈런볼*

---

## 2024/11/15 - [v0.0.2 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.0.2-beta)

### BUGFIX

* `OPTION` | 파일 접근 권한 부족으로 FFmpeg를 인식하지 못하던 문제 [#6](https://github.com/HO-Silverplate/multi_downloader/issues/6)

>*참치마요 김밥, 아이스티*

---

## 2024/11/14 - [v0.0.1 beta](https://github.com/HO-Silverplate/multi_downloader/releases/tag/v0.1.1-beta)

### INITIAL RELEASE
