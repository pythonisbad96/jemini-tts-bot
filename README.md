<h1>🎙️ 디스코드 잼민이 TTS 봇</h1>

<p>텍스트 채팅을 자동으로 감지하여 잼민이 스타일로 읽어주는 초경량 디스코드 TTS 봇입니다.</p>

<h2>🚀 주요 기능</h2>
<ul>
  <li>채팅 입력 자동 감지 및 실시간 음성 출력</li>
  <li>잼민이 스타일 음성 지원 (VITS 기반)</li>
  <li>명령어 없이 UI 기반 음성 송출</li>
  <li>라이트한 TTS 모델로 빠른 반응 속도</li>
</ul>

<details>
  <summary>📁 폴더 구조</summary>
  <pre><code>.
├── bot.py
├── tts/
│   ├── generate_tts.py  # 잼민이 스타일 TTS 생성 함수
│   └── model/           # 사전 학습된 VITS 모델 (또는 edge-tts 사용 시 해당 없음)
├── audio/
│   └── output.wav       # 생성된 음성 임시 저장 파일
├── .env                 # 디스코드 토큰 저장
└── requirements.txt     # 필요한 패키지 목록
</code></pre>
</details>

<details>
  <summary>⚙️ 실행 방법</summary>
  <ol>
    <li><code>git clone https://github.com/사용자명/tts-discord-bot.git</code></li>
    <li><code>cd tts-discord-bot</code></li>
    <li><code>pip install -r requirements.txt</code></li>
    <li><code>.env</code> 파일에 디스코드 토큰 추가</li>
    <li><code>python bot.py</code> 실행</li>
  </ol>
</details>

<details>
  <summary>🔊 TTS 기법 정리</summary>
  <ul>
    <li><strong>모델:</strong> VITS 기반 경량 음성 합성</li>
    <li><strong>보이스:</strong> Bark "ko_speaker_4" 스타일을 TTS로 이식</li>
    <li><strong>전처리:</strong> Whisper 또는 SpeechRecognition으로 명령어 없이 채팅 감지</li>
    <li><strong>재생 방식:</strong> <code>discord.FFmpegPCMAudio</code>로 음성 출력</li>
  </ul>
</details>

<hr>
<p>🛠 제작자: <strong>HeeJune Kim</strong> | 📅 최신 업데이트: 2025년 6월</p>
