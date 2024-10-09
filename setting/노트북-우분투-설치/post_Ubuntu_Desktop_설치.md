<!-- title: Ubuntu 24.04 Desktop Download 우분투 설치하기 가이드 -->

# Ubuntu 24.04 Desktop Download 우분투 설치하기 가이드

이번 달에 새로 노트북을 샀습니다. CPU 가 고성능이니 너무 좋은 것 같습니다.
<br/>
3년간 열심히 사용하던 노트북에 우분투를 설치하여 사용해보고자 합니다.
<br/>
2024년 올해 새로 나온 Ubuntu 24.04 버전을 설치한 기록을 공유합니다.

<br/>
<br/>


> 목차
>
> 1. Ubuntu 24.04 설치 이미지 다운로드
>
> 2. 부팅 USB 만들기
>
> 3. Ubuntu Desktop 24.04 설치

<br/>

## 1. Ubuntu 24.04 설치 이미지 다운로드

![설치이미지-다운로드-1](./images/설치이미지-다운로드-1.webp)

> Ubuntu Desktop 설치 이미지를 다운로드 받습니다.
>
> Ubuntu Desktop 24.04.01 LTS 다운로드 공식 홈페이지
>
> [https://ubuntu.com/download/desktop](https://ubuntu.com/download/desktop)

<br/>
<br/>
<br/>
<br/>
<br/>

## 2. 부팅 USB 만들기

![myUSB](./images/1.webp)

> 다운로드 받은 우분투 이미지를 이용하여 부팅 USB를 만들어봅시다.
>
> USB를 준비해주세요. USB 용량은 8 GB 면 충분합니다.
>
> Rufus라는 툴을 이용해서 부팅용 USB를 편리하게 만들 수 있습니다.
>
> [https://rufus.ie/ko/](https://rufus.ie/ko/)
>
> 이전에 다운로드 받은 우분투 데스크탑 설치 이미지를 이용하여 부팅 USB 를 만들 수 있습니다.

<br/>
<br/>
<br/>
<br/>
<br/>

## 3. Ubuntu Desktop 24.04 설치

![restart](./images/2.webp)

![bootMenu](./images/3.webp)

> 우분투를 설치할 노트북에 우분투 부팅 USB를 연결합니다.
>
> 다시 시작으로 재부팅시켜줍니다.
>
> LG 노트북은 부팅시 F10 을 눌러서 Boot 순서를 조정해줄 수 있습니다.
>
> USB Device 로 부팅하는 옵션을 선택합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![ubuntu](./images/4.webp)

> 잠시 기다리면 Ubuntu 부팅이 시작됩니다.
>
> Try or Install Ubuntu 를 선택합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![selectLanguage](./images/5.webp)

> 언어를 선택합니다. 저는 English 를 선택했습니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-accessibility](./images/6.webp)

> 접근성 설정 메뉴입니다.
>
> 설치 후에도 설정할 수 있으니 다음으로 넘어갑니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-keyboard](./images/7.webp)

> 키보드 설정입니다. 화면에서 간단하게 타이핑하면서 테스트도 가능합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-internet-1](./images/8.webp)
![step-internet-2](./images/9.webp)
![step-internet-3](./images/10.webp)

> 인터넷 연결 설정 단계입니다.
>
> 저는 간단하게 와이파이를 연결했습니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-install](./images/11.webp)

> 저는 기존 윈도우 운영체제를 대체하여 우분투를 설치하겠습니다.
>
> Install Ubuntu 를 선택합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-install-method](./images/12.webp)

> Interactive Installation 을 선택합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-install-method-2](./images/13.webp)

> 기본으로 Default Selection 을 선택합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-install-additional](./images/14.webp)

> 저는 추가 구성 요소를 같이 설치하겠습니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-install-manual](./images/15.webp)

> 저는 기존에 윈도우 노트북이었기 때문에 기존 디스크의 파티션도 정리해야합니다.
>
> Manual Installation 을 선택합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-install-manual-partitioning-1](./images/17.webp)
![step-install-manual-partitioning-2](./images/18.webp)
![step-install-manual-partitioning-3](./images/19.webp)
![step-install-manual-partitioning-4](./images/20.webp)
![step-install-manual-partitioning-5](./images/23.webp)

> 디스크의 파티션을 정리하고 우분투 운영체제를 어떤 디스크에 설치할지 결정하는 단계입니다.
>
> 1. 맨 마지막 USB 디스크는 제외하고 모든 영역에서 '-' 버튼을 클릭하여 초기화해줍니다.
>
> 2. 왼쪽하단 드롭다운 버튼으로 Boot loader 를 설치할 디스크를 선택합니다.
>
> 3. 메인 디스크를 Ext4 형식으로 '/' 경로로 마운트 합니다.
>
> 4. 추가 서브 디스크가 있다면, 메인 디스크와 마운트 경로를 다르게 하여 마운트합니다. 저는 /mnt/sdd-1 으로 마운트 했습니다.
>
> 5. 마지막으로 파티션 설정을 확인 후, 다음으로 넘어갑니다.
>

<br/>
<br/>
<br/>
<br/>
<br/>

![step-create-user](./images/24.webp)

> 사용자 계정을 비밀번호와 함께 만들어서 설정합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-select-timezone](./images/26.webp)

> Timezone을 설정하는 단계입니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-review](./images/27.webp)

> 마지막으로 설치 옵션을 확인합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-installing](./images/28.webp)

![step-install-finish](./images/29.webp)

> 설치를 진행하고 설치가 완료되면 다시 시작합니다.

<br/>
<br/>
<br/>
<br/>
<br/>

![step-complete](./images/30.webp)

> 다시 시작 진행 중 연결된 부팅 USB 를 분리해달라고합니다.
>
> 노트북에서 부팅 USB 를 분리후 엔터를 입력합니다.
>
> 조금 기다리면 우분투 데스크탑 바탕화면이 보입니다.
>
> 이렇게 설치를 모두 완료했습니다.
>
> 설치 과정은 윈도우와 비슷했던 것 같고, UI도 보기 좋은데요! 
>
> 저는 우분투를 사용하면서 공부도 하고 
>
> 외출할때는 우분투가 설치된 가벼운 노트북을 들고 다닐 것 같네요
>
> 감사합니다.

