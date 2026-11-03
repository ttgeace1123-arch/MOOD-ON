[index.html](https://github.com/user-attachments/files/34319613/index.html)
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<style>:root{color-scheme:light;padding-block:env(safe-area-inset-top,0px) env(safe-area-inset-bottom,0px)}body{margin:0;font:14px system-ui}img{max-width:100%}[hidden]{display:none!important}</style>
<title>무드온 명동 Guest Guide</title>
<meta name="claude:viewport-fit-sides" content="cover">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@400;500;700&display=swap">
<style>
/* Layout: one narrow phone column. Language chips, three appliance tabs, then numbered step cards for the chosen appliance. */
:root {
  --bg: #eef3f7;
  --card: #ffffff;
  --ink: #14212e;
  --muted: #55677a;
  --line: #d3dee8;
  --accent: #1f5f8b;
  --accent-ink: #ffffff;
  --badge: #f0a83a;
  --badge-ink: #3a2500;
  --note: #dcebf5;
  --remote: #e4ebf1;
  --btn: #cbd8e3;
  --ok: #2e7d4f; --ok-bg: #e6f4ec; --ok-line: #b5dcc4;
  --no: #b3261e; --no-bg: #fdeaea; --no-line: #efbdb9;
  --font: "Noto Sans KR", system-ui, -apple-system, "Segoe UI", "Hiragino Sans", "Yu Gothic", "PingFang SC", "PingFang TC", "Microsoft YaHei", "Microsoft JhengHei", sans-serif;
}
@media (prefers-color-scheme: dark) {
  :root:not([data-theme="light"]) {
    --bg: #0f1a24; --card: #172633; --ink: #e8eef4; --muted: #9db0c2; --line: #2b3e50;
    --accent: #7fb8e3; --accent-ink: #0b1620; --badge: #f0a83a; --badge-ink: #2a1a00;
    --remote: #20344a; --btn: #2f475e; --note: #16303f;
    --ok: #6fcf97; --ok-bg: #14291e; --ok-line: #2c5a40;
    --no: #ff8f86; --no-bg: #2e1a1a; --no-line: #6b3a38;
    color-scheme: dark;
  }
}
:root[data-theme="dark"] {
  --bg: #0f1a24; --card: #172633; --ink: #e8eef4; --muted: #9db0c2; --line: #2b3e50;
  --accent: #7fb8e3; --accent-ink: #0b1620; --badge: #f0a83a; --badge-ink: #2a1a00;
  --remote: #20344a; --btn: #2f475e; --note: #16303f;
  --ok: #6fcf97; --ok-bg: #14291e; --ok-line: #2c5a40;
  --no: #ff8f86; --no-bg: #2e1a1a; --no-line: #6b3a38;
  color-scheme: dark;
}
body {
  background: var(--bg); color: var(--ink); font-family: var(--font); font-size: 16px; line-height: 1.6;
  padding-block: 20px 36px;
  padding-left: max(16px, env(safe-area-inset-left, 0px));
  padding-right: max(16px, env(safe-area-inset-right, 0px));
}
.wrap { max-width: 560px; margin: 0 auto; display: flex; flex-direction: column; gap: 16px; }
.brand { font-size: 13px; letter-spacing: .08em; text-transform: uppercase; color: var(--muted); font-weight: 500; }
.brand .sep { opacity: .6; }
.brand .shop { color: var(--ink); font-weight: 700; letter-spacing: 0; font-size: 15px; }
.langs { display: flex; flex-wrap: wrap; gap: 8px; }
.langs button {
  font: inherit; font-size: 14px; line-height: 1; padding: 9px 13px; min-height: 38px;
  border: 1px solid var(--line); background: var(--card); color: var(--ink); border-radius: 999px; cursor: pointer;
}
.langs button[aria-pressed="true"] { background: var(--ink); color: var(--bg); border-color: var(--ink); font-weight: 700; }
.tabs { display: flex; flex-wrap: wrap; gap: 1px; border: 1px solid var(--line); border-radius: 10px; overflow: hidden; background: var(--line); }
.tabs button {
  font: inherit; flex: 1 1 calc(33.333% - 1px); font-size: 14px; font-weight: 500; line-height: 1.25; padding: 10px 4px; min-height: 46px; min-width: 0; overflow-wrap: anywhere;
  background: var(--card); color: var(--ink); border: 0; cursor: pointer;
}
.tabs button:first-child { border-left: 0; }
.tabs button[aria-pressed="true"] { background: var(--accent); color: var(--accent-ink); font-weight: 700; }
button:focus-visible { outline: 3px solid var(--badge); outline-offset: -3px; }
h1 { font-size: 27px; line-height: 1.25; margin: 0; text-wrap: balance; }
h2.sec { font-size: 19px; margin: 8px 0 0; }
.sub { margin: -10px 0 0; color: var(--muted); letter-spacing: .06em; font-size: 14px; }
.card { background: var(--card); border: 1px solid var(--line); border-radius: 12px; padding: 14px 16px; min-width: 0; }
.card h3 { font-size: 16px; margin: 0; line-height: 1.4; }
.card p { margin: 2px 0 0; }
.list { display: flex; flex-direction: column; gap: 10px; }
.step { display: grid; grid-template-columns: 30px minmax(0, 1fr); gap: 12px; align-items: start; }
.n {
  flex: none; width: 28px; height: 28px; border-radius: 50%; background: var(--badge); color: var(--badge-ink);
  display: inline-grid; place-items: center; font-size: 14px; font-weight: 700; line-height: 1;
}
.n.alt { background: var(--accent); color: var(--accent-ink); }
.chip {
  display: inline-block; font-weight: 700; font-size: .92em; line-height: 1.35; padding: 0 7px;
  border: 1px solid var(--line); border-radius: 6px; background: var(--bg); white-space: nowrap;
}
.tv { display: flex; flex-wrap: wrap; gap: 18px; align-items: flex-start; justify-content: center; }
.remote { width: 170px; max-width: 100%; flex: none; }
.remote svg { display: block; width: 100%; height: auto; }
.legend { list-style: none; margin: 0; padding: 0; display: grid; gap: 14px; flex: 1 1 220px; min-width: 0; }
.legend li { display: grid; grid-template-columns: 28px minmax(0, 1fr); gap: 12px; align-items: start; }
.photo { display: block; width: 100%; height: auto; border-radius: 12px; border: 1px solid var(--line); }
.net { display: grid; grid-template-columns: 68px minmax(0, 1fr) auto; gap: 12px; align-items: center; }
.band { border-radius: 999px; padding: 6px 4px; text-align: center; font-weight: 700; font-size: 13px; background: var(--accent); color: var(--accent-ink); }
.band.pw { background: var(--badge); color: var(--badge-ink); }
.net .lab { display: block; font-size: 13px; color: var(--muted); line-height: 1.4; }
.net .val { display: block; font-family: ui-monospace, "SF Mono", Menlo, Consolas, monospace; font-size: 17px; font-weight: 700; word-break: break-all; user-select: all; }
.copy { font: inherit; font-size: 13px; padding: 7px 10px; min-height: 36px; border: 1px solid var(--line); background: var(--card); color: var(--ink); border-radius: 8px; cursor: pointer; }
.help { text-align: center; color: var(--muted); margin: 4px 0 0; }
.step.big { grid-template-columns: 64px minmax(0, 1fr); align-items: center; }
.ic svg { display: block; }
.drops { display: grid; gap: 16px; margin-top: 10px; }
.drop { margin: 0; display: grid; gap: 8px; }
.drop figcaption { align-items: center; font-weight: 500; }
.sw { width: 28px; height: 28px; border-radius: 50%; border: 1.5px solid var(--muted); margin-top: 1px; }
.sw.gen { background: linear-gradient(90deg, #ffffff 50%, #23272b 50%); }
.sw.food { background: #f2c230; }
.sw.rec { background: #ffffff; }
.rules { margin: 6px 0 0; padding-left: 20px; display: grid; gap: 6px; }
.quick { background: var(--note); border-color: transparent; }
.kv { display: grid; gap: 10px; }
.kv > div { display: grid; grid-template-columns: minmax(84px, 30%) minmax(0, 1fr); gap: 10px; }
.kv .k { color: var(--muted); font-size: 14px; }
.kv .vv { font-weight: 700; }
.quick .big { font-size: 20px; font-weight: 700; margin: 2px 0 0; }
.quick h3 { font-size: 17px; }
.legend b { display: block; line-height: 1.4; }
.legend span.d { color: var(--muted); display: block; }
.important { background: var(--no-bg); border-color: var(--no-line); display: grid; grid-template-columns: 30px minmax(0, 1fr); gap: 12px; align-items: start; }
.important .n { background: var(--no); color: var(--card); }
.important h3 { color: var(--no); }
.important .big { font-weight: 700; margin: 4px 0 0; }
.two { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 12px; }
.yes, .nay { display: flex; flex-direction: column; gap: 6px; }
.yes { background: var(--ok-bg); border-color: var(--ok-line); }
.nay { background: var(--no-bg); border-color: var(--no-line); }
.yes h3 { color: var(--ok); font-size: 18px; }
.nay h3 { color: var(--no); font-size: 18px; }
.hint { color: var(--muted); font-size: 14px; margin: 0; }
.items { list-style: none; margin: 6px 0 0; padding: 0; display: grid; gap: 8px; }
.items li { display: grid; grid-template-columns: 22px minmax(0, 1fr); gap: 10px; align-items: start; }
.mk { width: 22px; height: 22px; border-radius: 50%; display: inline-grid; place-items: center; font-size: 13px; font-weight: 700; line-height: 1; margin-top: 2px; }
.yes .mk { background: var(--ok); color: var(--card); }
.nay .mk { background: var(--no); color: var(--card); }
/* svg remote */
.rb-body { fill: var(--remote); stroke: var(--line); stroke-width: 1.5; }
.rb-btn { fill: var(--btn); }
.rb-hi { fill: var(--card); stroke: var(--accent); stroke-width: 2; }
.rb-ink { stroke: var(--ink); fill: none; stroke-width: 2; stroke-linecap: round; stroke-linejoin: round; }
.rb-mut { fill: var(--muted); }
.rb-lead { stroke: var(--badge); stroke-width: 1.6; }
.rb-badge { fill: var(--badge); }
.rb-bt { fill: var(--badge-ink); font: 700 12px var(--font); text-anchor: middle; dominant-baseline: central; }
.rb-t { font: 700 11px var(--font); text-anchor: middle; dominant-baseline: central; fill: var(--ink); }
</style>

<main class="wrap">
  <header style="display:flex;flex-direction:column;gap:12px">
    <div class="brand">Guest Guide<span class="sep"> · </span><b class="shop">무드온 명동</b></div>
    <nav class="langs" id="langs" aria-label="Language">
      <button type="button" data-lang="en">English</button>
      <button type="button" data-lang="ko">한국어</button>
      <button type="button" data-lang="ja">日本語</button>
      <button type="button" data-lang="zh-hans">简体中文</button>
      <button type="button" data-lang="zh-hant">繁體中文</button>
      <button type="button" data-lang="es">Español</button>
      <button type="button" data-lang="fr">Français</button>
      <button type="button" data-lang="de">Deutsch</button>
    </nav>
    <nav class="tabs" id="tabs">
      <button type="button" data-topic="wifi"></button>
      <button type="button" data-topic="door"></button>
      <button type="button" data-topic="tv"></button>
      <button type="button" data-topic="ac"></button>
      <button type="button" data-topic="washer"></button>
      <button type="button" data-topic="food"></button>
      <button type="button" data-topic="trash"></button>
      <button type="button" data-topic="pickup"></button>
      <button type="button" data-topic="route"></button>
    </nav>
  </header>
  <div id="view" class="wrap" style="gap:14px"></div>
</main>

<script>
(function () {
  var REMOTE =
    '<svg viewBox="0 0 200 436" role="img" xmlns="http://www.w3.org/2000/svg">' +
    '<rect class="rb-body" x="42" y="6" width="116" height="422" rx="56"/>' +
    '<circle class="rb-hi" cx="100" cy="44" r="14"/>' +
    '<path d="M94.8 39.8a7.6 7.6 0 1 0 10.4 0M100 36v7" fill="none" stroke="#d64545" stroke-width="2.2" stroke-linecap="round"/>' +
    '<g class="rb-btn">' +
      '<rect x="58" y="84" width="24" height="14" rx="7"/><rect x="88" y="84" width="24" height="14" rx="7"/><rect x="118" y="84" width="24" height="14" rx="7"/>' +
      '<rect x="58" y="106" width="24" height="14" rx="7"/><rect x="88" y="106" width="24" height="14" rx="7"/><rect x="118" y="106" width="24" height="14" rx="7"/>' +
      '<rect x="58" y="128" width="24" height="14" rx="7"/><rect x="88" y="128" width="24" height="14" rx="7"/><rect x="118" y="128" width="24" height="14" rx="7"/>' +
    '</g>' +
    '<circle class="rb-hi" cx="100" cy="204" r="42"/>' +
    '<circle cx="100" cy="204" r="17" fill="var(--bg)" stroke="var(--line)" stroke-width="1.5"/>' +
    '<text class="rb-t" x="100" y="204">OK</text>' +
    '<g class="rb-mut"><polygon points="100,170 95,178 105,178"/><polygon points="100,238 95,230 105,230"/><polygon points="66,204 74,199 74,209"/><polygon points="134,204 126,199 126,209"/></g>' +
    '<circle class="rb-hi" cx="70" cy="268" r="12"/><path class="rb-ink" d="M76 268H64M69 263l-5 5 5 5"/>' +
    '<circle class="rb-btn" cx="100" cy="268" r="8"/>' +
    '<circle class="rb-hi" cx="130" cy="268" r="12"/><path class="rb-ink" d="M124 269l6-6 6 6M126 268v6h8v-6"/>' +
    '<rect class="rb-hi" x="58" y="296" width="26" height="62" rx="13"/><text class="rb-t" x="71" y="311">+</text><text class="rb-t" x="71" y="343">–</text>' +
    '<rect class="rb-btn" x="116" y="296" width="26" height="62" rx="13"/><text class="rb-t" x="129" y="311">+</text><text class="rb-t" x="129" y="343">–</text>' +
    '<circle class="rb-btn" cx="100" cy="327" r="9"/>' +
    '<rect class="rb-hi" x="56" y="382" width="40" height="22" rx="7"/><text x="76" y="393" text-anchor="middle" dominant-baseline="central" font-family="sans-serif" font-weight="700" font-size="7" fill="#e50914">NETFLIX</text>' +
    '<rect class="rb-hi" x="104" y="382" width="40" height="22" rx="7"/><text x="124" y="393" text-anchor="middle" dominant-baseline="central" font-family="sans-serif" font-weight="700" font-size="7" fill="#d62c2c">YouTube</text>' +
    '<g><line class="rb-lead" x1="29" y1="44" x2="84" y2="44"/><circle class="rb-badge" cx="18" cy="44" r="11"/><text class="rb-bt" x="18" y="44">1</text></g>' +
    '<g><line class="rb-lead" x1="29" y1="327" x2="58" y2="327"/><circle class="rb-badge" cx="18" cy="327" r="11"/><text class="rb-bt" x="18" y="327">2</text></g>' +
    '<g><line class="rb-lead" x1="171" y1="393" x2="144" y2="393"/><circle class="rb-badge" cx="182" cy="393" r="11"/><text class="rb-bt" x="182" y="393">3</text></g>' +
    '<g><line class="rb-lead" x1="171" y1="204" x2="142" y2="204"/><circle class="rb-badge" cx="182" cy="204" r="11"/><text class="rb-bt" x="182" y="204">4</text></g>' +
    '<g><line class="rb-lead" x1="171" y1="268" x2="142" y2="268"/><circle class="rb-badge" cx="182" cy="268" r="11"/><text class="rb-bt" x="182" y="268">5</text></g>' +
    '<g><line class="rb-lead" x1="29" y1="268" x2="58" y2="268"/><circle class="rb-badge" cx="18" cy="268" r="11"/><text class="rb-bt" x="18" y="268">6</text></g>' +
    '</svg>';

  /* Strings. [[...]] = label printed on the machine (shown as a chip). {pp} = the play/pause button. */
  var T = {
    en: {
      tabs: ["TV", "A/C", "Washer & Dryer", "Food Waste"],
      tv: { h: "TV Remote Guide", alt: "TV remote with buttons numbered 1 to 6", items: [
        ["Power", "Press the red power button to turn the TV on or off."],
        ["Volume", "Use the + / – buttons to adjust the volume."],
        ["Netflix / YouTube", "Press the NETFLIX or YouTube button to open the app."],
        ["Navigation / OK", "Use the round ring to move up, down, left, and right. Press the center button to select."],
        ["Home", "Press Home to return to the main screen."],
        ["Back", "Press Back to go to the previous screen."] ] },
      a: {"h": "Air Conditioner Guide", "qt": "I want to use the air conditioner.", "qb": "Press the Mode ([[모드]]) button to select Cool or Heat.", "items": [["Power On / Off", "Press to turn the air conditioner on or off."], ["Mode (Cool / Heat)", "Press the [[모드]] button to select Cool for cooling or Heat for heating. Each press changes the mode in order."], ["Temperature", "Press + or – ([[온도]]) to adjust the desired temperature."], ["Wind-Free Mode", "Press [[무풍]] for gentle cooling with soft airflow."], ["Airflow Up / Down", "Press ^ / v ([[바람]]) to adjust the vertical airflow direction."], ["Airflow Left / Right", "Adjusts the horizontal airflow direction."], ["Timer", "Press [[예약설정]] to set the timer or reservation."], ["Additional Functions", "Press [[부가기능]] to access extra features or settings."], ["Confirm / OK", "Press [[확인]] to confirm your selection."], ["Back", "Returns to the previous step or cancels a setting."]]},
      w: { h: "Washing Machine & Dryer", wt: "Washing machine", steps: [
        ["Press the power button.", "Press the power button to turn it on."],
        ["Check the display.", "The numbers will appear on the display."],
        ["Start washing.", "Press the {pp} button to start the wash cycle."],
        ["Wait for the sound.", "A sound will play when the wash is complete."],
        ["Open the door.", "Press and hold the {pp} button for about 3 seconds to unlock and open the door."] ],
        dt: "Dryer", dsteps: [
        ["Turn the dial to dryer mode.", "Turn the dial until the light is on the dryer ([[건조기]]) mode."],
        ["Start drying.", "Press the upper {pp} button to start drying."] ],
        it: "Important", ib: "Please do not wash the accommodation towels together with your personal clothes.", id: "The towels may change color if washed with other clothes. Please wash accommodation towels separately." },
      f: { h: "Food Waste Processor", sub: "CUCKOO", steps: [
        ["Press the power button.", "Press the power button ([[전원/취소]]) to turn it on."],
        ["Select a mode.", "Choose a mode ([[표준/쾌속]]) for normal use."],
        ["Add food waste.", "Put food waste into the processor."],
        ["It runs automatically.", "It dries and processes the food waste by itself. This takes about 1 hour."],
        ["Completed!", "After about 1 hour the process is finished and you can use it again whenever needed."] ],
        okT: "What you can put in", okS: "General food waste from daily meals",
        ok: ["Vegetable and fruit peels", "Leftover food", "Small bones and shells (chicken, fish, etc.)"],
        noT: "Do not put in", noS: "Items that may cause malfunction",
        no: ["Plastic bags and vinyl", "Metal, foil, packaging", "Large bones (beef/pork)", "Non-food items (tissues, sticks, etc.)"] }
    },
    ko: {
      tabs: ["TV", "에어컨", "세탁기·건조기", "음식물 처리기"],
      tv: { h: "TV 리모컨 안내", alt: "버튼에 1~6 번호가 붙은 TV 리모컨 그림", items: [
        ["전원", "빨간 전원 버튼을 누르면 TV가 켜지고 꺼집니다."],
        ["볼륨", "+ / – 버튼으로 소리를 조절하세요."],
        ["넷플릭스 / 유튜브", "NETFLIX 또는 YouTube 버튼을 누르면 앱이 열립니다."],
        ["방향 / OK", "동그란 링으로 위, 아래, 왼쪽, 오른쪽으로 이동하세요. 가운데 버튼을 누르면 선택됩니다."],
        ["홈", "홈 버튼을 누르면 메인 화면으로 돌아갑니다."],
        ["뒤로", "뒤로 버튼을 누르면 이전 화면으로 갑니다."] ] },
      a: {"h": "에어컨 냉난방기 사용법", "qt": "에어컨을 사용하고 싶어요.", "qb": "[[모드]] 버튼을 눌러 냉방(Cool) 또는 난방(Heat)을 선택하세요.", "items": [["전원 켜기 / 끄기", "누르면 에어컨이 켜지고 꺼집니다."], ["모드 (냉방 / 난방)", "[[모드]] 버튼으로 운전 모드를 고르세요. Cool은 냉방, Heat는 난방입니다. 누를 때마다 모드가 순서대로 바뀝니다."], ["온도", "+ 또는 – ([[온도]])를 눌러 원하는 온도로 맞추세요."], ["무풍 모드", "[[무풍]]을 누르면 바람이 약한 부드러운 냉방이 됩니다."], ["바람 방향 (위 / 아래)", "^ / v ([[바람]])로 바람의 상하 방향을 조절합니다."], ["바람 방향 (좌 / 우)", "바람의 좌우 방향을 조절합니다."], ["예약 / 타이머", "[[예약설정]]을 눌러 타이머나 예약을 설정합니다."], ["부가 기능", "[[부가기능]]을 눌러 추가 기능이나 설정을 엽니다."], ["확인 / OK", "[[확인]]을 눌러 선택을 확정합니다."], ["뒤로", "이전 단계로 돌아가거나 설정을 취소합니다."]]},
      w: { h: "세탁기 · 건조기 사용법", wt: "세탁기", steps: [
        ["전원 버튼을 누르세요.", "전원 버튼을 눌러 켜세요."],
        ["화면을 확인하세요.", "화면에 숫자가 나타납니다."],
        ["세탁 시작", "{pp} 버튼을 누르면 세탁이 시작됩니다."],
        ["소리를 기다리세요.", "세탁이 끝나면 소리가 납니다."],
        ["문 열기", "{pp} 버튼을 약 3초간 길게 누르면 잠금이 풀리고 문이 열립니다."] ],
        dt: "건조기", dsteps: [
        ["다이얼을 건조기 모드로", "불이 건조기([[건조기]]) 모드에 들어올 때까지 다이얼을 돌리세요."],
        ["건조 시작", "위쪽 {pp} 버튼을 누르면 건조가 시작됩니다."] ],
        it: "중요", ib: "숙소 수건은 개인 옷과 함께 빨지 마세요.", id: "다른 옷과 함께 빨면 수건 색이 변할 수 있습니다. 숙소 수건은 따로 세탁해 주세요." },
      f: { h: "음식물 처리기 사용법", sub: "CUCKOO", steps: [
        ["전원 버튼을 누르세요.", "전원 버튼([[전원/취소]])을 눌러 켜세요."],
        ["모드 선택", "일반적으로는 [[표준/쾌속]] 모드를 선택하세요."],
        ["음식물 넣기", "음식물 쓰레기를 처리기에 넣으세요."],
        ["자동으로 작동", "음식물을 알아서 건조·처리합니다. 약 1시간 걸립니다."],
        ["완료!", "약 1시간 후 처리가 끝나면 필요할 때 다시 사용할 수 있습니다."] ],
        okT: "넣어도 되는 것", okS: "일상 식사에서 나오는 일반 음식물",
        ok: ["채소·과일 껍질", "남은 음식", "작은 뼈와 껍데기(닭, 생선 등)"],
        noT: "넣으면 안 되는 것", noS: "고장의 원인이 될 수 있는 물건",
        no: ["비닐봉지와 비닐", "금속, 호일, 포장재", "큰 뼈(소·돼지)", "음식이 아닌 것(휴지, 나무젓가락 등)"] }
    },
    ja: {
      tabs: ["テレビ", "エアコン", "洗濯機・乾燥機", "生ごみ処理機"],
      tv: { h: "テレビのリモコンの使い方", alt: "ボタンに1〜6の番号を付けたリモコンの図", items: [
        ["電源", "赤い電源ボタンを押すと、テレビのオン・オフができます。"],
        ["音量", "+ / – ボタンで音量を調整します。"],
        ["Netflix / YouTube", "NETFLIXまたはYouTubeのボタンを押すと、アプリが開きます。"],
        ["矢印 / OK", "丸いリングで上下左右に移動します。中央のボタンで決定します。"],
        ["ホーム", "ホームボタンでメイン画面に戻ります。"],
        ["戻る", "戻るボタンで前の画面に戻ります。"] ] },
      a: {"h": "エアコンの使い方", "qt": "エアコンを使いたいとき", "qb": "[[모드]] ボタンを押して、冷房(Cool)か暖房(Heat)を選びます。", "items": [["電源 オン / オフ", "押すとエアコンのオン・オフができます。"], ["モード(冷房 / 暖房)", "[[모드]] ボタンで運転モードを選びます。Coolは冷房、Heatは暖房です。押すたびにモードが順番に切り替わります。"], ["温度", "+ または – ([[온도]])で設定温度を調整します。"], ["無風モード", "[[무풍]] を押すと、やわらかい風でやさしく冷房します。"], ["風向き(上 / 下)", "^ / v ([[바람]])で風の上下方向を調整します。"], ["風向き(左 / 右)", "風の左右方向を調整します。"], ["タイマー", "[[예약설정]] を押してタイマー(予約)を設定します。"], ["追加機能", "[[부가기능]] を押すと、追加機能や設定が開きます。"], ["確認 / OK", "[[확인]] を押して選択を確定します。"], ["戻る", "前の手順に戻る、または設定を取り消します。"]]},
      w: { h: "洗濯機・乾燥機の使い方", wt: "洗濯機", steps: [
        ["電源ボタンを押す", "電源ボタンを押してオンにします。"],
        ["表示を確認する", "表示画面に数字が出ます。"],
        ["洗濯を始める", "{pp} ボタンを押すと洗濯が始まります。"],
        ["終了の音を待つ", "洗濯が終わると音が鳴ります。"],
        ["ドアを開ける", "{pp} ボタンを約3秒間長押しすると、ロックが解除されてドアが開きます。"] ],
        dt: "乾燥機", dsteps: [
        ["ダイヤルを乾燥機モードに", "ライトが乾燥機([[건조기]])モードになるまでダイヤルを回します。"],
        ["乾燥を始める", "上側の {pp} ボタンを押すと乾燥が始まります。"] ],
        it: "重要", ib: "客室のタオルをご自身の衣類と一緒に洗わないでください。", id: "他の衣類と一緒に洗うと、タオルの色が変わることがあります。客室のタオルは別に洗ってください。" },
      f: { h: "生ごみ処理機の使い方", sub: "CUCKOO", steps: [
        ["電源ボタンを押す", "電源ボタン([[전원/취소]])を押してオンにします。"],
        ["モードを選ぶ", "通常は [[표준/쾌속]] モードを選びます。"],
        ["生ごみを入れる", "生ごみを処理機に入れます。"],
        ["自動で運転", "自動で乾燥・処理します。約1時間かかります。"],
        ["完了!", "約1時間で処理が終わり、必要なときにまた使えます。"] ],
        okT: "入れてよいもの", okS: "普段の食事で出る一般的な生ごみ",
        ok: ["野菜・果物の皮", "食べ残し", "小さな骨や殻(鶏、魚など)"],
        noT: "入れてはいけないもの", noS: "故障の原因になるもの",
        no: ["ビニール袋", "金属、アルミホイル、包装材", "大きな骨(牛・豚)", "食べ物ではないもの(ティッシュ、箸など)"] }
    },
    "zh-hans": {
      tabs: ["电视", "空调", "洗衣机·烘干机", "厨余处理机"],
      tv: { h: "电视遥控器使用指南", alt: "标有 1 到 6 号码按钮的遥控器示意图", items: [
        ["电源", "按红色电源按钮可开关电视。"],
        ["音量", "用 + / – 按钮调节音量。"],
        ["Netflix / YouTube", "按 NETFLIX 或 YouTube 按钮即可打开应用。"],
        ["方向键 / OK", "用圆环向上、下、左、右移动,按中间按钮确认。"],
        ["主页", "按主页键返回主屏幕。"],
        ["返回", "按返回键回到上一个画面。"] ] },
      a: {"h": "空调使用指南", "qt": "我想使用空调。", "qb": "按 [[모드]] 按钮,选择制冷(Cool)或制热(Heat)。", "items": [["开机 / 关机", "按下即可开启或关闭空调。"], ["模式(制冷 / 制热)", "按 [[모드]] 按钮选择运行模式。Cool 为制冷,Heat 为制热。每按一次,模式会依次切换。"], ["温度", "按 + 或 –([[온도]])调节所需温度。"], ["无风模式", "按 [[무풍]],以柔和的微风进行舒适制冷。"], ["风向(上 / 下)", "按 ^ / v([[바람]])调节上下风向。"], ["风向(左 / 右)", "调节左右风向。"], ["定时", "按 [[예약설정]] 设置定时或预约。"], ["附加功能", "按 [[부가기능]] 使用更多功能或设置。"], ["确认 / OK", "按 [[확인]] 确认所选内容。"], ["返回", "返回上一步,或取消当前设置。"]]},
      w: { h: "洗衣机和烘干机使用方法", wt: "洗衣机", steps: [
        ["按电源按钮", "按电源按钮开机。"],
        ["确认显示屏", "显示屏上会出现数字。"],
        ["开始洗衣", "按 {pp} 按钮开始洗涤。"],
        ["等待提示音", "洗涤完成时会响起提示音。"],
        ["开门", "长按 {pp} 按钮约 3 秒,解锁后即可开门。"] ],
        dt: "烘干机", dsteps: [
        ["把旋钮转到烘干模式", "转动旋钮,直到指示灯停在烘干机([[건조기]])模式。"],
        ["开始烘干", "按上方的 {pp} 按钮开始烘干。"] ],
        it: "重要", ib: "请勿将客房毛巾与您的个人衣物一起洗涤。", id: "与其他衣物一起洗,毛巾可能会变色。请将客房毛巾单独清洗。" },
      f: { h: "厨余处理机使用方法", sub: "CUCKOO", steps: [
        ["按电源按钮", "按电源按钮([[전원/취소]])开机。"],
        ["选择模式", "日常使用请选择 [[표준/쾌속]] 模式。"],
        ["放入厨余", "把厨余垃圾放进处理机。"],
        ["自动运行", "机器会自动烘干并处理厨余,大约需要 1 小时。"],
        ["完成!", "约 1 小时后处理结束,需要时可以再次使用。"] ],
        okT: "可以放入", okS: "日常饮食产生的一般厨余",
        ok: ["蔬菜和水果皮", "剩饭剩菜", "小骨头和壳(鸡、鱼等)"],
        noT: "不可放入", noS: "可能导致故障的物品",
        no: ["塑料袋和塑料膜", "金属、锡纸、包装材料", "大骨头(牛、猪)", "非食物(纸巾、筷子等)"] }
    },
    "zh-hant": {
      tabs: ["電視", "空調", "洗衣機・烘乾機", "廚餘處理機"],
      tv: { h: "電視遙控器使用指南", alt: "標有 1 到 6 號碼按鈕的遙控器示意圖", items: [
        ["電源", "按紅色電源按鈕可開關電視。"],
        ["音量", "用 + / – 按鈕調整音量。"],
        ["Netflix / YouTube", "按 NETFLIX 或 YouTube 按鈕即可開啟應用程式。"],
        ["方向鍵 / OK", "用圓環向上、下、左、右移動,按中間按鈕確認。"],
        ["主頁", "按主頁鍵回到主畫面。"],
        ["返回", "按返回鍵回到上一個畫面。"] ] },
      a: {"h": "冷氣使用指南", "qt": "我想使用冷氣。", "qb": "按 [[모드]] 按鈕,選擇冷氣(Cool)或暖氣(Heat)。", "items": [["開機 / 關機", "按下即可開啟或關閉冷氣。"], ["模式(冷氣 / 暖氣)", "按 [[모드]] 按鈕選擇運轉模式。Cool 為冷氣,Heat 為暖氣。每按一次,模式會依序切換。"], ["溫度", "按 + 或 –([[온도]])調整所需溫度。"], ["無風模式", "按 [[무풍]],以柔和的微風進行舒適製冷。"], ["風向(上 / 下)", "按 ^ / v([[바람]])調整上下風向。"], ["風向(左 / 右)", "調整左右風向。"], ["定時", "按 [[예약설정]] 設定定時或預約。"], ["附加功能", "按 [[부가기능]] 使用更多功能或設定。"], ["確認 / OK", "按 [[확인]] 確認所選內容。"], ["返回", "返回上一步,或取消目前設定。"]]},
      w: { h: "洗衣機與烘乾機使用方法", wt: "洗衣機", steps: [
        ["按電源按鈕", "按電源按鈕開機。"],
        ["確認顯示螢幕", "顯示螢幕上會出現數字。"],
        ["開始洗衣", "按 {pp} 按鈕開始洗滌。"],
        ["等待提示音", "洗滌完成時會響起提示音。"],
        ["開門", "長按 {pp} 按鈕約 3 秒,解鎖後即可開門。"] ],
        dt: "烘乾機", dsteps: [
        ["把旋鈕轉到烘乾模式", "轉動旋鈕,直到指示燈停在烘乾機([[건조기]])模式。"],
        ["開始烘乾", "按上方的 {pp} 按鈕開始烘乾。"] ],
        it: "重要", ib: "請勿將客房毛巾與您的個人衣物一起洗滌。", id: "與其他衣物一起洗,毛巾可能會變色。請將客房毛巾單獨清洗。" },
      f: { h: "廚餘處理機使用方法", sub: "CUCKOO", steps: [
        ["按電源按鈕", "按電源按鈕([[전원/취소]])開機。"],
        ["選擇模式", "日常使用請選擇 [[표준/쾌속]] 模式。"],
        ["放入廚餘", "把廚餘放進處理機。"],
        ["自動運行", "機器會自動烘乾並處理廚餘,大約需要 1 小時。"],
        ["完成!", "約 1 小時後處理結束,需要時可以再次使用。"] ],
        okT: "可以放入", okS: "日常飲食產生的一般廚餘",
        ok: ["蔬菜和水果皮", "剩飯剩菜", "小骨頭和殼(雞、魚等)"],
        noT: "不可放入", noS: "可能導致故障的物品",
        no: ["塑膠袋", "金屬、鋁箔、包裝材料", "大骨頭(牛、豬)", "非食物(衛生紙、筷子等)"] }
    },
    es: {"tabs": ["TV", "A/C", "Lavadora", "Restos"], "tv": {"h": "Guía del mando de la TV", "alt": "Mando de la TV con los botones numerados del 1 al 6", "items": [["Encendido", "Pulsa el botón rojo para encender o apagar la TV."], ["Volumen", "Usa los botones + / – para ajustar el volumen."], ["Netflix / YouTube", "Pulsa el botón NETFLIX o YouTube para abrir la aplicación."], ["Navegación / OK", "Usa el anillo redondo para moverte arriba, abajo, a la izquierda y a la derecha. Pulsa el botón central para seleccionar."], ["Inicio", "Pulsa Inicio para volver a la pantalla principal."], ["Atrás", "Pulsa Atrás para volver a la pantalla anterior."]]}, "a": {"h": "Guía del aire acondicionado", "qt": "Quiero usar el aire acondicionado.", "qb": "Pulsa el botón Modo ([[모드]]) para elegir Frío (Cool) o Calor (Heat).", "items": [["Encender / apagar", "Púlsalo para encender o apagar el aire acondicionado."], ["Modo (frío / calor)", "Pulsa el botón [[모드]] para elegir Cool (frío) o Heat (calor). Cada pulsación cambia el modo en orden."], ["Temperatura", "Pulsa + o – ([[온도]]) para ajustar la temperatura deseada."], ["Modo Wind-Free (sin viento)", "Pulsa [[무풍]] para enfriar suavemente con un flujo de aire leve."], ["Dirección del aire (arriba / abajo)", "Pulsa ^ / v ([[바람]]) para ajustar la dirección vertical del aire."], ["Dirección del aire (izquierda / derecha)", "Ajusta la dirección horizontal del aire."], ["Temporizador", "Pulsa [[예약설정]] para programar el temporizador."], ["Funciones adicionales", "Pulsa [[부가기능]] para acceder a funciones o ajustes adicionales."], ["Confirmar / OK", "Pulsa [[확인]] para confirmar tu selección."], ["Atrás", "Vuelve al paso anterior o cancela un ajuste."]]}, "w": {"h": "Lavadora y secadora", "wt": "Lavadora", "steps": [["Pulsa el botón de encendido.", "Pulsa el botón de encendido para encenderla."], ["Comprueba la pantalla.", "Aparecerán números en la pantalla."], ["Empieza a lavar.", "Pulsa el botón {pp} para iniciar el lavado."], ["Espera el sonido.", "Sonará un aviso cuando termine el lavado."], ["Abre la puerta.", "Mantén pulsado el botón {pp} unos 3 segundos para desbloquear y abrir la puerta."]], "dt": "Secadora", "dsteps": [["Gira el dial al modo secadora.", "Gira el dial hasta que la luz se ponga en el modo secadora ([[건조기]])."], ["Empieza a secar.", "Pulsa el botón {pp} de arriba para iniciar el secado."]], "it": "Importante", "ib": "Por favor, no laves las toallas del alojamiento junto con tu ropa personal.", "id": "Las toallas pueden cambiar de color si se lavan con otra ropa. Lava las toallas del alojamiento por separado."}, "f": {"h": "Procesador de restos de comida", "sub": "CUCKOO", "steps": [["Pulsa el botón de encendido.", "Pulsa el botón de encendido ([[전원/취소]]) para encenderlo."], ["Elige un modo.", "Elige un modo ([[표준/쾌속]]) para el uso normal."], ["Añade los restos de comida.", "Echa los restos de comida en el procesador."], ["Funciona automáticamente.", "Seca y procesa los restos de comida por sí solo. Tarda aproximadamente 1 hora."], ["¡Listo!", "Pasada aproximadamente 1 hora, el proceso termina y puedes volver a usarlo cuando lo necesites."]], "okT": "Qué puedes echar", "okS": "Restos de comida habituales de las comidas diarias", "ok": ["Cáscaras de verduras y frutas", "Sobras de comida", "Huesos pequeños y cáscaras (pollo, pescado, etc.)"], "noT": "Qué no debes echar", "noS": "Objetos que pueden causar averías", "no": ["Bolsas de plástico y film", "Metal, papel de aluminio, envases", "Huesos grandes (ternera/cerdo)", "Objetos que no son comida (pañuelos, palillos, etc.)"]}},
    fr: {"tabs": ["TV", "Clim", "Linge", "Déchets"], "tv": {"h": "Guide de la télécommande TV", "alt": "Télécommande TV avec les boutons numérotés de 1 à 6", "items": [["Marche / Arrêt", "Appuyez sur le bouton rouge pour allumer ou éteindre la TV."], ["Volume", "Utilisez les boutons + / – pour régler le volume."], ["Netflix / YouTube", "Appuyez sur le bouton NETFLIX ou YouTube pour ouvrir l'application."], ["Navigation / OK", "Utilisez l'anneau rond pour vous déplacer vers le haut, le bas, la gauche et la droite. Appuyez sur le bouton central pour valider."], ["Accueil", "Appuyez sur Accueil pour revenir à l'écran principal."], ["Retour", "Appuyez sur Retour pour revenir à l'écran précédent."]]}, "a": {"h": "Guide de la climatisation", "qt": "Je veux utiliser la climatisation.", "qb": "Appuyez sur le bouton Mode ([[모드]]) pour choisir Froid (Cool) ou Chaud (Heat).", "items": [["Marche / Arrêt", "Appuyez pour allumer ou éteindre la climatisation."], ["Mode (froid / chaud)", "Appuyez sur le bouton [[모드]] pour choisir Cool (froid) ou Heat (chaud). Chaque pression change le mode dans l'ordre."], ["Température", "Appuyez sur + ou – ([[온도]]) pour régler la température souhaitée."], ["Mode Wind-Free (sans courant d'air)", "Appuyez sur [[무풍]] pour un rafraîchissement doux avec un flux d'air léger."], ["Flux d'air (haut / bas)", "Appuyez sur ^ / v ([[바람]]) pour régler la direction verticale du flux d'air."], ["Flux d'air (gauche / droite)", "Règle la direction horizontale du flux d'air."], ["Minuterie", "Appuyez sur [[예약설정]] pour programmer la minuterie."], ["Fonctions supplémentaires", "Appuyez sur [[부가기능]] pour accéder à d'autres fonctions ou réglages."], ["Valider / OK", "Appuyez sur [[확인]] pour valider votre choix."], ["Retour", "Revient à l'étape précédente ou annule un réglage."]]}, "w": {"h": "Lave-linge et sèche-linge", "wt": "Lave-linge", "steps": [["Appuyez sur le bouton marche.", "Appuyez sur le bouton marche pour l'allumer."], ["Vérifiez l'écran.", "Des chiffres s'affichent à l'écran."], ["Lancez le lavage.", "Appuyez sur le bouton {pp} pour démarrer le cycle de lavage."], ["Attendez le signal sonore.", "Un signal sonore retentit à la fin du lavage."], ["Ouvrez la porte.", "Maintenez le bouton {pp} enfoncé environ 3 secondes pour déverrouiller et ouvrir la porte."]], "dt": "Sèche-linge", "dsteps": [["Tournez le cadran sur le mode séchage.", "Tournez le cadran jusqu'à ce que le voyant s'allume sur le mode sèche-linge ([[건조기]])."], ["Lancez le séchage.", "Appuyez sur le bouton {pp} du haut pour démarrer le séchage."]], "it": "Important", "ib": "Ne lavez pas les serviettes du logement avec vos vêtements personnels.", "id": "Les serviettes peuvent changer de couleur si elles sont lavées avec d'autres vêtements. Lavez-les séparément."}, "f": {"h": "Appareil à déchets alimentaires", "sub": "CUCKOO", "steps": [["Appuyez sur le bouton marche.", "Appuyez sur le bouton marche ([[전원/취소]]) pour l'allumer."], ["Choisissez un mode.", "Choisissez un mode ([[표준/쾌속]]) pour un usage normal."], ["Ajoutez les déchets.", "Mettez les déchets alimentaires dans l'appareil."], ["Fonctionnement automatique.", "L'appareil sèche et traite les déchets tout seul. Cela prend environ 1 heure."], ["Terminé !", "Après environ 1 heure, le traitement est terminé et vous pouvez le réutiliser quand vous voulez."]], "okT": "Ce que vous pouvez mettre", "okS": "Déchets alimentaires courants des repas", "ok": ["Épluchures de légumes et de fruits", "Restes de repas", "Petits os et coquilles (poulet, poisson, etc.)"], "noT": "À ne pas mettre", "noS": "Objets pouvant provoquer une panne", "no": ["Sacs en plastique et films", "Métal, aluminium, emballages", "Gros os (bœuf/porc)", "Objets non alimentaires (mouchoirs, baguettes, etc.)"]}},
    de: {"tabs": ["TV", "Klima", "Wäsche", "Reste"], "tv": {"h": "TV-Fernbedienung – Anleitung", "alt": "TV-Fernbedienung mit den Tasten 1 bis 6", "items": [["Ein / Aus", "Drücken Sie die rote Taste, um den Fernseher ein- oder auszuschalten."], ["Lautstärke", "Mit den Tasten + / – stellen Sie die Lautstärke ein."], ["Netflix / YouTube", "Drücken Sie die Taste NETFLIX oder YouTube, um die App zu öffnen."], ["Navigation / OK", "Mit dem runden Ring bewegen Sie sich nach oben, unten, links und rechts. Mit der mittleren Taste wählen Sie aus."], ["Startseite", "Drücken Sie Home, um zum Startbildschirm zurückzukehren."], ["Zurück", "Drücken Sie Zurück, um zum vorherigen Bildschirm zu gelangen."]]}, "a": {"h": "Klimaanlage – Anleitung", "qt": "Ich möchte die Klimaanlage benutzen.", "qb": "Drücken Sie die Taste Modus ([[모드]]), um Kühlen (Cool) oder Heizen (Heat) zu wählen.", "items": [["Ein / Aus", "Drücken, um die Klimaanlage ein- oder auszuschalten."], ["Modus (Kühlen / Heizen)", "Mit der Taste [[모드]] wählen Sie Cool (Kühlen) oder Heat (Heizen). Mit jedem Druck wechselt der Modus der Reihe nach."], ["Temperatur", "Mit + oder – ([[온도]]) stellen Sie die gewünschte Temperatur ein."], ["Wind-Free-Modus (zugfrei)", "Drücken Sie [[무풍]] für sanftes Kühlen mit schwachem Luftstrom."], ["Luftrichtung (oben / unten)", "Mit ^ / v ([[바람]]) stellen Sie die vertikale Luftrichtung ein."], ["Luftrichtung (links / rechts)", "Stellt die horizontale Luftrichtung ein."], ["Timer", "Drücken Sie [[예약설정]], um den Timer einzustellen."], ["Zusatzfunktionen", "Mit [[부가기능]] öffnen Sie zusätzliche Funktionen oder Einstellungen."], ["Bestätigen / OK", "Drücken Sie [[확인]], um Ihre Auswahl zu bestätigen."], ["Zurück", "Geht einen Schritt zurück oder bricht eine Einstellung ab."]]}, "w": {"h": "Waschmaschine und Trockner", "wt": "Waschmaschine", "steps": [["Ein-/Aus-Taste drücken.", "Drücken Sie die Ein-/Aus-Taste, um das Gerät einzuschalten."], ["Display prüfen.", "Auf dem Display erscheinen Zahlen."], ["Waschen starten.", "Drücken Sie die Taste {pp}, um das Waschprogramm zu starten."], ["Auf den Signalton warten.", "Nach dem Waschen ertönt ein Signalton."], ["Tür öffnen.", "Halten Sie die Taste {pp} etwa 3 Sekunden gedrückt, um die Tür zu entriegeln und zu öffnen."]], "dt": "Trockner", "dsteps": [["Drehknopf auf Trockner stellen.", "Drehen Sie den Knopf, bis die Anzeige beim Trockner ([[건조기]]) leuchtet."], ["Trocknen starten.", "Drücken Sie die obere Taste {pp}, um das Trocknen zu starten."]], "it": "Wichtig", "ib": "Bitte waschen Sie die Handtücher der Unterkunft nicht zusammen mit Ihrer persönlichen Kleidung.", "id": "Die Handtücher können ihre Farbe verändern, wenn sie mit anderer Kleidung gewaschen werden. Bitte waschen Sie sie separat."}, "f": {"h": "Gerät für Speisereste", "sub": "CUCKOO", "steps": [["Ein-/Aus-Taste drücken.", "Drücken Sie die Ein-/Aus-Taste ([[전원/취소]]), um das Gerät einzuschalten."], ["Modus wählen.", "Wählen Sie für den normalen Gebrauch den Modus ([[표준/쾌속]])."], ["Speisereste einfüllen.", "Geben Sie die Speisereste in das Gerät."], ["Läuft automatisch.", "Das Gerät trocknet und verarbeitet die Speisereste selbstständig. Das dauert etwa 1 Stunde."], ["Fertig!", "Nach etwa 1 Stunde ist der Vorgang abgeschlossen und Sie können das Gerät bei Bedarf wieder benutzen."]], "okT": "Das dürfen Sie einfüllen", "okS": "Normale Speisereste aus den täglichen Mahlzeiten", "ok": ["Gemüse- und Obstschalen", "Essensreste", "Kleine Knochen und Schalen (Huhn, Fisch usw.)"], "noT": "Das darf nicht hinein", "noS": "Gegenstände, die Störungen verursachen können", "no": ["Plastiktüten und Folie", "Metall, Alufolie, Verpackungen", "Große Knochen (Rind/Schwein)", "Keine Lebensmittel (Taschentücher, Stäbchen usw.)"]}}
  };
  var WF = {"en": {"tab": "Wi-Fi", "h": "Wi-Fi Information", "sub": "Here's the Wi-Fi info for your stay!", "free": "Feel free to use it anytime!", "ssid": "Network name (SSID)", "pw": "Password", "note": "The Mesh network can be used at the same time as Buddy.", "help": "If you have any trouble connecting, please let us know. We'll be happy to help!", "copy": "Copy", "copied": "Copied"}, "ko": {"tab": "와이파이", "h": "Wi-Fi 정보", "sub": "숙박 중에 사용하실 Wi-Fi 정보입니다!", "free": "언제든 편하게 이용하세요!", "ssid": "네트워크 이름 (SSID)", "pw": "비밀번호 (Password)", "note": "Mesh 무선랜은 Buddy와 동시에 사용 시 접속이 가능합니다.", "help": "연결에 문제가 있으면 언제든 알려주세요. 기꺼이 도와드리겠습니다!", "copy": "복사", "copied": "복사됨"}, "ja": {"tab": "Wi-Fi", "h": "Wi-Fi情報", "sub": "ご滞在中のWi-Fi情報です。", "free": "いつでもご自由にお使いください。", "ssid": "ネットワーク名(SSID)", "pw": "パスワード", "note": "MeshネットワークはBuddyと同時に使用できます。", "help": "接続でお困りの際は、お気軽にお知らせください。喜んでお手伝いします。", "copy": "コピー", "copied": "コピーしました"}, "zh-hans": {"tab": "Wi-Fi", "h": "Wi-Fi 信息", "sub": "这是您入住期间的 Wi-Fi 信息!", "free": "请随时放心使用!", "ssid": "网络名称(SSID)", "pw": "密码", "note": "Mesh 网络可与 Buddy 同时使用。", "help": "如果连接遇到问题,请告诉我们,我们很乐意帮助您!", "copy": "复制", "copied": "已复制"}, "zh-hant": {"tab": "Wi-Fi", "h": "Wi-Fi 資訊", "sub": "這是您住宿期間的 Wi-Fi 資訊!", "free": "歡迎隨時使用!", "ssid": "網路名稱(SSID)", "pw": "密碼", "note": "Mesh 網路可與 Buddy 同時使用。", "help": "若連線時遇到問題,請告訴我們,我們很樂意協助您!", "copy": "複製", "copied": "已複製"}, "es": {"tab": "Wi-Fi", "h": "Información del Wi-Fi", "sub": "¡Aquí tienes los datos del Wi-Fi para tu estancia!", "free": "¡Úsalo cuando quieras!", "ssid": "Nombre de la red (SSID)", "pw": "Contraseña", "note": "La red Mesh se puede usar al mismo tiempo que Buddy.", "help": "Si tienes algún problema para conectarte, avísanos. ¡Estaremos encantados de ayudarte!", "copy": "Copiar", "copied": "Copiado"}, "fr": {"tab": "Wi-Fi", "h": "Informations Wi-Fi", "sub": "Voici les informations Wi-Fi pour votre séjour !", "free": "Utilisez-le quand vous voulez !", "ssid": "Nom du réseau (SSID)", "pw": "Mot de passe", "note": "Le réseau Mesh peut être utilisé en même temps que Buddy.", "help": "Si vous avez des difficultés pour vous connecter, dites-le-nous. Nous serons ravis de vous aider !", "copy": "Copier", "copied": "Copié"}, "de": {"tab": "WLAN", "h": "WLAN-Informationen", "sub": "Hier sind die WLAN-Daten für Ihren Aufenthalt!", "free": "Nutzen Sie es jederzeit!", "ssid": "Netzwerkname (SSID)", "pw": "Passwort", "note": "Das Mesh-Netzwerk kann gleichzeitig mit Buddy genutzt werden.", "help": "Falls Sie Probleme bei der Verbindung haben, sagen Sie uns bitte Bescheid. Wir helfen gern!", "copy": "Kopieren", "copied": "Kopiert"}};
  var TR = {"en": {"tab": "Trash", "h": "Trash Disposal Guide", "intro": "Korea's waste-sorting system may be unfamiliar if you are visiting from abroad. Please follow the guide below.", "gen": ["General waste", "White bag with printed text. For tissues and waste with food on it."], "food": ["Food waste", "Use the food waste processor on the sink counter."], "rec": ["Recycling", "White bag without text, placed inside the recycling bins. For plastic, cans, bottles, and glass."], "bagsT": "Where are the bags?", "bags": "Trash bags are in the second compartment of the cabinet under the sink.", "rulesT": "Please note", "n1": "Trash can only be put out after 9 PM, following Myeongdong area rules.", "n2": "Put it out at the 1st-floor spot shown above and it will be collected.", "thanks": "For a pleasant environment, please help us by sorting your trash. Thank you."}, "ko": {"tab": "쓰레기", "h": "쓰레기 배출 안내", "intro": "외국인 거주자분들께서는 한국의 분리수거 방식이 익숙하지 않으실 수 있습니다. 아래 안내를 참고해 주세요.", "gen": ["일반 쓰레기", "글씨가 있는 흰 봉투 (휴지, 음식물이 묻은 쓰레기)"], "food": ["음식물 쓰레기", "싱크대 위에 있는 음식물 처리기"], "rec": ["재활용품", "분리수거통에 씌워져 있는 글씨 없는 흰 봉투 (플라스틱, 캔, 병, 유리)"], "bagsT": "봉투는 어디에 있나요?", "bags": "쓰레기 봉투는 싱크대 하부장 2번째 자리에 있습니다.", "rulesT": "꼭 확인해 주세요", "n1": "쓰레기는 명동 지역 규정에 따라 저녁 9시 이후에만 배출 가능합니다.", "n2": "위에 안내된 1층 장소에 놓아주시면 수거됩니다.", "thanks": "쾌적한 환경을 위해 분리수거에 꼭 협조 부탁드립니다. 감사합니다."}, "ja": {"tab": "ゴミ", "h": "ゴミの出し方", "intro": "海外からお越しの方は、韓国の分別方法に慣れていないかもしれません。以下をご参照ください。", "gen": ["一般ゴミ", "文字の印刷された白い袋(ティッシュ、食べ物が付いたゴミ)"], "food": ["生ごみ", "シンクの上にある生ごみ処理機をご利用ください。"], "rec": ["リサイクル", "分別ボックスに入っている文字のない白い袋(プラスチック、缶、びん、ガラス)"], "bagsT": "ゴミ袋の場所", "bags": "ゴミ袋はシンク下の収納の2番目のスペースにあります。", "rulesT": "ご注意ください", "n1": "ゴミは明洞地区の規定により、夜9時以降のみ出すことができます。", "n2": "上記の1階の場所に置いていただければ回収されます。", "thanks": "快適な環境のため、分別にご協力をお願いいたします。ありがとうございます。"}, "zh-hans": {"tab": "垃圾", "h": "垃圾投放指南", "intro": "来自国外的住客可能不熟悉韩国的垃圾分类方式。请参考以下说明。", "gen": ["一般垃圾", "印有文字的白色垃圾袋(纸巾、沾有食物的垃圾)"], "food": ["厨余垃圾", "请使用水槽上方的厨余处理机。"], "rec": ["可回收物", "套在回收桶里、没有文字的白色垃圾袋(塑料、易拉罐、瓶子、玻璃)"], "bagsT": "垃圾袋在哪里?", "bags": "垃圾袋放在水槽下柜子的第二格。", "rulesT": "请注意", "n1": "根据明洞地区规定,垃圾只能在晚上 9 点以后投放。", "n2": "请放在上面所示的一楼位置,会有人来收取。", "thanks": "为了保持环境舒适,请配合垃圾分类。谢谢!"}, "zh-hant": {"tab": "垃圾", "h": "垃圾丟棄指南", "intro": "來自國外的住客可能不熟悉韓國的垃圾分類方式。請參考以下說明。", "gen": ["一般垃圾", "印有文字的白色垃圾袋(衛生紙、沾有食物的垃圾)"], "food": ["廚餘", "請使用水槽上方的廚餘處理機。"], "rec": ["資源回收", "套在回收桶裡、沒有文字的白色垃圾袋(塑膠、鋁罐、瓶子、玻璃)"], "bagsT": "垃圾袋在哪裡?", "bags": "垃圾袋放在水槽下櫃子的第二格。", "rulesT": "請注意", "n1": "依明洞地區規定,垃圾只能在晚上 9 點以後丟棄。", "n2": "請放在上面所示的一樓位置,會有人來收取。", "thanks": "為了維持舒適的環境,請配合垃圾分類。謝謝!"}, "es": {"tab": "Basura", "h": "Guía para tirar la basura", "intro": "Si vienes de otro país, quizá no conozcas el sistema coreano de separación de residuos. Consulta la siguiente guía.", "gen": ["Basura general", "Bolsa blanca con texto impreso. Para pañuelos y residuos con restos de comida."], "food": ["Restos de comida", "Usa el procesador de restos de comida que está sobre el fregadero."], "rec": ["Reciclaje", "Bolsa blanca sin texto, colocada dentro de los contenedores de reciclaje. Para plástico, latas, botellas y vidrio."], "bagsT": "¿Dónde están las bolsas?", "bags": "Las bolsas de basura están en el segundo compartimento del mueble bajo el fregadero.", "rulesT": "Importante", "n1": "Según la normativa de la zona de Myeongdong, la basura solo se puede sacar después de las 9 de la noche.", "n2": "Déjala en el lugar de la planta baja (1F) indicado arriba y la recogerán.", "thanks": "Para mantener un entorno agradable, te pedimos que separes los residuos. ¡Gracias!"}, "fr": {"tab": "Tri", "h": "Guide pour jeter les déchets", "intro": "Si vous venez de l'étranger, le système coréen de tri des déchets peut vous sembler inhabituel. Veuillez suivre le guide ci-dessous.", "gen": ["Déchets ordinaires", "Sac blanc avec du texte imprimé. Pour les mouchoirs et les déchets souillés par de la nourriture."], "food": ["Déchets alimentaires", "Utilisez l'appareil à déchets alimentaires placé sur l'évier."], "rec": ["Recyclage", "Sac blanc sans texte, placé dans les bacs de recyclage. Pour le plastique, les canettes, les bouteilles et le verre."], "bagsT": "Où sont les sacs ?", "bags": "Les sacs poubelle se trouvent dans le deuxième compartiment du meuble sous l'évier.", "rulesT": "À noter", "n1": "Selon le règlement du quartier de Myeongdong, les déchets ne peuvent être sortis qu'après 21 h.", "n2": "Déposez-les à l'endroit du rez-de-chaussée (1F) indiqué ci-dessus : ils seront collectés.", "thanks": "Pour préserver un cadre agréable, merci de bien vouloir trier vos déchets."}, "de": {"tab": "Müll", "h": "Hinweise zur Müllentsorgung", "intro": "Wenn Sie aus dem Ausland kommen, ist Ihnen das koreanische Mülltrennsystem vielleicht nicht vertraut. Bitte beachten Sie die folgende Anleitung.", "gen": ["Restmüll", "Weißer Beutel mit aufgedrucktem Text. Für Taschentücher und Abfall mit Essensresten."], "food": ["Speisereste", "Nutzen Sie das Gerät für Speisereste auf der Spüle."], "rec": ["Wertstoffe", "Weißer Beutel ohne Text, der in den Wertstoffbehältern steckt. Für Plastik, Dosen, Flaschen und Glas."], "bagsT": "Wo sind die Müllbeutel?", "bags": "Die Müllbeutel befinden sich im zweiten Fach des Unterschranks der Spüle.", "rulesT": "Bitte beachten", "n1": "Gemäß den Vorschriften im Stadtviertel Myeongdong darf der Müll nur nach 21 Uhr herausgestellt werden.", "n2": "Stellen Sie ihn an der oben gezeigten Stelle im Erdgeschoss (1F) ab; er wird dort abgeholt.", "thanks": "Für eine angenehme Umgebung bitten wir Sie, den Müll zu trennen. Vielen Dank!"}};
  var BIN = {"en": {"binT": "Recycling bins", "bin": "The recycling bins (Paper, Can, Plastic) are at the entrance of the room, each with a bag inside. Take the bag with you and put it out on the 1st floor.", "full": "If there is too much trash, please put it out on the 1st floor every night after 9 PM."}, "ko": {"binT": "분리수거통", "bin": "분리수거통(종이, 캔, 플라스틱)은 숙소 현관에 있고, 통마다 봉투가 씌워져 있습니다. 그 봉투를 그대로 가지고 1층에 배출하시면 됩니다.", "full": "쓰레기가 너무 많을 때는 매일 밤 9시 이후 1층에 배출해 주세요."}, "ja": {"binT": "分別ボックス", "bin": "分別ボックス(紙、缶、プラスチック)はお部屋の玄関にあり、それぞれ袋がかかっています。その袋を持って1階に出してください。", "full": "ゴミが多い場合は、毎晩夜9時以降に1階へ出してください。"}, "zh-hans": {"binT": "分类回收桶", "bin": "分类回收桶(纸张、罐头、塑料)放在房间入口处,每个桶里都套有垃圾袋。请带着垃圾袋放到一楼。", "full": "如果垃圾太多,请每晚 9 点以后放到一楼。"}, "zh-hant": {"binT": "分類回收桶", "bin": "分類回收桶(紙類、罐頭、塑膠)放在房間入口處,每個桶裡都套有垃圾袋。請帶著垃圾袋放到一樓。", "full": "如果垃圾太多,請每晚 9 點以後放到一樓。"}, "es": {"binT": "Contenedores de reciclaje", "bin": "Los contenedores de reciclaje (papel, latas y plástico) están en la entrada del alojamiento, cada uno con una bolsa puesta. Llévate la bolsa y déjala en la planta baja (1F).", "full": "Si hay demasiada basura, sácala a la planta baja (1F) cada noche después de las 9."}, "fr": {"binT": "Bacs de recyclage", "bin": "Les bacs de recyclage (papier, canettes et plastique) se trouvent à l'entrée du logement, chacun avec un sac à l'intérieur. Emportez le sac et déposez-le au rez-de-chaussée (1F).", "full": "S'il y a trop de déchets, sortez-les au rez-de-chaussée (1F) chaque soir après 21 h."}, "de": {"binT": "Wertstoffbehälter", "bin": "Die Wertstoffbehälter (Papier, Dosen und Plastik) stehen im Eingangsbereich der Unterkunft, jeweils mit einem Beutel darin. Nehmen Sie den Beutel mit und stellen Sie ihn im Erdgeschoss (1F) heraus.", "full": "Wenn zu viel Müll anfällt, stellen Sie ihn bitte jeden Abend nach 21 Uhr im Erdgeschoss (1F) heraus."}};
  var DROP = {"en": {"t": "Where to put out your trash (1st floor)", "c": ["Go down to the 1st floor and turn left.", "The alley is on your left, next to the yellow shop.", "Put your trash out in this alley."]}, "ko": {"t": "1층 배출 장소", "c": ["1층으로 내려와서 좌회전하세요.", "왼쪽에 있는 골목입니다. 노란색 가게 옆이에요.", "이 골목에 쓰레기를 내놓아 주세요."]}, "ja": {"t": "1階のゴミ置き場", "c": ["1階に下りて、左に曲がります。", "左側の路地です。黄色い店の横にあります。", "この路地にゴミを出してください。"]}, "zh-hans": {"t": "一楼垃圾投放位置", "c": ["下到一楼后向左转。", "左边的小巷,就在黄色店铺旁边。", "请把垃圾放在这条小巷里。"]}, "zh-hant": {"t": "一樓垃圾放置位置", "c": ["下到一樓後向左轉。", "左邊的小巷,就在黃色店面旁邊。", "請把垃圾放在這條小巷裡。"]}, "es": {"t": "Dónde dejar la basura (planta baja)", "c": ["Baja a la planta baja (1F) y gira a la izquierda.", "El callejón está a tu izquierda, junto a la tienda amarilla.", "Deja la basura en este callejón."]}, "fr": {"t": "Où déposer vos déchets (rez-de-chaussée)", "c": ["Descendez au rez-de-chaussée (1F) et tournez à gauche.", "La ruelle est sur votre gauche, à côté du magasin jaune.", "Déposez vos déchets dans cette ruelle."]}, "de": {"t": "Wo der Müll abgestellt wird (Erdgeschoss)", "c": ["Gehen Sie ins Erdgeschoss (1F) und biegen Sie links ab.", "Die Gasse liegt links, neben dem gelben Geschäft.", "Stellen Sie Ihren Müll in dieser Gasse ab."]}};
  var DROPDIM = [[1000, 710], [1000, 928], [992, 1160]];
  var DOOR = {"en": {"tab": "Entrance", "h": "Building Entrance Guide", "n": "For security, the front door on the 1st floor of the building is closed after 11 PM.", "t1": "Coming back late?", "s1": "Enter using the door lock.", "s2": "Then press the switch on the inside of the door so the door closes again.", "code": "Glass door lock code", "close": "This notice is for your comfortable stay."}, "ko": {"tab": "출입문", "h": "건물 출입문 안내", "n": "보안을 위해 건물 1층 출입문은 밤 11시 이후 닫아두고 있습니다.", "t1": "늦은 시간에 돌아오셨나요?", "s1": "도어락으로 출입해 주세요.", "s2": "들어오신 뒤, 문 안쪽에 있는 스위치를 눌러 출입문이 다시 닫히도록 해주세요.", "code": "유리출입문 도어락 비밀번호", "close": "편안한 이용을 위해 안내드립니다."}, "ja": {"tab": "出入口", "h": "建物の出入口のご案内", "n": "セキュリティのため、建物1階の出入口は夜11時以降は閉めています。", "t1": "遅い時間にお戻りですか?", "s1": "ドアロックで入ってください。", "s2": "入ったあと、ドアの内側にあるスイッチを押して、出入口が再び閉まるようにしてください。", "code": "ガラス扉のドアロック暗証番号", "close": "快適にご利用いただくためのご案内です。"}, "zh-hans": {"tab": "大门", "h": "楼栋入口使用说明", "n": "为了安全,大楼一楼的大门在晚上 11 点以后关闭。", "t1": "很晚才回来?", "s1": "请使用密码门锁进入。", "s2": "进入后,请按下门内侧的开关,让大门重新关闭。", "code": "玻璃门密码锁密码", "close": "以上说明是为了让您住得更舒适。"}, "zh-hant": {"tab": "大門", "h": "大樓入口使用說明", "n": "為了安全,大樓一樓的大門在晚上 11 點以後關閉。", "t1": "很晚才回來?", "s1": "請使用密碼門鎖進入。", "s2": "進入後,請按下門內側的開關,讓大門重新關閉。", "code": "玻璃門密碼鎖密碼", "close": "以上說明是為了讓您住得更舒適。"}, "es": {"tab": "Entrada", "h": "Guía de la puerta de entrada", "n": "Por seguridad, la puerta de entrada del edificio (1F) se cierra después de las 11 de la noche.", "t1": "¿Vuelves tarde?", "s1": "Entra con la cerradura electrónica.", "s2": "Después, pulsa el interruptor que está en el interior de la puerta para que se vuelva a cerrar.", "code": "Código de la cerradura de la puerta de cristal", "close": "Te lo indicamos para que tu estancia sea más cómoda."}, "fr": {"tab": "Entrée", "h": "Guide de la porte d'entrée", "n": "Pour des raisons de sécurité, la porte d'entrée de l'immeuble (1F) est fermée après 23 h.", "t1": "Vous rentrez tard ?", "s1": "Entrez avec la serrure à code.", "s2": "Ensuite, appuyez sur le bouton situé à l'intérieur de la porte pour qu'elle se referme.", "code": "Code de la serrure de la porte vitrée", "close": "Ces informations sont là pour rendre votre séjour plus agréable."}, "de": {"tab": "Eingang", "h": "Hinweise zur Eingangstür", "n": "Aus Sicherheitsgründen wird die Eingangstür des Gebäudes (1F) nach 23 Uhr geschlossen.", "t1": "Kommen Sie spät zurück?", "s1": "Öffnen Sie die Tür mit dem Türschloss.", "s2": "Drücken Sie danach den Schalter an der Innenseite der Tür, damit sich die Tür wieder schließt.", "code": "Code des Türschlosses der Glastür", "close": "Diese Hinweise dienen Ihrem angenehmen Aufenthalt."}};
  var PK = {"en": {"tab": "Pickup", "h": "Airport Pickup Service", "price": "Price", "pv": "About 90,000–100,000 KRW per van (1 vehicle).", "c": [["Tell us your flight number", "Please give us your flight number."], ["Tell us your messenger ID", "Give us the ID of the messenger app you use: WhatsApp, LINE, or KakaoTalk. The pickup driver will contact you there."], ["The driver will message you", "The driver will send you the exact fare and the pickup spot at the airport by messenger."]], "note": "We will pass your details to the pickup driver."}, "ko": {"tab": "픽업", "h": "공항 픽업 서비스 안내", "price": "요금", "pv": "승합차 1대 약 9~10만원", "c": [["비행기 편명을 알려주세요", "탑승하시는 비행기 편명을 알려주세요."], ["메신저 아이디를 알려주세요", "왓츠앱, 라인, 카카오톡 중 사용하시는 메신저 아이디를 알려주세요. 픽업 기사님이 그 메신저로 연락드립니다."], ["기사님이 연락드립니다", "정확한 요금과 공항에서 픽업 위치는 기사님이 메신저로 전달해 주실 거예요."]], "note": "알려주신 정보는 픽업 기사님께 전달해 드립니다."}, "ja": {"tab": "送迎", "h": "空港送迎サービスのご案内", "price": "料金", "pv": "ワゴン1台 約9〜10万ウォン", "c": [["フライト番号をお知らせください", "ご利用の便のフライト番号をお知らせください。"], ["メッセンジャーIDをお知らせください", "WhatsApp、LINE、カカオトークのうち、お使いのアプリのIDをお知らせください。送迎ドライバーがそちらからご連絡します。"], ["ドライバーからご連絡します", "正確な料金と空港での待ち合わせ場所は、ドライバーがメッセージでお知らせします。"]], "note": "お知らせいただいた情報は送迎ドライバーにお伝えします。"}, "zh-hans": {"tab": "接机", "h": "机场接送服务", "price": "费用", "pv": "每辆商务车约 9~10 万韩元", "c": [["请告知航班号", "请告诉我们您的航班号。"], ["请告知通讯软件账号", "请告诉我们您使用的通讯软件账号(WhatsApp、LINE 或 KakaoTalk)。接送司机会通过该软件联系您。"], ["司机会联系您", "准确的费用和机场接送地点,司机会通过通讯软件发给您。"]], "note": "我们会把您提供的信息转交给接送司机。"}, "zh-hant": {"tab": "接機", "h": "機場接送服務", "price": "費用", "pv": "每輛廂型車約 9~10 萬韓元", "c": [["請告知航班編號", "請告訴我們您的航班編號。"], ["請告知通訊軟體帳號", "請告訴我們您使用的通訊軟體帳號(WhatsApp、LINE 或 KakaoTalk)。接送司機會透過該軟體聯絡您。"], ["司機會聯絡您", "準確的費用和機場接送地點,司機會透過通訊軟體傳給您。"]], "note": "我們會將您提供的資訊轉交給接送司機。"}, "es": {"tab": "Recogida", "h": "Servicio de recogida en el aeropuerto", "price": "Precio", "pv": "Unos 90.000–100.000 KRW por furgoneta (1 vehículo).", "c": [["Indícanos tu número de vuelo", "Por favor, dinos tu número de vuelo."], ["Indícanos tu ID de mensajería", "Dinos tu ID de WhatsApp, LINE o KakaoTalk, según la que uses. El conductor se pondrá en contacto contigo por ahí."], ["El conductor te escribirá", "El conductor te enviará por mensaje la tarifa exacta y el punto de recogida en el aeropuerto."]], "note": "Transmitiremos tus datos al conductor."}, "fr": {"tab": "Navette", "h": "Service de transfert depuis l'aéroport", "price": "Tarif", "pv": "Environ 90 000 à 100 000 KRW par van (1 véhicule).", "c": [["Indiquez-nous votre numéro de vol", "Merci de nous communiquer votre numéro de vol."], ["Indiquez-nous votre identifiant de messagerie", "Donnez-nous votre identifiant WhatsApp, LINE ou KakaoTalk, selon celle que vous utilisez. Le chauffeur vous contactera par ce biais."], ["Le chauffeur vous écrira", "Le chauffeur vous enverra par message le tarif exact et le point de rendez-vous à l'aéroport."]], "note": "Nous transmettrons vos informations au chauffeur."}, "de": {"tab": "Abholung", "h": "Flughafen-Abholservice", "price": "Preis", "pv": "Etwa 90.000–100.000 KRW pro Van (1 Fahrzeug).", "c": [["Nennen Sie uns Ihre Flugnummer", "Bitte teilen Sie uns Ihre Flugnummer mit."], ["Nennen Sie uns Ihre Messenger-ID", "Teilen Sie uns Ihre ID bei WhatsApp, LINE oder KakaoTalk mit, je nachdem, was Sie nutzen. Der Fahrer meldet sich dort bei Ihnen."], ["Der Fahrer schreibt Ihnen", "Der Fahrer schickt Ihnen den genauen Fahrpreis und den Abholpunkt am Flughafen per Messenger."]], "note": "Wir leiten Ihre Angaben an den Fahrer weiter."}};
  var AP = {"en": {"tab": "Airport", "h": "From Incheon Airport", "bt": "Airport bus", "rows": [["Bus", "6001 / 6015"], ["Interval", "About every 20–25 minutes"], ["Get off at", "Sejong Hotel (Myeongdong Station)"], ["Fare", "Adults about 17,000 KRW. T-money cards accepted."]]}, "ko": {"tab": "공항", "h": "인천공항에서 오시는 길", "bt": "공항버스", "rows": [["버스", "6001번 / 6015번"], ["배차 간격", "약 20~25분"], ["하차 정류장", "명동역 세종호텔"], ["요금", "성인 약 17,000원 (T머니 카드 사용 가능)"]]}, "ja": {"tab": "空港", "h": "仁川空港からのアクセス", "bt": "空港バス", "rows": [["バス", "6001番 / 6015番"], ["運行間隔", "約20〜25分"], ["降りる停留所", "明洞駅 セジョンホテル"], ["料金", "大人 約17,000ウォン(T-moneyカード利用可)"]]}, "zh-hans": {"tab": "机场", "h": "从仁川机场出发", "bt": "机场巴士", "rows": [["巴士", "6001 路 / 6015 路"], ["发车间隔", "约 20~25 分钟"], ["下车站", "明洞站 世宗酒店"], ["费用", "成人约 17,000 韩元(可使用 T-money 卡)"]]}, "zh-hant": {"tab": "機場", "h": "從仁川機場出發", "bt": "機場巴士", "rows": [["巴士", "6001 號 / 6015 號"], ["發車間隔", "約 20~25 分鐘"], ["下車站", "明洞站 世宗飯店"], ["費用", "成人約 17,000 韓元(可使用 T-money 卡)"]]}, "es": {"tab": "Aeropuerto", "h": "Desde el aeropuerto de Incheon", "bt": "Autobús del aeropuerto", "rows": [["Autobús", "6001 / 6015"], ["Frecuencia", "Aproximadamente cada 20–25 minutos"], ["Bajada", "Hotel Sejong (estación de Myeongdong)"], ["Tarifa", "Adultos unos 17.000 KRW. Se acepta la tarjeta T-money."]]}, "fr": {"tab": "Aéroport", "h": "Depuis l'aéroport d'Incheon", "bt": "Bus aéroport", "rows": [["Bus", "6001 / 6015"], ["Fréquence", "Environ toutes les 20 à 25 minutes"], ["Descente", "Hôtel Sejong (station Myeongdong)"], ["Tarif", "Adulte environ 17 000 KRW. Carte T-money acceptée."]]}, "de": {"tab": "Flughafen", "h": "Vom Flughafen Incheon", "bt": "Flughafenbus", "rows": [["Bus", "6001 / 6015"], ["Takt", "Etwa alle 20–25 Minuten"], ["Aussteigen", "Sejong Hotel (Station Myeongdong)"], ["Fahrpreis", "Erwachsene etwa 17.000 KRW. T-money-Karte wird akzeptiert."]]}};
  var DIR = {"en": {"tab": "Directions", "h": "From Incheon Airport", "bt": "Airport bus", "bf": ["Buses 6001 and 6015 run about every 20–25 minutes.", "The bus stops at Sejong Hotel ([[세종호텔]]), near Myeongdong Station.", "Adult fare: about 17,000 KRW.", "T-money cards are accepted."], "at": "AREX Airport Railroad", "af": ["Adult fare: about 13,000 KRW."], "as": ["Take AREX to Seoul Station ([[서울역]]).", "Transfer to Line 4 at Seoul Station.", "Get off at Myeongdong Station ([[명동역]]) and take Exit 6."]}, "ko": {"tab": "오시는 길", "h": "인천공항에서 오시는 길", "bt": "공항버스", "bf": ["6001번, 6015번 버스가 약 20~25분 간격으로 다닙니다.", "명동역 근처 세종호텔([[세종호텔]])에 정차합니다.", "요금: 성인 약 17,000원", "T머니 카드를 사용할 수 있습니다."], "at": "AREX 공항철도", "af": ["요금: 성인 약 13,000원"], "as": ["AREX를 타고 서울역([[서울역]])으로 가세요.", "서울역에서 4호선으로 환승하세요.", "명동역([[명동역]])에서 내려 6번 출구로 나오세요."]}, "ja": {"tab": "アクセス", "h": "仁川空港からのアクセス", "bt": "空港バス", "bf": ["6001番・6015番のバスが約20〜25分間隔で運行しています。", "明洞駅近くの世宗ホテル([[세종호텔]])に停車します。", "料金:大人 約17,000ウォン", "T-moneyカードが使えます。"], "at": "AREX空港鉄道", "af": ["料金:大人 約13,000ウォン"], "as": ["AREXでソウル駅([[서울역]])まで行きます。", "ソウル駅で4号線に乗り換えます。", "明洞駅([[명동역]])で降りて、6番出口に出ます。"]}, "zh-hans": {"tab": "交通", "h": "从仁川机场出发", "bt": "机场大巴", "bf": ["6001 路和 6015 路大巴约每 20~25 分钟一班。", "大巴停靠在明洞站附近的世宗酒店([[세종호텔]])。", "票价:成人约 17,000 韩元", "可使用 T-money 卡。"], "at": "AREX 机场快线", "af": ["票价:成人约 13,000 韩元"], "as": ["乘坐 AREX 到首尔站([[서울역]])。", "在首尔站换乘 4 号线。", "在明洞站([[명동역]])下车,从 6 号出口出站。"]}, "zh-hant": {"tab": "交通", "h": "從仁川機場出發", "bt": "機場巴士", "bf": ["6001 號和 6015 號巴士約每 20~25 分鐘一班。", "巴士停靠在明洞站附近的世宗飯店([[세종호텔]])。", "票價:成人約 17,000 韓元", "可使用 T-money 卡。"], "at": "AREX 機場鐵路", "af": ["票價:成人約 13,000 韓元"], "as": ["搭乘 AREX 到首爾站([[서울역]])。", "在首爾站轉乘 4 號線。", "在明洞站([[명동역]])下車,從 6 號出口出站。"]}, "es": {"tab": "Cómo llegar", "h": "Desde el aeropuerto de Incheon", "bt": "Autobús del aeropuerto", "bf": ["Los autobuses 6001 y 6015 pasan aproximadamente cada 20–25 minutos.", "El autobús para en el Hotel Sejong ([[세종호텔]]), cerca de la estación de Myeongdong.", "Tarifa de adulto: unos 17.000 KRW.", "Se aceptan tarjetas T-money."], "at": "Tren AREX del aeropuerto", "af": ["Tarifa de adulto: unos 13.000 KRW."], "as": ["Toma el AREX hasta la estación de Seúl ([[서울역]]).", "Haz transbordo a la línea 4 en la estación de Seúl.", "Bájate en la estación de Myeongdong ([[명동역]]) y sal por la salida 6."]}, "fr": {"tab": "Accès", "h": "Depuis l'aéroport d'Incheon", "bt": "Bus de l'aéroport", "bf": ["Les bus 6001 et 6015 passent environ toutes les 20 à 25 minutes.", "Le bus s'arrête à l'hôtel Sejong ([[세종호텔]]), près de la station Myeongdong.", "Tarif adulte : environ 17 000 KRW.", "Les cartes T-money sont acceptées."], "at": "Train AREX de l'aéroport", "af": ["Tarif adulte : environ 13 000 KRW."], "as": ["Prenez l'AREX jusqu'à la gare de Séoul ([[서울역]]).", "Changez pour la ligne 4 à la gare de Séoul.", "Descendez à la station Myeongdong ([[명동역]]) et sortez par la sortie 6."]}, "de": {"tab": "Anreise", "h": "Vom Flughafen Incheon", "bt": "Flughafenbus", "bf": ["Die Busse 6001 und 6015 fahren etwa alle 20–25 Minuten.", "Der Bus hält am Sejong Hotel ([[세종호텔]]) in der Nähe der Station Myeongdong.", "Fahrpreis Erwachsene: ca. 17.000 KRW.", "T-money-Karten werden akzeptiert."], "at": "AREX Flughafenbahn", "af": ["Fahrpreis Erwachsene: ca. 13.000 KRW."], "as": ["Fahren Sie mit der AREX bis zum Bahnhof Seoul ([[서울역]]).", "Steigen Sie am Bahnhof Seoul in die Linie 4 um.", "Steigen Sie an der Station Myeongdong ([[명동역]]) aus und nehmen Sie Ausgang 6."]}};
  var ROUTE = {"en": {"t": "Walking from Exit 6 to our building", "c": ["Come out of Exit 6 and walk straight.", "Keep going straight on the main street.", "At the pink BANILA CO building, turn left.", "Walk down this alley.", "Turn right here, by the NYUNYU Girls building.", "Keep going straight along the alley with the benches.", "At the end of the alley, turn left (BRICKSAND is straight ahead).", "Keep going straight past the ginseng chicken soup ([[삼계탕]]) sign and the clinic.", "DAOL ([[다올]]) Korean BBQ is on the 1st floor of our building, on your left."]}, "ko": {"t": "6번 출구에서 숙소까지 걷는 길", "c": ["6번 출구로 나와서 직진하세요.", "큰 길을 따라 계속 직진하세요.", "분홍색 BANILA CO(바닐라코) 건물에서 좌회전하세요.", "이 골목으로 걸어가세요.", "NYUNYU Girls 건물 옆에서 우회전하세요.", "벤치가 있는 골목을 따라 앞으로 쭉 가세요.", "골목 끝에서 좌회전하세요. (정면에 BRICKSAND가 보입니다.)", "삼계탕 간판과 의원을 지나 계속 직진하세요.", "저희 건물 1층에는 다올 숯불구이(DAOL)가 있습니다. 왼쪽에 보이는 건물이에요."]}, "ja": {"t": "6番出口から宿まで歩く道順", "c": ["6番出口を出て、まっすぐ進みます。", "大通りをそのまままっすぐ進みます。", "ピンク色のBANILA CO(バニラコ)の建物で左に曲がります。", "この路地を進みます。", "NYUNYU Girlsの建物のそばで右に曲がります。", "ベンチのある路地をまっすぐ進みます。", "路地の突き当たりで左に曲がります(正面にBRICKSANDが見えます)。", "参鶏湯([[삼계탕]])の看板とクリニックを過ぎて、まっすぐ進みます。", "当館の1階には韓国式焼肉店「DAOL([[다올]])」があります。左側の建物です。"]}, "zh-hans": {"t": "从 6 号出口步行到我们的住宿", "c": ["从 6 号出口出来后直走。", "沿着大街继续直走。", "在粉色的 BANILA CO(芭妮兰)大楼处左转。", "走进这条小巷。", "在 NYUNYU Girls 大楼旁右转。", "沿着有长椅的小巷一直往前走。", "走到小巷尽头左转(正前方是 BRICKSAND)。", "经过参鸡汤([[삼계탕]])招牌和诊所,继续直走。", "我们大楼的一楼是 DAOL([[다올]])韩式烤肉店,就在您的左手边。"]}, "zh-hant": {"t": "從 6 號出口步行到我們的住宿", "c": ["從 6 號出口出來後直走。", "沿著大街繼續直走。", "在粉色的 BANILA CO(芭妮蘭)大樓處左轉。", "走進這條小巷。", "在 NYUNYU Girls 大樓旁右轉。", "沿著有長椅的小巷一直往前走。", "走到小巷盡頭左轉(正前方是 BRICKSAND)。", "經過蔘雞湯([[삼계탕]])招牌和診所,繼續直走。", "我們大樓的一樓是 DAOL([[다올]])韓式烤肉店,就在您的左手邊。"]}, "es": {"t": "A pie desde la salida 6 hasta nuestro alojamiento", "c": ["Sal por la salida 6 y sigue recto.", "Sigue recto por la calle principal.", "En el edificio rosa BANILA CO, gira a la izquierda.", "Camina por este callejón.", "Gira a la derecha aquí, junto al edificio NYUNYU Girls.", "Sigue recto por el callejón de los bancos.", "Al final del callejón, gira a la izquierda (BRICKSAND queda justo enfrente).", "Sigue recto, pasando el cartel de samgyetang ([[삼계탕]]) y la clínica.", "En la planta baja (1F) de nuestro edificio está el restaurante de barbacoa coreana DAOL ([[다올]]), a tu izquierda."]}, "fr": {"t": "À pied, de la sortie 6 jusqu'à notre logement", "c": ["Sortez par la sortie 6 et allez tout droit.", "Continuez tout droit sur la grande rue.", "Au bâtiment rose BANILA CO, tournez à gauche.", "Engagez-vous dans cette ruelle.", "Tournez à droite ici, près du bâtiment NYUNYU Girls.", "Continuez tout droit le long de la ruelle avec les bancs.", "Au bout de la ruelle, tournez à gauche (BRICKSAND est juste en face).", "Continuez tout droit, en passant devant l'enseigne de samgyetang ([[삼계탕]]) et la clinique.", "Au rez-de-chaussée (1F) de notre immeuble se trouve le restaurant de barbecue coréen DAOL ([[다올]]), sur votre gauche."]}, "de": {"t": "Zu Fuß von Ausgang 6 zu unserer Unterkunft", "c": ["Verlassen Sie Ausgang 6 und gehen Sie geradeaus.", "Gehen Sie auf der Hauptstraße weiter geradeaus.", "Biegen Sie am rosa Gebäude BANILA CO links ab.", "Gehen Sie in diese Gasse hinein.", "Biegen Sie hier, am Gebäude NYUNYU Girls, rechts ab.", "Gehen Sie in der Gasse mit den Bänken weiter geradeaus.", "Biegen Sie am Ende der Gasse links ab (geradeaus sehen Sie BRICKSAND).", "Gehen Sie geradeaus, vorbei am Schild für Samgyetang ([[삼계탕]]) und der Klinik.", "Im Erdgeschoss (1F) unseres Gebäudes befindet sich das koreanische BBQ-Restaurant DAOL ([[다올]]), auf Ihrer linken Seite."]}};
  var ROUTEDIM = [[900, 778], [900, 782], [900, 707], [900, 791], [900, 684], [900, 824], [900, 678], [900, 706], [900, 799]];
  var HTML_LANG = { en: "en", ko: "ko", ja: "ja", "zh-hans": "zh-Hans", "zh-hant": "zh-Hant", es: "es", fr: "fr", de: "de" };
  var TOPICS = ["wifi", "door", "tv", "ac", "washer", "food", "trash", "pickup", "route"];
  var cur = { topic: "wifi", lang: "en" };

  function rich(e, text) {
    text.split(/(\[\[.+?\]\]|\{pp\})/).forEach(function (p) {
      if (!p) return;
      var s;
      if (p === "{pp}") { s = document.createElement("span"); s.className = "chip"; s.textContent = "▶︎II"; e.appendChild(s); }
      else if (p.indexOf("[[") === 0) { s = document.createElement("span"); s.className = "chip"; s.lang = "ko"; s.textContent = p.slice(2, -2); e.appendChild(s); }
      else e.appendChild(document.createTextNode(p));
    });
  }
  function el(tag, cls, text) {
    var e = document.createElement(tag);
    if (cls) e.className = cls;
    if (text != null) rich(e, text);
    return e;
  }
  function photo(v, file, alt, w, h) {
    var ph = document.createElement("img");
    ph.className = "photo"; ph.src = file; ph.alt = alt; ph.width = w; ph.height = h;
    v.appendChild(ph);
  }
  function steps(list, alt) {
    var box = el("div", "list");
    list.forEach(function (s, i) {
      var c = el("div", "card step");
      c.appendChild(el("span", "n" + (alt ? " alt" : ""), String(i + 1)));
      var b = el("div");
      b.appendChild(el("h3", null, s[0]));
      b.appendChild(el("p", null, s[1]));
      c.appendChild(b);
      box.appendChild(c);
    });
    return box;
  }
  function markList(items, mark) {
    var ul = el("ul", "items");
    items.forEach(function (t) {
      var li = el("li");
      li.appendChild(el("span", "mk", mark));
      li.appendChild(el("span", null, t));
      ul.appendChild(li);
    });
    return ul;
  }

  function renderTv(d, v) {
    v.appendChild(el("h1", null, d.h));
    photo(v, "tv.jpg", d.h, 1122, 1402);
    var card = el("div", "card tv");
    var wrap = el("div", "remote");
    wrap.innerHTML = REMOTE;
    var svg = wrap.firstChild;
    svg.setAttribute("aria-label", d.alt);
    card.appendChild(wrap);
    var ol = el("ol", "legend");
    d.items.forEach(function (it, i) {
      var li = el("li");
      li.appendChild(el("span", "n", String(i + 1)));
      var b = el("div");
      b.appendChild(el("b", null, it[0]));
      b.appendChild(el("span", "d", it[1]));
      li.appendChild(b);
      ol.appendChild(li);
    });
    card.appendChild(ol);
    v.appendChild(card);
  }
  function copyTo(btn, node, text, w) {
    function done() { btn.textContent = w.copied; setTimeout(function () { btn.textContent = w.copy; }, 1500); }
    function fb() {
      try { var r = document.createRange(); r.selectNodeContents(node); var sel = window.getSelection(); sel.removeAllRanges(); sel.addRange(r); } catch (e) {}
    }
    try { navigator.clipboard.writeText(text).then(done, fb); } catch (e) { fb(); }
  }
  function renderWifi(w, v) {
    v.appendChild(el("h1", null, w.h));
    v.appendChild(el("p", "sub", w.sub));
    photo(v, "wifi.jpg", w.h, 1214, 1295);
    [["2.4GHz", "KT_GiGA_F18A", false], ["5GHz", "KT_GiGA_5G_F18A", false], ["Mesh", "KT_GiGA_Mesh_F18A", false], ["PW", "9gc19ce777", true]].forEach(function (r) {
      var c = el("div", "card net");
      c.appendChild(el("span", "band" + (r[2] ? " pw" : ""), r[0]));
      var b = el("div");
      b.appendChild(el("span", "lab", r[2] ? w.pw : w.ssid));
      var val = el("span", "val", r[1]);
      b.appendChild(val);
      c.appendChild(b);
      var btn = el("button", "copy", w.copy);
      btn.type = "button";
      btn.addEventListener("click", function () { copyTo(btn, val, r[1], w); });
      c.appendChild(btn);
      v.appendChild(c);
    });
    var q = el("div", "card quick");
    q.appendChild(el("p", null, w.note));
    v.appendChild(q);
    v.appendChild(el("p", "help", w.free + " " + w.help));
  }
  var ICONS = {gen: '<svg viewBox="0 0 64 72" width="64" height="72" aria-hidden="true"><path d="M20 17C10 23 6 37 8 54c1 10 6 14 24 14s23-4 24-14c2-17-2-31-12-37z" fill="#ffffff" stroke="#6b7a89" stroke-width="2"/><path d="M26 17c-2-9 2-13 6-11 4-2 8 2 6 11" fill="#ffffff" stroke="#6b7a89" stroke-width="2"/><rect x="15" y="29" width="34" height="15" rx="2" fill="#e8f0fb" stroke="#2a5fa8" stroke-width="1.2"/><text x="32" y="37" text-anchor="middle" dominant-baseline="central" font-family="sans-serif" font-weight="700" font-size="8" fill="#2a5fa8">종량제</text><path d="M16 50h32M19 56h26" stroke="#9aa9b8" stroke-width="1.6" stroke-linecap="round"/></svg>', food: '<svg viewBox="0 0 64 72" width="64" height="72" aria-hidden="true"><rect x="14" y="27" width="36" height="39" rx="6" fill="#f2c230" stroke="#9a7a0a" stroke-width="2"/><rect x="10" y="19" width="44" height="10" rx="4" fill="#f7d768" stroke="#9a7a0a" stroke-width="2"/><path d="M32 36c-6 3-6 11 0 14 6-3 6-11 0-14z" fill="#fff4c2" stroke="#9a7a0a" stroke-width="1.5"/></svg>', rec: '<svg viewBox="0 0 64 72" width="64" height="72" aria-hidden="true"><path d="M20 17C10 23 6 37 8 54c1 10 6 14 24 14s23-4 24-14c2-17-2-31-12-37z" fill="#ffffff" stroke="#6b7a89" stroke-width="2"/><path d="M26 17c-2-9 2-13 6-11 4-2 8 2 6 11" fill="#ffffff" stroke="#6b7a89" stroke-width="2"/><path d="M17 32c-2 9-1 18 2 26" fill="none" stroke="#d7e0e9" stroke-width="2.5" stroke-linecap="round"/></svg>'};
  function renderTrash(t, v) {
    v.appendChild(el("h1", null, t.h));
    v.appendChild(el("p", null, t.intro));
    var box = el("div", "list");
    [["gen", t.gen], ["food", t.food], ["rec", t.rec]].forEach(function (r) {
      var c = el("div", "card step big");
      var ic = el("div", "ic");
      ic.innerHTML = ICONS[r[0]];
      c.appendChild(ic);
      var b = el("div");
      b.appendChild(el("h3", null, r[1][0]));
      b.appendChild(el("p", null, r[1][1]));
      c.appendChild(b);
      box.appendChild(c);
    });
    v.appendChild(box);
    var bag = el("div", "card");
    bag.appendChild(el("h3", null, t.bagsT));
    bag.appendChild(el("p", null, t.bags));
    v.appendChild(bag);
    var b2 = BIN[cur.lang];
    var bc = el("div", "card");
    bc.appendChild(el("h3", null, b2.binT));
    var bi = document.createElement("img");
    bi.className = "photo"; bi.src = "bins.jpg"; bi.alt = b2.binT; bi.width = 512; bi.height = 512;
    bi.style.margin = "8px 0";
    bc.appendChild(bi);
    bc.appendChild(el("p", null, b2.bin));
    bc.appendChild(el("p", null, b2.full));
    v.appendChild(bc);
    var dr = DROP[cur.lang];
    var dc = el("div", "card");
    dc.appendChild(el("h3", null, dr.t));
    var dl = el("div", "drops");
    dr.c.forEach(function (cap, i) {
      var f = el("figure", "drop");
      var di = document.createElement("img");
      di.className = "photo"; di.src = "drop" + (i + 1) + ".jpg"; di.alt = cap;
      di.width = DROPDIM[i][0]; di.height = DROPDIM[i][1];
      f.appendChild(di);
      var fc = el("figcaption", "step");
      fc.appendChild(el("span", "n", String(i + 1)));
      fc.appendChild(el("span", null, cap));
      f.appendChild(fc);
      dl.appendChild(f);
    });
    dc.appendChild(dl);
    v.appendChild(dc);
    var rc = el("div", "card quick");
    rc.appendChild(el("h3", null, t.rulesT));
    var ul = el("ul", "rules");
    ul.appendChild(el("li", null, t.n1));
    ul.appendChild(el("li", null, t.n2));
    rc.appendChild(ul);
    v.appendChild(rc);
    v.appendChild(el("p", "help", t.thanks));
  }
  function renderDoor(d, v) {
    v.appendChild(el("h1", null, d.h));
    var n = el("div", "card quick");
    n.appendChild(el("p", null, d.n));
    v.appendChild(n);
    var c = el("div", "card step");
    c.appendChild(el("span", "n", "1"));
    var b = el("div");
    b.appendChild(el("h3", null, d.t1));
    b.appendChild(el("p", null, d.s1));
    c.appendChild(b);
    v.appendChild(c);
    var c2 = el("div", "card step");
    c2.appendChild(el("span", "n", "2"));
    var b2 = el("div");
    b2.appendChild(el("p", null, d.s2));
    c2.appendChild(b2);
    v.appendChild(c2);
    v.appendChild(el("p", "help", d.close));
  }
  function renderPickup(k, v) {
    var a = AP[cur.lang];
    v.appendChild(el("h1", null, a.h));
    v.appendChild(el("h2", "sec", a.bt));
    var bc = el("div", "card kv");
    a.rows.forEach(function (r) {
      var row = el("div");
      row.appendChild(el("span", "k", r[0]));
      row.appendChild(el("span", "vv", r[1]));
      bc.appendChild(row);
    });
    v.appendChild(bc);
    v.appendChild(el("h2", "sec", k.h));
    var pc = el("div", "card quick");
    pc.appendChild(el("h3", null, k.price));
    pc.appendChild(el("p", "big", k.pv));
    v.appendChild(pc);
    v.appendChild(steps(k.c, false));
    v.appendChild(el("p", "help", k.note));
  }
  function renderRoute(k, v) {
    v.appendChild(el("h1", null, k.h));
    var bc = el("div", "card");
    var bh = el("h3", null, k.bt + " ");
    ["6001", "6015"].forEach(function (n) { bh.appendChild(el("span", "chip", n)); bh.appendChild(document.createTextNode(" ")); });
    bc.appendChild(bh);
    var ul = el("ul", "rules");
    k.bf.forEach(function (t) { ul.appendChild(el("li", null, t)); });
    bc.appendChild(ul);
    v.appendChild(bc);
    var ac = el("div", "card");
    ac.appendChild(el("h3", null, k.at));
    var ul2 = el("ul", "rules");
    k.af.forEach(function (t) { ul2.appendChild(el("li", null, t)); });
    ac.appendChild(ul2);
    var sl = el("div", "list");
    sl.style.marginTop = "12px";
    k.as.forEach(function (t, i) {
      var r = el("div", "step");
      r.appendChild(el("span", "n alt", String(i + 1)));
      r.appendChild(el("span", null, t));
      sl.appendChild(r);
    });
    ac.appendChild(sl);
    v.appendChild(ac);
    var rt = ROUTE[cur.lang];
    var rc = el("div", "card");
    rc.appendChild(el("h3", null, rt.t));
    var rl = el("div", "drops");
    rt.c.forEach(function (cap, i) {
      var f = el("figure", "drop");
      var ri = document.createElement("img");
      ri.className = "photo"; ri.src = "route" + (i + 1) + ".jpg"; ri.alt = cap.replace(/\[\[|\]\]/g, "");
      ri.width = ROUTEDIM[i][0]; ri.height = ROUTEDIM[i][1];
      f.appendChild(ri);
      var fc = el("figcaption", "step");
      fc.appendChild(el("span", "n", String(i + 1)));
      fc.appendChild(el("span", null, cap));
      f.appendChild(fc);
      rl.appendChild(f);
    });
    rc.appendChild(rl);
    v.appendChild(rc);
  }
  function renderAc(d, v) {
    v.appendChild(el("h1", null, d.h));
    photo(v, "ac.jpg", d.h, 1080, 1073);
    var q = el("div", "card quick");
    q.appendChild(el("h3", null, d.qt));
    q.appendChild(el("p", null, d.qb));
    v.appendChild(q);
    var card = el("div", "card");
    var ol = el("ol", "legend");
    d.items.forEach(function (it, i) {
      var li = el("li");
      li.appendChild(el("span", "n", String(i + 1)));
      var b = el("div");
      b.appendChild(el("b", null, it[0]));
      var dd = el("span", "d", it[1]);
      b.appendChild(dd);
      li.appendChild(b);
      ol.appendChild(li);
    });
    card.appendChild(ol);
    v.appendChild(card);
  }
  function renderWasher(d, v) {
    v.appendChild(el("h1", null, d.h));
    photo(v, "washer.jpg", d.h, 1223, 1286);
    v.appendChild(el("h2", "sec", d.wt));
    v.appendChild(steps(d.steps, false));
    v.appendChild(el("h2", "sec", d.dt));
    v.appendChild(steps(d.dsteps, true));
    var imp = el("div", "card important");
    imp.appendChild(el("span", "n", "!"));
    var b = el("div");
    b.appendChild(el("h3", null, d.it));
    b.appendChild(el("p", "big", d.ib));
    b.appendChild(el("p", null, d.id));
    imp.appendChild(b);
    v.appendChild(imp);
  }
  function renderFood(d, v) {
    v.appendChild(el("h1", null, d.h));
    v.appendChild(el("p", "sub", d.sub));
    photo(v, "food.jpg", d.h, 1223, 1286);
    v.appendChild(steps(d.steps, false));
    var two = el("div", "two");
    var y = el("div", "card yes");
    y.appendChild(el("h3", null, d.okT));
    y.appendChild(el("p", "hint", d.okS));
    y.appendChild(markList(d.ok, "✓"));
    var n = el("div", "card nay");
    n.appendChild(el("h3", null, d.noT));
    n.appendChild(el("p", "hint", d.noS));
    n.appendChild(markList(d.no, "✕"));
    two.appendChild(y);
    two.appendChild(n);
    v.appendChild(two);
  }

  function apply(state) {
    cur = state;
    var d = T[state.lang];
    document.documentElement.lang = HTML_LANG[state.lang];
    var v = document.getElementById("view");
    v.textContent = "";
    if (state.topic === "wifi") renderWifi(WF[state.lang], v);
    else if (state.topic === "door") renderDoor(DOOR[state.lang], v);
    else if (state.topic === "tv") renderTv(d.tv, v);
    else if (state.topic === "ac") renderAc(d.a, v);
    else if (state.topic === "washer") renderWasher(d.w, v);
    else if (state.topic === "trash") renderTrash(TR[state.lang], v);
    else if (state.topic === "pickup") renderPickup(PK[state.lang], v);
    else if (state.topic === "route") renderRoute(DIR[state.lang], v);
    else renderFood(d.f, v);
    document.querySelectorAll("#tabs button").forEach(function (b, i) {
      b.textContent = [WF[state.lang].tab, DOOR[state.lang].tab].concat(d.tabs, [TR[state.lang].tab, PK[state.lang].tab, DIR[state.lang].tab])[i];
      b.setAttribute("aria-pressed", b.getAttribute("data-topic") === state.topic ? "true" : "false");
    });
    document.querySelectorAll("#langs button").forEach(function (b) {
      b.setAttribute("aria-pressed", b.getAttribute("data-lang") === state.lang ? "true" : "false");
    });
    try { localStorage.setItem("guide-lang", state.lang); } catch (e) {}
  }

  function parse() {
    var h = (location.hash || "").replace("#", "");
    var topic = "wifi";
    for (var i = 0; i < TOPICS.length; i++) {
      if (h === TOPICS[i]) { topic = TOPICS[i]; h = ""; break; }
      if (h.indexOf(TOPICS[i] + "-") === 0) { topic = TOPICS[i]; h = h.slice(TOPICS[i].length + 1); break; }
    }
    var lang = T[h] ? h : null;
    if (!lang) { try { var s = localStorage.getItem("guide-lang"); if (T[s]) lang = s; } catch (e) {} }
    if (!lang) {
      var n = (navigator.language || "en").toLowerCase();
      lang = n.indexOf("ko") === 0 ? "ko" : n.indexOf("ja") === 0 ? "ja"
        : n.indexOf("zh") === 0 ? (/tw|hk|mo|hant/.test(n) ? "zh-hant" : "zh-hans")
        : n.indexOf("es") === 0 ? "es" : n.indexOf("fr") === 0 ? "fr" : n.indexOf("de") === 0 ? "de" : "en";
    }
    return { topic: topic, lang: lang };
  }
  function go(topic, lang) {
    var h = "#" + topic + "-" + lang;
    if (location.hash === h) apply({ topic: topic, lang: lang }); else location.hash = h;
  }

  document.getElementById("langs").addEventListener("click", function (e) {
    var b = e.target.closest("button[data-lang]");
    if (b) go(cur.topic, b.getAttribute("data-lang"));
  });
  document.getElementById("tabs").addEventListener("click", function (e) {
    var b = e.target.closest("button[data-topic]");
    if (b) go(b.getAttribute("data-topic"), cur.lang);
  });
  window.addEventListener("hashchange", function () { apply(parse()); });
  apply(parse());
})();
</script>

</body>
</html>
