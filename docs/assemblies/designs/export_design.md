---
layout: default
title: 디자인 내보내기
nav_order: 10
permalink: /docs/assemblies/designs/export_design
parent: 디자인
grand_parent: 조립품
---
디자인 내보내기
========

디자인을 Fusion 360에서 다른 CAD 응용프로그램 형식으로 내보내거나 기본 Fusion 360 파일로 내보내는 방법을 알아봅니다.

1.  내보낼 디자인을 엽니다.
    
2.  **응용프로그램** 막대에서 **파일** ![파일 아이콘](https://help.autodesk.com/cloudhelp/KOR/Fusion-Assemble/images/icon/common/file.png) **\> 내보내기**를 클릭합니다.
    
    **내보내기** 대화상자가 표시됩니다.
    
3.  **내보내기** 대화상자에서 내보낸 디자인의 **이름**을 입력합니다.
    
4.  내보낼 파일의 **유형**을 선택합니다.
    
    *   Fusion 360 파일(`*.f3d`, `*.f3z`)
    *   적층 제조를 위해 디자인된 3D 제조 형식 파일(`*.3mf`) XML 기반 파일입니다. 정점, 삼각형 면, 단위, 색상 및 텍스처를 포함하여 3D 곡면의 특성을 설명합니다.
    *   Inventor 파일(`*.ipt`, `*.iam`)
    *   AutoCAD DWG 파일(`*.dwg`)
    *   DXF 파일(`*.dxf`) Drawing Interchange Format의 약어로 다른 CAD 시스템에서 읽을 수 있는 도면 정보가 포함된 문자 파일입니다.
    *   FBX 파일(`*.fbx`) 3ds Max, Maya, MotionBuilder, Mudbox 및 기타 특성과 타사 소프트웨어 간에 충실도 높은 데이터 교환을 용이하게 하는 형식입니다.
    *   IGES 파일(`*.igs`, `*.iges`) Initial Graphics Exchange Specification의 약어로 CAD/CAM 시스템 간의 정보 교환과 디지털 표현을 위한 ANSI 표준 형식입니다.
    *   LMV 파일(`*.svf`): 간단한 벡터 형식(큰 모형 뷰어용).
    *   OBJ 파일(`*.obj`) 대략적인 형상 쉐이프를 만드는 꼭지점 위치, 꼭지점 법선, 텍스처 좌표 꼭지점 및 다각형 면(일반적으로 메쉬)을 사용하여 형상을 나타내는 간단한 데이터 형식입니다.
    *   SAT 파일(`*.sat`) ASCII 파일에 저장된 형상 객체입니다.
    *   SketchUp 파일(`*.skp`)
    *   SMT 파일(`*.smt`) ASM(Autodesk Shape Manager) 파일과 연관된 내보내기 중립 파일 형식입니다.
    *   SPD 파일(`*.spd`) Z형과 연관된 파일 유형입니다.
    *   STEP 파일(`*.stp`, `*.step`) 현재 데이터 변환 표준의 일부 제한을 극복하기 위해 개발된 국제 3D 파일 교환 형식입니다.
    *   STL 파일(`*.stl`) 스테레오 리소그래피를 위한 솔리드, 영역, 부품 및 부분조립품의 출력 파일입니다. STL 형식은 전체 쉐이프를 대략적으로 묘사한 여러 개의 플랫 면으로 축소시킵니다.
    *   USD 파일(`*.usdz`) AR(증강 현실)에서 3D 객체를 보는 데 사용되는 범용 장면 설명 파일입니다.
5.  파일을 저장할 **위치**를 지정합니다.
    
6.  **내보내기**를 클릭합니다.
    
7.  파일을 저장할 **위치**를 지정합니다.
    
8.  **내보내기**를 클릭합니다.
    

디자인을 선택한 파일 형식으로 내보내고 지정한 위치에 저장합니다.

팁
-

*   내보낸 디자인은 원래 Fusion 360 디자인과의 연관성을 유지하지 않습니다.
*   외부 참조(`*.f3z`)가 포함된 Fusion 360 디자인 파일을 Fusion 360 디자인 파일(`*.f3d`)로 내보낼 수 없습니다. `*.f3z` 파일을 비롯한 다른 CAD 파일 형식으로만 내보낼 수 있습니다.
*   USDz 파일의 경우 다음과 같은 용도로 ASCII 영어 문자를 사용해야 합니다.
    *   경로
    *   파일 이름
    *   시스템 사용자 이름
    *   Fusion 360 설치 경로
*   USDz 파일의 경우 지원되지 않는 모양은 **강철 새틴** 모양으로 대체됩니다. 예를 들어 3D 목재 모양입니다.

![usdz AR 이미지](https://help.autodesk.com/cloudhelp/KOR/Fusion-Assemble/images/example/usd-ar-image.png)