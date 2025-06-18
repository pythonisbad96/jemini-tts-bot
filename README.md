<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>잼민이 Discord TTS Bot</title>
  <style>
    body { font-family: "Pretendard", sans-serif; line-height: 1.6; padding: 2em; background-color: #f9f9f9; }
    h1 { color: #333; }
    code, pre { background: #eee; padding: 0.2em 0.4em; border-radius: 4px; font-size: 0.9em; }
    .section { margin-bottom: 2em; }
    ul { list-style-type: square; }
  </style>
</head>
<body>

  <h1>🗣️ 잼민이 Discord TTS Bot</h1>
  <p><strong>디스코드 채팅을 입력하면 실시간으로 잼민이 보이스로 읽어주는 봇</strong></p>

  <div class="section">
    <h2>📌 주요 기능</h2>
    <ul>
      <li>채팅 입력 시 자동 TTS 읽기 (명령어 없이)</li>
      <li>잼민이 스타일 보이스 (pitch, rate 조정)</li>
      <li>FFmpeg 기반 음성 재생</li>
      <li>slash 명령어 기반 봇 제어도 지원</li>
    </ul>
  </div>

  <div class="section">
    <h2>🛠 사용 기술</h2>
    <ul>
      <li><code>discord.py</code>: 디스코드 봇 기본 구조</li>
      <li><code>edge-tts</code>: Microsoft Neural TTS API 사용</li>
      <li><code>ffmpeg</code>: mp3 음성을 PCM으로 변환 및 재생</li>
      <li><code>dotenv</code>: 봇 토큰 환경변수로 관리</li>
    </ul>
  </div>

  <div class="section">
    <h2>🎛 잼민이 보이스 설정 예시</h2>
    <pre><code>
Communicate(
  text="안녕 나는 잼민이야~",
  voice="ko-KR-SunHiNeural",
  rate="+20%",
  pitch="+20%"
)
    </code></pre>
    <p><small>※ 높고 빠른 여성 목소리를 기반으로 설정</small></p>
  </div>

  <div class="section">
    <h2>📁 프로젝트 구조 예시</h2>
    <pre><code>
📁 jemini-tts-bot/
├── bot.py           # 봇 실행 메인
├── tts.py           # TTS 생성 함수
├── .env             # 디스코드 토큰 저장
├── requirements.txt # 라이브러리 목록
    </code></pre>
  </div>

  <div class="section">
    <h2>💡 향후 확장 예정</h2>
    <ul>
      <li>음성 인식 (Whisper) 기능 추가</li>
      <li>사용자별 voice profile 설정</li>
      <li>웹 UI (Streamlit 또는 Flask 기반)</li>
    </ul>
  </div>

  <footer>
    <hr />
    <p>© 2025 JaminiBot by HeeJune Kim | Powered by <code>Python</code> + <code>discord.py</code></p>
  </footer>

</body>
</html>
