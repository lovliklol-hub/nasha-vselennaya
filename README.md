<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#111116">
<title>Наша маленькая вселенная</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Montserrat:wght@300;400;500;600&display=swap');
:root{--bg:#101014;--panel:#1b1b23;--panel2:#24242e;--text:#eeeaf0;--muted:#aaa3af;--accent:#854456;--accent2:#40577c;--line:#ffffff20;--paper:#e9dfe3;--ink:#29212a}
*{box-sizing:border-box}html{scroll-behavior:smooth}body{margin:0;background:radial-gradient(ellipse at 15% 10%,#34435a55,transparent 38%),radial-gradient(ellipse at 85% 50%,#78374630,transparent 40%),var(--bg);color:var(--text);font-family:Montserrat,Arial,sans-serif;min-height:100vh}button,input,textarea{font:inherit}button{cursor:pointer}a{color:inherit;text-decoration:none}.stars{position:fixed;inset:0;pointer-events:none;z-index:0;overflow:hidden}.star{position:absolute;color:#ffffff80;animation:twinkle 3s infinite alternate}@keyframes twinkle{to{opacity:.2;transform:scale(.6)}}@keyframes rise{from{opacity:0;transform:translateY(18px)}to{opacity:1;transform:translateY(0)}}@keyframes float{50%{transform:translateY(-9px)}}@keyframes pulse{50%{transform:scale(1.12)}}header,main,footer{position:relative;z-index:1}.topbar{position:sticky;top:0;z-index:10;background:#101014df;backdrop-filter:blur(14px);border-bottom:1px solid var(--line);padding:12px 4%;display:flex;align-items:center;justify-content:space-between;gap:12px}.brand{font-family:'Cormorant Garamond',serif;font-size:23px;color:#d5b7c2}.nav{display:flex;gap:16px;flex-wrap:wrap;justify-content:center}.nav a{font-size:10px;letter-spacing:1px;color:var(--muted)}.nav a:hover{color:#fff}.top-actions{display:flex;gap:8px}.wrap{width:min(1080px,91%);margin:auto}.hero{min-height:88vh;display:grid;place-items:center;text-align:center;padding:80px 16px}.hero-inner{max-width:760px;animation:rise 1s ease}.eyebrow{font-size:10px;letter-spacing:5px;color:#c08b9d}.hero h1{font:500 clamp(54px,10vw,105px)/.95 'Cormorant Garamond',serif;margin:24px 0}.hero h1 em{color:#a86b80}.hero p{max-width:520px;margin:0 auto 28px;color:var(--muted);font-size:13px;line-height:2}.heart-big{font-size:30px;color:#a66c80;display:inline-block;animation:float 3s infinite}.btn{border:1px solid #986174;background:#71374655;color:var(--text);padding:11px 17px;border-radius:3px;font-size:11px;letter-spacing:1px;transition:.25s}.btn:hover{background:var(--accent);transform:translateY(-2px)}.btn.blue{border-color:#647da5;background:#344b7055}.btn.ghost{background:transparent;border-color:var(--line)}.btn.danger{border-color:#9c5555;background:#672e36}.section{padding:78px 0;scroll-margin-top:65px}.section-title{text-align:center;font:500 clamp(36px,6vw,56px) 'Cormorant Garamond',serif;margin:0 0 10px}.subtitle{text-align:center;color:var(--muted);font-size:12px;line-height:1.8;margin:0 auto 34px;max-width:620px}.orn{text-align:center;color:#a66c80;letter-spacing:9px;margin-bottom:18px}.panel{background:#ffffff09;border:1px solid var(--line);padding:25px;border-radius:4px;backdrop-filter:blur(8px)}.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:16px}.two{display:grid;grid-template-columns:1fr 1fr;gap:20px;align-items:center}.muted{color:var(--muted)}.small{font-size:11px;line-height:1.8}.display{font:500 31px 'Cormorant Garamond',serif;color:#d7bdc7}.counter{font:500 44px 'Cormorant Garamond',serif;color:#d5aaba}.field{width:100%;background:#111117;color:var(--text);border:1px solid var(--line);padding:11px;border-radius:3px;margin:6px 0 12px;outline:none}.field:focus{border-color:#986174}textarea.field{min-height:100px;resize:vertical}.upload{border:1px dashed #8a5a6d;padding:20px;text-align:center;margin:18px 0;color:var(--muted);font-size:12px}.upload input{display:none}.upload label{display:inline-block;margin-top:10px}.item{background:#22222b;border:1px solid var(--line);padding:12px;animation:rise .4s ease;min-width:0}.item img,.item video{width:100%;max-height:320px;object-fit:contain;background:#09090c;display:block}.item audio{width:100%;margin-top:10px}.item-title{font:500 23px 'Cormorant Garamond',serif;margin:8px 0}.item p{white-space:pre-wrap;line-height:1.7;font-size:12px;color:#c6c0c9}.item-actions{display:flex;gap:7px;flex-wrap:wrap;margin-top:10px}.item-actions button{font-size:10px;padding:7px 9px}.memory{border-top:2px solid var(--accent);background:#ffffff09;padding:20px}.memory:nth-child(even){border-color:var(--accent2)}.memory h3{font:500 25px 'Cormorant Garamond',serif;margin:0 0 8px}.card{height:220px;perspective:1000px;cursor:pointer}.card-inner{position:relative;width:100%;height:100%;transition:transform .7s;transform-style:preserve-3d}.card.flipped .card-inner{transform:rotateY(180deg)}.card-face{position:absolute;inset:0;backface-visibility:hidden;display:grid;place-items:center;text-align:center;padding:22px;background:linear-gradient(145deg,#37303b,#20232f);border:1px solid #80566a}.card-face.back{transform:rotateY(180deg);background:linear-gradient(145deg,#28364c,#24212a);border-color:#52698c}.card-face h3{font:500 27px 'Cormorant Garamond',serif}.card-face p{font-size:12px;line-height:1.8}.envelope{font-size:76px;cursor:pointer;display:inline-block;animation:float 3s infinite}.letter{display:none;background:var(--paper);color:var(--ink);font:20px/1.9 'Cormorant Garamond',serif;padding:28px;white-space:pre-wrap;margin-top:20px;text-align:left}.letter.show{display:block;animation:rise .5s}.reason-box{min-height:115px;display:grid;place-items:center;text-align:center;font:26px/1.5 'Cormorant Garamond',serif;padding:20px;color:#e1c5ce}.heart-button{font-size:40px;border:0;background:transparent;color:#bd748c;animation:pulse 2s infinite}.secret{display:none}.secret.show{display:block;animation:rise .5s}.toolbar{display:flex;gap:8px;flex-wrap:wrap;justify-content:center;margin:15px 0}.modal{position:fixed;inset:0;z-index:30;background:#050508dd;display:none;place-items:center;padding:18px}.modal.show{display:grid}.modal-box{width:min(520px,100%);max-height:90vh;overflow:auto;background:#202029;border:1px solid #86576a;padding:24px;position:relative}.modal-close{position:absolute;right:12px;top:10px;background:none;border:0;color:white;font-size:23px}.toast{position:fixed;bottom:20px;left:50%;transform:translateX(-50%);background:#29242e;border:1px solid #8c5b70;padding:12px 18px;z-index:50;font-size:12px;display:none}.toast.show{display:block;animation:rise .3s}.footer{text-align:center;border-top:1px solid var(--line);padding:40px 15px;color:var(--muted);font-size:10px;letter-spacing:2px}.hidden{display:none!important}
body.light{--bg:#d9d5d9;--panel:#e9e4e8;--panel2:#d4cdd4;--text:#29242c;--muted:#665e68;--line:#30233030;background:radial-gradient(ellipse at 15% 10%,#9eafc855,transparent 38%),radial-gradient(ellipse at 85% 50%,#b98a9930,transparent 40%),var(--bg)}body.light .topbar{background:#e5e0e5e8}body.light .item,body.light .memory{background:#ffffff80}body.light .field{background:#f8f5f8;color:#29242c}
@media(max-width:760px){.topbar{flex-wrap:wrap;justify-content:center}.brand{width:100%;text-align:center}.nav{gap:10px}.nav a{font-size:9px}.two{grid-template-columns:1fr}.section{padding:60px 0}.hero{min-height:82vh}.panel{padding:19px}}
</style>
</head>
<body>
<div class="stars" id="stars"></div>
<header class="topbar">
  <div class="brand">♡ наша вселенная</div>
  <nav class="nav">
    <a href="#home">ГЛАВНАЯ</a><a href="#about">О НАС</a><a href="#archive">АРХИВ</a><a href="#diary">ДНЕВНИК</a><a href="#music">МУЗЫКА</a><a href="#postcards">ОТКРЫТКИ</a><a href="#secret-room">СЕКРЕТЫ</a>
  </nav>
  <div class="top-actions"><button class="btn ghost" id="themeBtn">◐ ТЕМА</button><button class="btn ghost" id="settingsBtn">⚙</button></div>
</header>

<main>
<section class="hero" id="home"><div class="hero-inner">
  <div class="eyebrow">ЛИЧНЫЙ АРХИВ НАШЕЙ ДРУЖБЫ</div>
  <h1 id="heroTitle">Ты — часть<br><em>моей истории.</em></h1>
  <div class="heart-big">♡</div>
  <p id="heroText">Здесь живут наши фотографии, смешные истории, любимые песни и маленькие секреты. Добро пожаловать в наше особенное место.</p>
  <div class="toolbar"><a class="btn" href="#about">ВОЙТИ В НАШ МИР ↓</a><button class="btn blue" id="randomHeart">♡ СЛУЧАЙНОЕ ПОСЛАНИЕ</button></div>
  <div class="small muted" id="friendCounter">Наша история начинается здесь</div>
</div></section>

<section class="section" id="about"><div class="wrap">
  <div class="orn">✦ ♡ ✦</div><h2 class="section-title">Немного о нас</h2><p class="subtitle">Некоторые люди становятся воспоминанием. А некоторые — целым миром.</p>
  <div class="two">
    <div class="panel"><div class="display" id="aboutHeading">Для самого дорогого человека</div><p class="small muted" id="aboutCopy">Этот сайт — маленькая коллекция всего, что делает нашу дружбу особенной. Здесь можно смеяться, вспоминать, перечитывать письма и находить сюрпризы.</p><button class="btn" id="editAbout">ИЗМЕНИТЬ ТЕКСТ</button></div>
    <div class="panel" style="text-align:center"><div class="counter" id="daysCount">♡</div><div class="small muted">дней нашей дружбы</div><p class="small muted">Установи дату знакомства в настройках.</p><button class="btn blue" id="setDate">УСТАНОВИТЬ ДАТУ</button></div>
  </div>
</div></section>

<section class="section" id="archive"><div class="wrap">
  <div class="orn">✧</div><h2 class="section-title">Архив воспоминаний</h2><p class="subtitle">Фотографии и видео, которые хочется сохранить.</p>
  <div class="panel">
    <h3 class="display">Фотогалерея</h3><div class="upload"><p>Выбери фотографии с устройства. Они сохранятся в этом браузере.</p><label class="btn" for="photoFiles">＋ ДОБАВИТЬ ФОТО</label><input id="photoFiles" type="file" accept="image/*" multiple></div>
    <div class="grid" id="photoGrid"></div>
    <hr style="border:0;border-top:1px solid var(--line);margin:28px 0">
    <h3 class="display">Видеоархив</h3><div class="upload"><p>Добавь видео с устройства.</p><label class="btn blue" for="videoFiles">＋ ДОБАВИТЬ ВИДЕО</label><input id="videoFiles" type="file" accept="video/*" multiple></div>
    <div class="grid" id="videoGrid"></div>
  </div>
</div></section>

<section class="section" id="diary"><div class="wrap">
  <div class="orn">♡</div><h2 class="section-title">Наш дневник</h2><p class="subtitle">Записывай истории, даты, мысли и моменты, которые нельзя потерять.</p>
  <div class="panel"><div class="two">
    <div><label class="small">Название записи</label><input class="field" id="memoryTitle" placeholder="Например: тот самый вечер..."></div>
    <div><label class="small">Дата (необязательно)</label><input class="field" id="memoryDate" type="date"></div>
  </div><label class="small">Твоя история</label><textarea class="field" id="memoryText" placeholder="Расскажи, что произошло..."></textarea><button class="btn" id="saveMemory">СОХРАНИТЬ В ДНЕВНИК</button></div>
  <div class="grid" id="memoryGrid" style="margin-top:18px"></div>
</div></section>

<section class="section" id="music"><div class="wrap">
  <div class="orn">♫</div><h2 class="section-title">Музыкальная комната</h2><p class="subtitle">Песни, которые напоминают о людях, местах и моментах.</p>
  <div class="panel"><div class="upload"><p>Добавь аудиофайлы с устройства. Воспроизведение доступно прямо здесь.</p><label class="btn" for="audioFiles">♫ ДОБАВИТЬ МУЗЫКУ</label><input id="audioFiles" type="file" accept="audio/*" multiple></div><div class="grid" id="audioGrid"></div></div>
</div></section>

<section class="section" id="postcards"><div class="wrap">
  <div class="orn">✧ ♡ ✧</div><h2 class="section-title">Комната открыток</h2><p class="subtitle">Нажми на открытку, чтобы перевернуть её. Можно создавать собственные.</p>
  <div class="toolbar"><button class="btn" id="newCard">＋ СОЗДАТЬ ОТКРЫТКУ</button></div><div class="grid" id="cardGrid"></div>
</div></section>

<section class="section" id="reasons"><div class="wrap">
  <div class="orn">♡</div><h2 class="section-title">Причины ценить тебя</h2><p class="subtitle">Нажми на сердце — и получи одну из маленьких причин.</p>
  <div class="panel" style="text-align:center"><button class="heart-button" id="reasonBtn">♥</button><div class="reason-box" id="reasonText">Нажми на сердце, чтобы открыть послание.</div><div class="small muted" id="reasonNumber">♡ / 100</div></div>
</div></section>

<section class="section" id="letters"><div class="wrap">
  <div class="orn">✉</div><h2 class="section-title">Почтовая комната</h2><p class="subtitle">Письмо, которое можно открыть только по нажатию.</p>
  <div class="panel" style="text-align:center"><button class="envelope" id="envelopeBtn" aria-label="Открыть письмо">✉️</button><p class="small muted">Нажми на конверт</p><div class="letter" id="mainLetter">Моя дорогая подруга!

Спасибо за все разговоры, смех, поддержку и моменты, которые мы разделили. Я надеюсь, что впереди у нас ещё столько всего, о чём мы пока даже не подозреваем.

Береги себя и никогда не забывай, как много хорошего ты приносишь в этот мир.

С любовью, твоя подруга. ♡</div><div class="toolbar"><button class="btn ghost" id="editLetter">ИЗМЕНИТЬ ПИСЬМО</button></div></div>
</div></section>

<section class="section" id="secret-room"><div class="wrap">
  <div class="orn">☾</div><h2 class="section-title">Секретная комната</h2><p class="subtitle">Здесь спрятано послание. Введи пароль, чтобы открыть его.</p>
  <div class="panel" style="max-width:560px;margin:auto;text-align:center"><div style="font-size:42px">🔒</div><input class="field" id="secretPassword" type="password" placeholder="Введи пароль"><button class="btn" id="unlockBtn">ОТКРЫТЬ ДВЕРЬ</button><div class="secret" id="secretContent"><div class="display" style="margin-top:25px">Ты нашла секрет ♡</div><p class="small muted" id="secretMessage">Самые тёплые воспоминания ещё впереди. Спасибо, что ты есть.</p><button class="btn ghost" id="editSecret">ИЗМЕНИТЬ ПОСЛАНИЕ</button></div></div>
  <p class="small muted" style="text-align:center;margin-top:12px">Примечание: это игровой пароль, а не настоящая защита личных данных.</p>
</div></section>
</main>

<footer class="footer">СОЗДАНО С <span style="color:#bd748c">♡</span> И СОХРАНЕНО В НАШИХ ВОСПОМИНАНИЯХ</footer>

<div class="modal" id="modal"><div class="modal-box"><button class="modal-close" id="modalClose">×</button><div id="modalContent"></div></div></div>
<div class="toast" id="toast"></div>

<script>
const $=id=>document.getElementById(id);
const DB_NAME='friendship-universe-db', STORE='media';
let db;
const defaultReasons=[
'Ты умеешь превращать обычный день в особенный.','С тобой можно смеяться над полной ерундой.','Ты умеешь слушать.','У нас есть свои маленькие шутки.','С тобой можно быть собой.','Ты делаешь воспоминания ярче.','Ты не боишься быть настоящей.','С тобой даже молчание не неловкое.','Ты умеешь поддержать.','Ты — важная часть моей истории.',
'У тебя своё неповторимое чувство юмора.','Ты умеешь замечать мелочи.','С тобой всегда есть о чём поговорить.','Ты вдохновляешь пробовать новое.','Ты умеешь радоваться мелочам.','Ты делаешь мир чуточку добрее.','Ты не похожа ни на кого другого.','Ты умеешь удивлять.','Ты хранишь наши секреты.','Ты — человек, которому хочется рассказывать новости.',
'Ты умеешь быть искренней.','С тобой хочется строить планы.','Ты добавляешь красок в серые дни.','Ты умеешь находить смешное в неожиданном.','Ты помнишь важные детали.','Ты принимаешь странности.','Ты умеешь мечтать.','Ты делаешь обычные прогулки приключением.','Ты умеешь вдохновлять.','Ты рядом в важных моментах.',
'Ты умеешь говорить честно.','С тобой можно обсуждать всё на свете.','Ты даришь ощущение уюта.','Ты умеешь быть смелой.','Ты создаёшь атмосферу.','Ты умеешь ценить дружбу.','Ты оставляешь после себя хорошие воспоминания.','Ты умеешь удивляться миру.','Ты не даёшь скучать.','Ты — одна из моих любимых историй.',
'У нас есть общие воспоминания.','Ты умеешь поддержать разговор.','Ты делаешь праздники теплее.','Ты умеешь смеяться от души.','Ты интересный человек.','Ты умеешь быть внимательной.','Ты добавляешь в жизнь спонтанность.','Ты умеешь вдохновлять на творчество.','Ты умеешь признавать ошибки.','Ты умеешь прощать.',
'Ты помогаешь увидеть другую сторону ситуации.','Ты умеешь делиться радостью.','С тобой хочется фотографировать моменты.','Ты умеешь превращать идеи в планы.','Ты делаешь дружбу живой.','Ты умеешь быть терпеливой.','Ты умеешь замечать красоту.','Ты приносишь много хорошего.','Ты умеешь хранить смешные истории.','Ты — часть моих лучших воспоминаний.',
'Ты умеешь быть собой.','Ты делаешь даже переписки интересными.','Ты умеешь поддержать одной фразой.','Ты добавляешь жизни немного безумия.','Ты умеешь быть заботливой.','Ты умеешь придумывать необычное.','Ты помогаешь не забывать о хорошем.','Ты делаешь мир интереснее.','Ты умеешь радоваться за других.','Ты умеешь быть настоящим другом.',
'Ты умеешь ценить моменты.','Ты умеешь мечтать масштабно.','Ты добавляешь тепла в повседневность.','Ты умеешь быть решительной.','Ты умеешь замечать хорошее.','Ты создаёшь истории, которые хочется пересказывать.','Ты умеешь быть доброй.','Ты умеешь удивлять своими идеями.','Ты делаешь дружбу особенной.','Ты умеешь быть рядом.',
'Ты — человек со своим светом.','С тобой хочется узнавать новое.','Ты умеешь рассмешить.','Ты делаешь маленькие события важными.','Ты умеешь вдохновлять своим характером.','Ты умеешь слушать истории снова.','Ты умеешь создавать уют.','Ты делаешь воспоминания живыми.','Ты умеешь быть открытой.','Ты умеешь замечать детали.',
'Ты добавляешь в жизнь новые главы.','Ты умеешь быть верной себе.','Ты умеешь находить выход из неловких ситуаций.','Ты умеешь поддерживать мечты.','Ты делаешь обычные дни особенными.','Ты умеешь быть интересной собеседницей.','Ты — человек, которого я рада знать.','Ты умеешь дарить хорошее настроение.','Ты делаешь нашу историю уникальной.','Просто потому, что ты — это ты.'];
const state={memories:[],cards:[],about:'Этот сайт — маленькая коллекция всего, что делает нашу дружбу особенной. Здесь можно смеяться, вспоминать, перечитывать письма и находить сюрпризы.',aboutTitle:'Для самого дорогого человека',letter:$('mainLetter').textContent,secret:'Самые тёплые воспоминания ещё впереди. Спасибо, что ты есть.',password:'дружба',date:'',heroTitle:'Ты — часть моей истории.',heroText:$('heroText').textContent};
function loadState(){try{const s=JSON.parse(localStorage.getItem('friendshipState')||'{}');Object.assign(state,s)}catch(e){}}
function saveState(){localStorage.setItem('friendshipState',JSON.stringify(state))}
function toast(msg){$('toast').textContent=msg;$('toast').classList.add('show');setTimeout(()=>$('toast').classList.remove('show'),2300)}
function openDB(){return new Promise((resolve,reject)=>{const req=indexedDB.open(DB_NAME,1);req.onupgradeneeded=()=>req.result.createObjectStore(STORE,{keyPath:'id',autoIncrement:true});req.onsuccess=()=>{db=req.result;resolve(db)};req.onerror=()=>reject(req.error)})}
function mediaAdd(type,file){return new Promise((resolve,reject)=>{const tx=db.transaction(STORE,'readwrite');tx.objectStore(STORE).add({type,name:file.name,blob:file,created:Date.now()});tx.oncomplete=resolve;tx.onerror=()=>reject(tx.error)})}
function mediaAll(){return new Promise((resolve,reject)=>{const req=db.transaction(STORE).objectStore(STORE).getAll();req.onsuccess=()=>resolve(req.result);req.onerror=()=>reject(req.error)})}
function mediaDelete(id){return new Promise(resolve=>{const tx=db.transaction(STORE,'readwrite');tx.objectStore(STORE).delete(id);tx.oncomplete=resolve})}
function make(tag,cls,text){const el=document.createElement(tag);if(cls)el.className=cls;if(text!==undefined)el.textContent=text;return el}
async function renderMedia(){const all=await mediaAll();['photo','video','audio'].forEach(type=>$(type+'Grid').replaceChildren());all.forEach(m=>{const box=make('div','item');cons
