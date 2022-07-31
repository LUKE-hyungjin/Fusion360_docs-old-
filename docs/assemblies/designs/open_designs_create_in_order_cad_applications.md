---
layout: default
title: 다른 CAD 응용프로그램에서 작성된 디자인 열기
nav_order: 16
permalink: /docs/assemblies/designs/open_designs_create_in_order_cad_applications
parent: 디자인
grand_parent: 조립품
---
다른 CAD 응용프로그램에서 작성된 디자인 열기
==========================

다른 CAD 응용프로그램에서 작성된 기존 디자인을 Fusion 360에서 여는 방법을 알아봅니다.

데이터 패널에서 원하는 항목을 두 번 클릭하여 AnyCAD 파일을 열거나 항목을 마우스 오른쪽 버튼으로 클릭하고 **열기**를 선택합니다.

원래 부품 파일이 업데이트되면 **응용프로그램** 막대 및 타임라인의 **오래된 버전** 아이콘 ![오래된 버전 아이콘](https://help.autodesk.com/cloudhelp/KOR/Fusion-Assemble/images/icon/browser/component-out-of-date.png)이 참조된 모형이 오래된 버전임을 나타냅니다. 필요한 경우 타임라인에서 마우스 오른쪽 버튼을 클릭하여 부품의 최신 버전을 가져오거나 원하는 버전을 선택합니다.

주: 원본 파일은 CAD 응용프로그램을 제작하여 생성되었으므로 Fusion 360에서 원본 파일을 직접 수정할 수 없습니다. 열려 있는 AnyCAD 파일에 대한 변경 사항을 저장하려면 해당 파일을 별도의 파일로 저장해야 합니다.

Fusion 360에서 AnyCAD 조립품을 처리하는 방법
--------------------------------

Fusion 360에서는 조립품 피쳐를 아직 지원하지 않습니다. 조립품 피쳐가 있는 조립품 형상이 올바르게 표시되도록 Fusion 360에서는 조립품 피쳐가 적용된 후 형상을 표시하기 위해 AnyCAD 상단 단계 조립품 아래에 구성요소 재지정을 작성합니다. 원래 구성요소는 동일한 계층구조를 유지하지만 시각적으로 숨겨집니다. 아래 예를 참고하십시오.

![anycad 조립품 브라우저 계층구조](https://help.autodesk.com/cloudhelp/KOR/Fusion-Assemble/images/browser/anycad-assemblies-browser-hierarchy.png)

주: 일부 기술적 한계로 인해 이 문제는 일시적으로 발생하며, 더 나은 솔루션이 곧 제공될 예정입니다. 현재 솔루션으로 인해 다음과 같은 알려진 문제가 발생할 수 있습니다.

*   부정확한 BOM/부품 리스트 정보 및 AnyCAD 조립품의 계층구조입니다. 숨겨진 원래 구성요소를 제거하고 재지정 구성요소를 원하는 위치로 이동하여 수동으로 수정할 수 있습니다.
    
*   재지정 구성요소는 원래 부품의 새 복제 대신 새 독립 구성요소로 처리됩니다. 즉, 이러한 구성요소는 이전에 원래 부품 구성요소에 적용된 다운스트림 작업을 상속하지 않습니다.
    

제작 CAD 응용프로그램에서 조립품 파일을 업데이트해야 하는 이유
------------------------------------

다음 대화상자가 표시되면 Fusion 360에서 데이터를 올바르게 처리할 수 있도록 제작 CAD 응용프로그램에서 조립품을 업데이트해야 함을 의미합니다.

![anycad 파일 업데이트 대화상자](https://help.autodesk.com/cloudhelp/KOR/Fusion-Assemble/images/dialog/anycad-update-file-dialog.png)

제작 CAD 응용프로그램에서 AnyCAD 조립품을 업데이트하는 방법
-------------------------------------

Fusion 360에서 AnyCAD 조립품의 최신 변경 사항을 처리하는 데 도움이 되도록 아래 지침에 따라 제작 CAD 응용프로그램에서 모형을 업데이트합니다.

### Inventor

Inventor .IPT 파일만 열고 편집하는 경우 부품 파일에 대한 모든 변경 사항을 저장한 후 해당 상단 조립품 .IAM 파일을 엽니다. 아래에 팝업 대화상자가 표시될 수 있습니다.

![anycad inventor 대화상자](https://help.autodesk.com/cloudhelp/KOR/Fusion-Assemble/images/dialog/anycad-inventor-dialog.png)

**예**를 선택하여 조립품을 업데이트하고 업데이트 후에 조립품 파일을 저장합니다.

조립품 파일을 열고 부품 파일을 내부에서 편집하는 경우 편집을 마친 후 변경 사항을 저장하고 **전부 예** 옵션을 선택한 다음 **확인**을 클릭하여 조립품을 업데이트합니다. 그런 다음 변경 사항을 .IPT 파일과 필요한 모든 상위 조립품 .IAM 파일에 저장합니다.

![anycad 저장 대화상자](https://help.autodesk.com/cloudhelp/KOR/Fusion-Assemble/images/dialog/anycad-save-dialog.png)

### SolidWorks

.SLDPRT 파일을 열고 편집만 할 경우 변경 사항을 .SLDPRT 파일에 저장한 후 상단 조립품 파일을 열면 문서를 재작성할지 여부를 확인하는 경고 메시지가 표시될 수 있습니다. **재작성**을 선택하여 부품 파일의 변경 사항을 처리합니다.

조립품에서 최신 부품 변경 사항이 제대로 재생성된 것을 확인한 후 저장 버튼을 클릭합니다. 이 시나리오에서는 SolidWorks에서 이 조립품의 참조된 파일(부품 및 부분조립품 포함)을 처리하는 방법을 묻는 메시지가 표시될 수 있습니다. 리스트에서 **모든 파일을 선택**하고 **모두 저장**을 클릭합니다.

### 기타 CAD 앱

다른 CAD 소프트웨어의 경우 유사한 로직을 따라 Fusion 360에서 최신 변경을 처리합니다. 부품 파일을 업데이트하는 경우 해당 조립품/부분조립품 파일을 동시에 업데이트해야 합니다. 그렇지 않으면 Fusion 360에서 최신 변경을 제대로 처리하지 못할 수 있습니다.

또한 수정된 모든 파일이 Desktop Connector에서 동기화되는지 확인합니다.