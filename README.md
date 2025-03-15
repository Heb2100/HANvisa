<div style="text-align: center;">
    <h1 style="font-size: 24px; font-weight: bold;">HANvisa</h1>
    <h2 style="font-size: 20px; font-weight: bold;">1. 소개 및 수행업무</h2>
    <p style="font-size: 18px;">HANvisa: 외국인 비자 발급 자동화 서비스</p>
    <p style="font-size: 16px;">HANvisa는 외국인 비자 발급 절차를 간소화하고 비용을 절감하는 서비스를 제공합니다.</p>
    <p style="font-size: 16px;">이 제품은 사용자 앱과 관리 페이지로 구성되어 있으며, 사용자의 상황에 맞춰 LLM(대형 언어 모델)을 활용하여 소통합니다.</p>
    <p style="font-size: 16px;">이 프로젝트는 카이스트 예비창업패키지와 정주영 창업대회에 출전한 제품으로, 비자 발급이 복잡하고 비용이 높은 문제를 해결하려고 합니다.</p>
    <div style="display: flex; justify-content: center; gap: 10px;">
        <img src="https://github.com/user-attachments/assets/b2b68e17-fa7d-4134-8628-208b93d875f5" 
             alt="Image 1" style="width: 35%;">
        <img src="https://github.com/user-attachments/assets/b33dba8e-22bf-4f70-bba7-7854a674568d" 
             alt="Image 2" style="width: 35%;">
        <img src="https://github.com/user-attachments/assets/895b2dac-f249-48e2-bb28-fba9b4788f85" 
             alt="Image 3" style="width: 35%;">
        <img src="https://github.com/user-attachments/assets/95262dd7-a3c5-41db-af98-ac8b1c1d1308"
             alt="Image 4" style="width: 35%;">
    </div>
</div>

<div style="text-align: center; margin-top: 30px;">
    <h2 style="font-size: 20px; font-weight: bold;">2. 트러블슈팅</h2>
    <p style="font-size: 18px;"><li><b>비자 발급 프로세스에서 발생한 문제와 해결 방법</b></p></li>
    <p style="font-size: 16px;">비자 발급 과정에서 발생하는 지연 문제를 해결하기 위해 실시간 알림 시스템을 도입하였습니다.</p>
    <p style="font-size: 16px;">이로 인해 사용자들은 자신의 비자 상태를 빠르게 확인할 수 있게 되었습니다.</p>
    <p style="font-size: 16px;"><li><b>다양한 국가의 비자 규정 통합 문제</b></p></li>
    <p style="font-size: 16px;">각 국가의 비자 규정이 다르기 때문에, 이를 통합하여 일관된 데이터 처리 시스템을 구축하는 데 어려움이 있었습니다.</p>
    <p style="font-size: 16px;">이를 해결하기 위해 자동화된 데이터 수집과 처리 시스템을 개발하여 규정을 쉽게 관리할 수 있도록 했습니다.</p>    

    <p style="font-size: 16px;"><li><b>API를 사용한 정보 추출 문제</b></p></li>
    <p style="font-size: 16px;">비자 정보 추출 과정에서 다양한 국가의 비자 정보가 각각 다른 형식으로 제공되어, 이를 API를 통해 일관성 있게 처리하는 데 어려움이 있었습니다.</p>
    <p style="font-size: 16px;">이를 해결하기 위해 API에서 제공하는 데이터를 먼저 파싱하여 공통된 형식으로 변환한 후, 이를 처리하는 중간 레이어를 추가하여 데이터를 통합했습니다.</p>

    <p style="font-size: 16px;"><li><b>LLM Fine-Tuning 문제 해결</b></p></li>
    <p style="font-size: 16px;">비자 관련 정보를 다루는 데 있어, 기존의 언어 모델이 다소 일반적인 정보로만 작동하여 실제 사용자에게 맞춤형 정보를 제공하는 데 한계가 있었습니다.</p>
    <p style="font-size: 16px;">이를 해결하기 위해, <b>LLM Fine-Tuning</b>을 진행하여 비자 발급과 관련된 특정 도메인 지식에 맞춘 모델을 학습시켰습니다. 이를 통해 비자 규정, 문서 요구사항 등 특정 용어와 조건에 대해 더 정확한 정보를 제공할 수 있었습니다.</p>

    <p style="font-size: 16px;"><li><b>Flutter와 Spring 서버 동시에 배포 문제</b></p></li>
    <p style="font-size: 16px;">Flutter 앱과 Spring 서버를 동시에 배포하는 과정에서 발생한 문제는, 서버와 앱 간의 통신이 원활하지 않다는 점이었습니다. 특히, API 통신 시 CORS 문제가 발생하여 앱이 서버와 제대로 연결되지 않았습니다.</p>
    <p style="font-size: 16px;">이 문제를 해결하기 위해 <b>CORS</b> 설정을 Spring 서버에서 허용하도록 설정하고, 필요한 HTTP 메소드와 헤더를 명시적으로 추가하여 통신이 원활하게 이루어지도록 했습니다.</p>
    <p style="font-size: 16px;">또한, Flutter 앱이 모바일 환경에서 서버와의 연결을 유지하는 데 있어, <b>WebSocket</b>을 활용한 실시간 데이터 송수신 방식을 적용하여 사용자 경험을 개선했습니다.</p>
    <p style="font-size: 16px;">배포 후에는 AWS EC2 인스턴스를 사용하여 Spring 서버와 Flutter 앱의 빌드를 각각 분리하여 배포하고, 두 시스템 간의 API 통신을 안정적으로 유지할 수 있도록 했습니다.</p>
</div>

<div style="text-align: center; margin-top: 30px;">
    <h2 style="font-size: 20px; font-weight: bold;">3. 기술 스택</h2>
    <p style="font-size: 18px;">이 프로젝트에서 사용한 기술들</p>
    <ul style="font-size: 16px; list-style-position: inside; text-align: left; display: inline-block; text-align: left;">
        <li><b>프로그래밍 언어</b>: Dart (Flutter)</li>
        <li><b>백엔드 프레임워크</b>: Spring Framework</li>
        <li><b>데이터베이스</b>: MySQL</li>
        <li><b>서버 배포 환경</b>: Apache Tomcat</li>
        <li><b>언어 모델</b>: ChatGPT API</li>
    </ul>
</div>
