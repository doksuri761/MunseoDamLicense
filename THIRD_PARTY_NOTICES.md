# 문서담 제3자 소프트웨어 고지

문서담(MunseoDam)은 아래의 오픈소스 및 제3자 소프트웨어를 사용합니다. 문서담 자체에는 [문서담 독점 소프트웨어 사용권 계약서](./LICENSE.txt)가 적용되지만, 제3자 구성요소에는 각 권리자가 정한 라이선스가 독립적으로 적용됩니다. 문서담의 독점 사용권은 제3자 라이선스가 부여한 권리를 제한하거나 변경하지 않습니다.

## 주요 직접 의존성

| 구성요소 | 라이선스 | 프로젝트 |
|---|---|---|
| PySide6 / Qt for Python / Shiboken | LGPL-3.0-only, GPL-2.0-only, GPL-3.0-only 또는 별도 Qt 상업용 라이선스 중 적용 가능한 조건 | [Qt for Python](https://doc.qt.io/qtforpython-6/licenses.html) |
| HTTPX | BSD-3-Clause | [encode/httpx](https://github.com/encode/httpx) |
| Chroma | Apache-2.0 | [chroma-core/chroma](https://github.com/chroma-core/chroma) |
| python-docx | MIT | [python-openxml/python-docx](https://github.com/python-openxml/python-docx) |
| pypdf | BSD-3-Clause | [py-pdf/pypdf](https://github.com/py-pdf/pypdf) |
| python-pptx | MIT | [scanny/python-pptx](https://github.com/scanny/python-pptx) |
| openpyxl | MIT | [openpyxl](https://foss.heptapod.net/openpyxl/openpyxl) |
| keyring | MIT | [jaraco/keyring](https://github.com/jaraco/keyring) |
| charset-normalizer | MIT | [jawah/charset_normalizer](https://github.com/jawah/charset_normalizer) |

## Qt / PySide6 LGPL 고지

문서담 배포물은 PySide6를 통해 Qt 라이브러리를 동적으로 불러옵니다. 배포자가 별도의 Qt 상업용 라이선스를 적용하지 않고 LGPL-3.0 조건을 선택하는 경우 다음 고지와 조건이 적용됩니다.

- [GNU GPL 버전 3 원문](./docs/third-party/GPL-3.0.txt)
- [GNU LGPL 버전 3 원문](./docs/third-party/LGPL-3.0.txt)
- Qt for Python 소스: [pyside-setup](https://code.qt.io/cgit/pyside/pyside-setup.git/)
- Qt 소스: [Qt Project repositories](https://code.qt.io/cgit/qt/)

LGPL이 보장하는 범위에서 사용자는 LGPL 적용 라이브러리를 교체·수정·재링크하고, 그러한 수정을 디버깅하기 위해 필요한 범위에서 역공학할 수 있습니다. 문서담 독점 사용권 계약의 제한은 이 권리를 제한하지 않습니다. 호환되지 않는 라이브러리로 교체한 결과까지 문서담의 정상 작동이나 지원이 보장되는 것은 아닙니다.

해당 릴리스에 포함된 Qt/PySide6의 정확한 대응 소스가 필요한 사용자는 소프트웨어를 제공받은 배포 담당 경로로 서면 요청할 수 있습니다. 사용허락자는 해당 릴리스 배포일부터 최소 3년 동안, 매체·전송에 실제로 드는 합리적인 비용 이하로 적용 LGPL 조건에 따른 대응 소스와 필요한 설치 정보를 제공합니다.

## 전이 의존성과 원문 라이선스

위 표는 문서담이 직접 선언한 주요 런타임 의존성을 요약한 것입니다. 실제 배포물에는 이 구성요소들이 사용하는 전이 의존성과 네이티브 라이브러리가 추가로 포함될 수 있습니다. 각 배포물에 포함된 패키지 메타데이터와 라이선스 파일이 해당 버전의 정확한 고지와 조건을 구성합니다.

배포 담당자는 릴리스마다 실제 번들 목록을 확인하고 다음 사항을 보존해야 합니다.

- 각 구성요소의 저작권 고지와 라이선스 원문
- NOTICE 또는 COPYING 파일이 있는 경우 해당 파일
- 소스 제공, 교체·재링크 허용 또는 그 밖의 조건이 적용되는 경우 이를 충족하는 안내
- 수정한 제3자 구성요소가 있는 경우 변경 사항과 적용 라이선스가 요구하는 고지

특히 PySide6와 Qt 라이브러리를 독점 소프트웨어와 함께 배포할 때에는 보유한 Qt 상업용 라이선스를 따르거나, 선택한 LGPL/GPL 조건을 충족해야 합니다. 라이선스 선택과 배포 방식은 릴리스 전에 별도 검토해야 합니다.

제3자 라이선스의 정확한 내용은 각 프로젝트가 배포한 원문이 우선합니다. 이 문서는 법률 자문이나 모든 전이 의존성에 대한 완전한 적합성 판정을 대신하지 않습니다.
