<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1.0,maximum-scale=1.0,user-scalable=no"><title>ENIGMA_KNOWLEDGE_BASE</title>
<script src="https://cdn.tailwindcss.com"></script>
<link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@300;400;500;700&family=Courier+Prime&display=swap" rel="stylesheet">
<style>
    /* Default Dark Mode for App */
    body{font-family:'Sarabun',sans-serif;background-color:#020202;color:#00ff41;-webkit-tap-highlight-color:transparent}
    .c-f{font-family:'Courier Prime',monospace}
    textarea,input{background-color:#0f0f0f!important;color:#00ff41!important;border-color:#003300!important;font-size:16px!important;appearance:none}
    textarea:focus,input:focus{border-color:#00ff41!important;outline:none;box-shadow:0 0 15px rgba(0,255,65,.15)}
    .b-a:active{transform:scale(.96)}
    .fade-in{animation:f .5s ease-in-out}@keyframes f{from{opacity:0}to{opacity:1}}
    
    /* Knowledge Page Specific Styles (Light Mode) */
    #_kp {
        background-color: #f8fafc; /* Slate-50 */
        color: #334155; /* Slate-700 */
        font-family: 'Sarabun', sans-serif;
    }
    #_kp h1 { color: #1e293b; }
    #_kp h2 { color: #0f172a; }
    #_kp strong { color: #0f172a; }
    
    /* Custom Scrollbar for Dark Mode parts */
    ::-webkit-scrollbar{width:4px}
    ::-webkit-scrollbar-track{background:#000}
    ::-webkit-scrollbar-thumb{background:#004411;border-radius:2px}
</style>
</head>
<body class="min-h-screen flex flex-col items-center justify-center">

<!-- 1. KNOWLEDGE PAGE (Educational Theme) -->
<!-- ใช้ fixed inset-0 เพื่อให้คลุมทับธีมมืดด้านหลังทั้งหมด -->
<div id="_kp" class="fixed inset-0 z-50 overflow-y-auto fade-in">
    <div class="max-w-4xl mx-auto px-6 py-12 pb-24"> <!-- pb-24 เผื่อที่ให้ปุ่มด้านล่าง -->
        <header class="mb-10 text-center border-b border-gray-200 pb-8">
            <h1 class="text-3xl md:text-4xl font-bold mb-3 tracking-tight">จักรกลปริศนา: The Enigma Machine</h1>
            <p class="text-gray-500 text-sm">แหล่งเรียนรู้ประวัติศาสตร์เทคโนโลยีการเข้ารหัส</p>
        </header>

        <article class="prose prose-slate max-w-none leading-relaxed space-y-6 text-base md:text-lg">
            <p>
                ในหน้าประวัติศาสตร์สงครามโลกครั้งที่ 2 <strong>"Enigma"</strong> ไม่ใช่แค่ชื่อของเครื่องจักร แต่เป็นสัญลักษณ์ของการชิงไหวชิงพริบทางปัญญาที่เดิมพันด้วยชีวิตคนนับล้าน เครื่องเข้ารหัสสัญชาติเยอรมันนี้ถูกออกแบบมาให้ดูภายนอกเหมือนเครื่องพิมพ์ดีดธรรมดา แต่ภายในซ่อนกลไกที่ซับซ้อนเกินกว่ามนุษย์ยุคนั้นจะจินตนาการ
            </p>

            <div class="my-8 p-6 bg-white rounded-lg shadow-sm border-l-4 border-blue-600">
                <h2 class="text-xl font-bold mb-2">กลไกการทำงาน</h2>
                <p class="text-gray-600 text-sm md:text-base">
                    หัวใจสำคัญคือ <strong>"โรเตอร์ (Rotors)"</strong> หรือวงล้อหมุนที่มีตัวอักษร 26 ตัว เมื่อผู้ใช้งานกดคีย์บอร์ด 1 ครั้ง สัญญาณไฟฟ้าจะวิ่งผ่านวงล้อเหล่านี้และสลับตำแหน่งไปมา ก่อนจะไปแสดงผลที่หลอดไฟ สิ่งที่น่าทึ่งคือ <em>"หากคุณกดตัวอักษร A ย้ำๆ กัน 3 ครั้ง เครื่องอาจจะแปลงเป็น G, P, และ X"</em> ไม่ซ้ำกันเลย ทำให้การแกะรอยหาความถี่ตัวอักษรเป็นไปไม่ได้
                </p>
            </div>

            <h2 class="text-2xl font-bold mt-8 mb-4">ความเป็นไปได้ที่ไร้ขีดจำกัด</h2>
            <p>
                ด้วยการสลับโรเตอร์ 3 ตัว และการเสียบสายไฟที่แผงด้านหน้า (Plugboard) ทำให้การตั้งค่าเริ่มต้นของเครื่องมีความเป็นไปได้มหาศาลถึง <strong>158,962,555,217,826,360,000 รูปแบบ</strong> (158 ล้านล้านล้าน) ทางกองทัพเยอรมันจึงมั่นใจว่ารหัสลับนี้ <em>"ไม่มีวันถูกถอดได้"</em>
            </p>

            <h2 class="text-2xl font-bold mt-8 mb-4">จุดเปลี่ยนของสงคราม</h2>
            <p>
                ความพยายามของทีมถอดรหัสที่ <strong>Bletchley Park</strong> นำโดยนักคณิตศาสตร์อัจฉริยะ <strong>Alan Turing</strong> ได้สร้างเครื่องจักร "The Bombe" เพื่อจำลองการทำงานย้อนกลับ ความสำเร็จนี้ช่วยให้ฝ่ายสัมพันธมิตรล่วงรู้แผนการรบ และได้รับการยกย่องว่าช่วยย่นระยะเวลาสงครามได้ถึง 2 ปี
            </p>
            
            <p class="text-sm text-gray-400 mt-12 pt-4 border-t border-gray-200">
                เอกสารอ้างอิง: พิพิธภัณฑ์สงครามและการเข้ารหัส (Declassified Archives)
            </p>
        </article>
    </div>

    <!-- ปุ่มเข้าสู่ระบบ (มุมขวาล่าง) -->
    <div class="fixed bottom-6 right-6 z-50">
        <button onclick="_k()" class="bg-gray-900 hover:bg-gray-700 text-white text-sm font-medium py-3 px-6 rounded-lg shadow-lg transition-all hover:-translate-y-1 flex items-center gap-2">
            เข้าสู่ระบบทดสอบ
            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3" />
            </svg>
        </button>
    </div>
</div>

<!-- 2. LOGIN PAGE (Hacker Theme) -->
<div id="_l" class="hidden w-full max-w-md p-8 bg-black border-2 border-green-800 rounded-2xl shadow-[0_0_60px_rgba(0,100,0,0.6)] text-center relative overflow-hidden fade-in">
    <div class="absolute top-0 left-0 w-full h-1 bg-gradient-to-r from-transparent via-green-500 to-transparent"></div>
    <h1 class="text-3xl font-bold text-green-500 mb-2 tracking-widest animate-pulse">ACCESS GATE</h1>
    <p class="text-[10px] text-green-800 mb-8 uppercase tracking-[0.3em]">Identity Verification Required</p>
    <div class="mb-6"><input id="_p" type="password" class="w-full p-4 rounded-xl border-2 c-f text-center text-lg tracking-widest placeholder-green-900" placeholder="PASSCODE"></div>
    <button onclick="_c()" class="w-full bg-green-900 hover:bg-green-800 text-white font-bold py-4 rounded-xl border border-green-600 transition-all shadow-[0_0_15px_rgba(0,255,65,0.3)]">AUTHENTICATE</button>
    <p id="_m" class="mt-4 text-xs text-red-500 h-4 font-mono"></p>
</div>

<!-- 3. MAIN APP (Chaos Engine) -->
<div id="_m_a" class="hidden w-full max-w-xl mx-auto mt-2 sm:mt-6 p-6 sm:p-8 bg-black border border-green-800 rounded-2xl shadow-[0_0_50px_rgba(0,50,0,0.5)] relative overflow-hidden fade-in">
    <h1 class="text-xl sm:text-2xl font-bold text-center mb-1 tracking-widest text-green-500">CHAOS ENGINE V.29</h1>
    <p class="text-[9px] text-center text-green-800 mb-6 uppercase tracking-[0.2em]">Non-Linear Cryptography</p>
    <div class="mb-5"><label class="block text-[10px] font-bold mb-1.5 text-yellow-600 uppercase ml-1">Chaos Seed</label><input id="_sk" type="password" class="w-full p-3 rounded-lg border-2 c-f text-center tracking-[0.5em]" placeholder="KEY"></div>
    <div class="mb-4"><label class="block text-[10px] font-bold mb-1.5 text-green-800 uppercase ml-1">Input</label><textarea id="_i" rows="3" class="w-full p-4 rounded-lg border-2 c-f" placeholder="..."></textarea></div>
    <div class="flex flex-col sm:flex-row gap-3 mb-6"><div class="flex flex-row gap-2 flex-1"><button onclick="_e()" class="b-a flex-1 bg-green-950 hover:bg-green-900 text-green-400 font-bold py-4 rounded-lg border border-green-700 text-sm transition-all">GEN CHAOS</button><button onclick="_d()" class="b-a flex-1 bg-blue-950 hover:bg-blue-900 text-blue-400 font-bold py-4 rounded-lg border border-blue-700 text-sm transition-all">REV CHAOS</button></div><button onclick="_z()" class="b-a w-full sm:w-20 bg-gray-900 text-gray-500 py-4 sm:py-2 rounded-lg border border-gray-800 text-sm">CLR</button></div>
    <div class="relative"><label class="block text-[10px] font-bold mb-1.5 text-green-800 uppercase ml-1">Stream</label><textarea id="_o" rows="5" readonly class="w-full p-4 rounded-lg border-2 c-f break-all text-xs tracking-wider" placeholder="..."></textarea><button onclick="_cp()" class="b-a absolute bottom-3 right-3 bg-green-900/60 hover:bg-green-800 text-white text-[9px] font-bold px-3 py-1.5 rounded border border-green-600">COPY</button></div>
    <div class="mt-4 text-center"><span id="_en" class="text-[9px] text-green-900 font-mono">E: 0%</span></div>
</div>

<!-- ERROR MODAL -->
<div id="_err" class="fixed inset-0 bg-black bg-opacity-95 z-50 flex items-center justify-center hidden"><div class="bg-black border-4 border-red-600 p-6 sm:p-8 rounded-xl shadow-[0_0_50px_rgba(255,0,0,0.8)] text-center max-w-sm sm:max-w-md w-full relative mx-4"><h2 class="text-3xl sm:text-4xl text-red-600 font-bold mb-4 tracking-widest animate-pulse">ERROR</h2><div class="h-px w-full bg-red-600 mb-6"></div><p class="text-red-500 mb-8 text-xs sm:text-sm tracking-widest c-f leading-relaxed">UNAUTHORIZED ACCESS.<br>PROTOCOL 0xDEADBEEF.</p><button id="_cb" onclick="_ce()" class="border-2 border-red-600 text-red-600 hover:bg-red-600 hover:text-black font-bold px-6 py-3 rounded tracking-widest transition-all duration-100 uppercase text-xs sm:text-sm w-full">TERMINATE</button></div></div>

<script>
const _A="ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";let _ec=0;
document.oncontextmenu=e=>{e.preventDefault();_t()};
document.onkeydown=e=>{if(123==e.keyCode||(e.ctrlKey&&e.shiftKey&&73==e.keyCode)||(e.ctrlKey&&e.shiftKey&&67==e.keyCode)||(e.ctrlKey&&e.shiftKey&&74==e.keyCode)||(e.ctrlKey&&85==e.keyCode))return!1};
function _k(){document.getElementById('_kp').style.display='none';document.getElementById('_l').classList.remove('hidden')}
function _c(){let p=document.getElementById('_p').value;if(p==="Good"){document.getElementById('_l').style.display='none';document.getElementById('_m_a').classList.remove('hidden');document.getElementById('_p').value=''}else{let m=document.getElementById('_m');m.innerText="DENIED";let ip=document.getElementById('_p');ip.classList.add('border-red-600');setTimeout(()=>ip.classList.remove('border-red-600'),500)}}
document.getElementById('_p').addEventListener("keypress",e=>{if(e.key==="Enter"){e.preventDefault();_c()}});
function _t(){_ec++;document.getElementById('_err').classList.remove('hidden');if(_ec>=5)document.getElementById('_cb').style.display='none'}
function _ce(){document.getElementById('_err').classList.add('hidden')}
function _gn(l){let r='';for(let i=0;i<l;i++)r+=_A.charAt(Math.floor(Math.random()*_A.length));return r}
function _nv(n){let v=0;for(let i=0;i<n.length;i++)v+=n.charCodeAt(i);return v}
function _gs(){let s=document.getElementById('_sk').value||"D";let v=0;for(let i=0;i<s.length;i++)v+=s.charCodeAt(i)*(i+1);return v}
function _e(){let i=document.getElementById('_i').value;if(!i)return;let n=_gn(4),s=_gs(),cc=_nv(n)+s,o=`[${n}]`;for(let k=0;k<i.length;k++){let c=i.charCodeAt(k),ev=c+cc+(k*7),vs=ev.toString(36).toUpperCase();o+=vs+".";cc=(cc+ev)%99999}document.getElementById('_o').value=o;_u()}
function _d(){let i=document.getElementById('_o').value||document.getElementById('_i').value;if(!i)return;let m=i.match(/^\[([A-Za-z0-9]{4})\]/);if(!m){alert("ERR_HEAD");return}let n=m[1],s=_gs(),cc=_nv(n)+s,d=i.substring(6),tk=d.split("."),r="";for(let k=0;k<tk.length;k++){if(tk[k]==="")continue;let ev=parseInt(tk[k],36),cd=ev-cc-(k*7);r+=String.fromCharCode(cd);cc=(cc+ev)%99999}document.getElementById('_o').value=r}
function _z(){document.getElementById('_i').value="";document.getElementById('_o').value="";document.getElementById('_en').innerText="E: 0%"}
function _cp(){let o=document.getElementById('_o');o.select();document.execCommand('copy');let b=event.target;b.innerText="OK";setTimeout(()=>b.innerText="CP",2000)}
function _u(){document.getElementById('_en').innerText=`E: ${Math.floor(Math.random()*20)+80}%`}
</script>
</body>
</html>
