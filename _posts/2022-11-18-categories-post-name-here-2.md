---
title: "[10일차] 프로그래밍 기초 & 리눅스 설치"
excerpt: "프로그래밍 기초를 익히고 리눅스 설치를 해보겠습니다"

categories:
  - Categories2
tags:
  - [Github, VirtualBox, Vagrant, Centos]

permalink: /categories2/post-name-here-2/

toc: true
toc_sticky: true

date: 2022-11-18
last_modified_at: 2022-11-19
---

## 🦥 수업 내용

* Application 아키텍처
<br>

* 가상화 / 하이퍼바이저 개념 익히기
<br>

* GIT
  - 버전 관리 시스템 / 프로그래밍 명령어 버전 관리
  - 형상관리 시스템 = CMS / SCM
  - 중앙관리 -> 분산관리
  - git fetch / git merge = git pull  
<br>

* 리눅스 설치
  - VirtualBox 설치 (https://www.virtualbox.org/)
  - Vagrant 설치 (_AMD64_) (https://developer.hashicorp.com/vagrant/downloads)
  - Centos 설치 (_Vagrant_) (https://www.centos.org/download/)
  - Vagrant cloud 설치 (https://app.vagrantup.com/boxes/search)
<br>

## 🦥 과제

* 하이퍼바이저란? (Hypervisor)
  - 하이퍼바이저는 가상화를 구현하기 위한 기반이 되는 기술로 가상 머신 (Virtual Machine, VM)을 생성하고 구동하는 소프트웨어이다.
  - 하이퍼바이저로 사용되는 주인장 하드웨어를 'Host', 리소스를 사용하는 여러 VM들을 'Guest'라고 부르기로 했다. 그러기로 했으니까 왜인지는 물어보지마라.
  - 아래의 그림과 같이 Type1 or Type2로 세팅을 할 수 있다. 외에도 'Container' 방식이 있음

![KakaoTalk_Photo_2022-11-19-20-02-09](https://user-images.githubusercontent.com/118426890/202847470-98a5b8b6-0e8f-475f-817b-93f09d5d6be4.jpeg)

* Type1
  - 'Native' or 'Bare Metal'형
  - 운영 체제가 프로그램을 제어하듯이 하이퍼바이저가 해당 하드웨어에서 직접 실행되며 하드웨어 제어가 가능

  장점)
  - 별도 Host OS가 없어서 오버헤드가 적고 직접 관리함으로 리소스 관리가 유연하다.

  단점)
  - 자체적으로 머신에 대한 관리 기능이 없어서 관리를 위한 컴퓨터나 콘솔이 필요하다.
  - Type2에 비해 성능이 향상된다.

  종류)  
    ▶ 젠(Xen)  
    ▶ KVM(Kernel-based Virtual Machine)  
    ▶ Citrix의 XenServer  
    ▶ IBM의 POWER 하이퍼바이저(PR/SM)  
    ▶ 스파크(SPARC)용 오라클(Oracle) VM 서버  
    ▶ x86용 오라클 VM 서버  
    ▶ 마이크로소프트 하이퍼(Hyper)-V  
    ▶ VM웨어의 ESX Server  
<br>

* Type2
    - 'Hosted'형
    - 일반 프로그램과 같이 호스트 운영 체제에서 실행된다.

  장점)
  - 가상의 하드웨어를 에뮬레이팅하기 때문에 호스트 운영체제에 크게 제약사항이 없다.

  단점)
  - OS위에 OS가 얹히는 방식이기 때문에 오버헤드가 클 수 있다.

  종류)  
    ▶ VM웨어 워크스테이션(Workstation)  
    ▶ VM웨어 플레이어(Player)  
    ▶ 버추얼박스(VirtualBox)  
    ▶ 맥용 패럴랠스 데스크톱(Parallels Desktop for Mac)  
    ▶ QEMU  
    
