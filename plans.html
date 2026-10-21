(()=>{
'use strict';
if(top!==self){try{top.location=self.location}catch(e){document.documentElement.style.display='none'}}
const $=s=>document.querySelector(s),B=document.body,H=document.documentElement;
const reduce=matchMedia('(prefers-reduced-motion: reduce)').matches;
const L={
ar:{h1:'مرحبًا بك في عالم AQX',lead:'هويتك الموحدة للوصول إلى خدمات AQX.',slogan:'حساب واحد. عالم كامل.',
c1t:'إنشاء حساب جديد',c1d:'ابدأ رحلتك مع AQX.',c2t:'تسجيل الدخول',c2d:'تابع من حيث توقفت.',c3t:'الاشتراكات والباقات',c3d:'اكتشف الخدمات والباقات المتاحة.',
note:'الاشتراك منفصل عن إنشاء الحساب: الحساب هو هويتك، والاشتراك هو ما تختاره من خدمات.',
about:'الحساب الموحد AQX (AQX-UA) هو البوابة الرسمية لمنظومة AQX: حساب واحد لتسجيل الدخول وإدارة الاشتراكات والوصول إلى كل الخدمات.',
skip:'تخطي المقدمة',sndOff:'الصوت: متوقف',sndOn:'الصوت: يعمل',stUnknown:'جارٍ التحقق من الحالة',stUp:'جميع الخدمات تعمل',stDegraded:'أداء جزئي',stDown:'الخدمات متوقفة',stErr:'تعذر التحقق من الحالة',msg:'عالمك يبدأ من هنا.',btn:'English'},
en:{h1:'Welcome to the AQX universe',lead:'Your unified identity for every AQX service.',slogan:'One Account. Infinite Possibilities.',
c1t:'Create account',c1d:'Start your journey with AQX.',c2t:'Sign in',c2d:'Pick up where you left off.',c3t:'Plans & subscriptions',c3d:'Explore available services and plans.',
note:'A subscription is separate from an account: the account is your identity, the subscription is the services you choose.',
about:'AQX Unified Account (AQX-UA) is the official gateway to the AQX ecosystem: one account to sign in, manage subscriptions and reach every service. Also searched as alqurmani x or alqurmanix.',
skip:'Skip intro',sndOff:'Sound: off',sndOn:'Sound: on',stUnknown:'Checking status',stUp:'All services operational',stDegraded:'Partial degradation',stDown:'Services down',stErr:'Status unavailable',msg:'Your world starts here.',btn:'العربية'}
};
let lang='ar',stKey='stUnknown';
try{lang=localStorage.getItem('aqx-lang')||(navigator.language||'').startsWith('en')?'en':'ar';const s=localStorage.getItem('aqx-lang');if(s)lang=s}catch(e){}
function apply(){
 H.lang=lang;H.dir=lang==='ar'?'rtl':'ltr';
 document.querySelectorAll('[data-i18n]').forEach(e=>{const k=e.dataset.i18n;if(k==='stUnknown')return;if(k==='sndOff'){return}e.textContent=L[lang][k]});
 $('#lang').textContent=L[lang].btn;$('#snd').textContent=soundOn?L[lang].sndOn:L[lang].sndOff;$('#statusTxt').textContent=L[lang][stKey];
 $('#main .about p').textContent=L[lang].about;
}
$('#lang').onclick=()=>{lang=lang==='ar'?'en':'ar';try{localStorage.setItem('aqx-lang',lang)}catch(e){}apply()};

/* sound (opt-in, synthesized) */
let ac,soundOn=false;
function tone(f1,f2,d,type,v){if(!soundOn||!ac)return;const t=ac.currentTime,o=ac.createOscillator(),g=ac.createGain();o.type=type||'sine';o.frequency.setValueAtTime(f1,t);o.frequency.exponentialRampToValueAtTime(f2,t+d);g.gain.setValueAtTime(.0001,t);g.gain.linearRampToValueAtTime(v||.07,t+.06);g.gain.exponentialRampToValueAtTime(.0001,t+d);o.connect(g).connect(ac.destination);o.start(t);o.stop(t+d)}
$('#snd').onclick=()=>{try{ac=ac||new (window.AudioContext||window.webkitAudioContext)();ac.resume()}catch(e){return}soundOn=!soundOn;apply();if(soundOn)tone(120,360,2,'sine',.08)};

/* canvas galaxy */
const cv=$('#fx'),c=cv.getContext('2d');let W,Hh,dpr,mode='galaxy',grow=0,glow=0,tilt=.5,ringA=0,spin=1;
function size(){dpr=Math.min(devicePixelRatio||1,2);W=cv.width=innerWidth*dpr;Hh=cv.height=innerHeight*dpr}
size();addEventListener('resize',size);
const N=innerWidth<700?650:1300;
const P=Array.from({length:N},()=>{const arm=(Math.random()*3)|0,r=Math.pow(Math.random(),.65);return{a:arm*2.094+r*5+(Math.random()-.5)*.55,r0:r,cr:0,s:.3+Math.random()*.9,z:Math.random(),h:Math.random()<.6?188:262,j:Math.random()}});
const S=Array.from({length:160},()=>({x:Math.random(),y:Math.random(),z:Math.random(),p:Math.random()*6}));
function frame(t){
 c.globalCompositeOperation='source-over';c.clearRect(0,0,W,Hh);
 const cx=W/2,cy=Hh/2,R=Math.min(W,Hh)*.44;
 for(const s of S){const a=.25+.35*Math.sin(t/700+s.p);c.fillStyle=`rgba(190,215,255,${a*s.z})`;c.fillRect(s.x*W,s.y*Hh,s.z*1.6*dpr,s.z*1.6*dpr)}
 c.globalCompositeOperation='lighter';
 const amb=mode==='ambient';
 let gt=mode==='ring'||mode==='open'?0:amb?.1:(mode==='galaxy'?.7:.25),tt=mode==='ring'||mode==='open'?1:amb?.5:.5;
 grow+=((amb?1:mode==='open'?0:1)-grow)*.02;glow+=((mode==='ring'?1.2:mode==='open'?2.4:mode==='logo'||mode==='msg'?.7:amb?.18:.6)-glow)*.03;
 tilt+=(tt-tilt)*.03;ringA+=((mode==='ring'?1:mode==='open'?.0:0)-ringA)*.04;
 const g=c.createRadialGradient(cx,cy,0,cx,cy,R*(.35+glow*.25));g.addColorStop(0,`rgba(255,255,255,${Math.min(.9,.5*glow)})`);g.addColorStop(.25,`rgba(37,232,255,${.35*glow})`);g.addColorStop(1,'rgba(123,77,255,0)');
 c.fillStyle=g;c.fillRect(0,0,W,Hh);
 for(const p of P){
  let tr=p.r0*(mode==='galaxy'?grow:1);
  if(mode==='logo'||mode==='msg')tr=p.r0*.55+.05;
  if(mode==='ring')tr=.62+p.j*.015;
  if(mode==='open')tr=2.2+p.r0*2;
  if(amb)tr=p.r0*1.1+.05;
  p.cr+=(tr-p.cr)*(mode==='open'?.05:.035);
  p.a+=(.0015+.004*(1-p.r0*.6))*p.s*spin*(mode==='ring'?2.5:1);
  const x=cx+Math.cos(p.a)*p.cr*R,y=cy+Math.sin(p.a)*p.cr*R*(tilt+(1-tilt)*ringA*0+0);
  const al=(amb?.45:.9)*(.35+p.z*.65)*(mode==='open'?Math.max(0,1-(p.cr-.8)/1.6):1);
  c.fillStyle=`hsla(${p.h},100%,${60+p.z*25}%,${al})`;const sz=(.6+p.z*1.8)*dpr;c.fillRect(x,y,sz,sz);
 }
 if(ringA>.02){c.lineWidth=5*dpr;const gr=c.createLinearGradient(cx-R,cy,cx+R,cy);gr.addColorStop(0,`rgba(123,77,255,${ringA})`);gr.addColorStop(.5,`rgba(37,232,255,${ringA})`);gr.addColorStop(1,`rgba(123,77,255,${ringA})`);c.strokeStyle=gr;c.shadowColor='#25e8ff';c.shadowBlur=30*dpr;c.beginPath();c.ellipse(cx,cy,R*.62,R*.62*(tilt+(1-tilt)),0,0,6.283);c.stroke();c.shadowBlur=0}
 if(!reduce)requestAnimationFrame(frame);
}

/* timeline */
let ids=[],done=false;
function ph(n,ms){ids.push(setTimeout(()=>{B.dataset.ph=n;mode=n;if(n==='logo')tone(300,900,.5,'triangle',.09);if(n==='ring')tone(90,700,1.8,'sawtooth',.04);if(n==='msg')typeMsg()},ms))}
function typeMsg(){const el=$('#msg'),txt=L[lang].msg;let i=0;const k=setInterval(()=>{el.textContent=txt.slice(0,++i);if(i>=txt.length)clearInterval(k)},90)}
function finish(){if(done)return;done=true;ids.forEach(clearTimeout);mode='ambient';delete B.dataset.ph;
 $('#intro').classList.remove('flash');B.classList.remove('intro-on');B.classList.add('revealed')}
function open(){tone(200,1400,1.4,'sine',.07)}
function start(){
 apply();
 if(reduce){mode='ambient';P.forEach(p=>p.cr=p.r0*1.1+.05);frame(0);return}
 B.classList.add('intro-on');requestAnimationFrame(frame);
 B.dataset.ph='galaxy';ph('galaxy',0);ph('logo',3200);ph('msg',6400);ph('ring',9200);
 ids.push(setTimeout(()=>{B.dataset.ph='open';mode='open';open();$('#intro').classList.add('flash')},11000));
 ids.push(setTimeout(finish,12300));
 $('#skip').onclick=()=>{finish()};
 addEventListener('keydown',e=>{if(e.key==='Escape')finish()});
}
requestAnimationFrame(()=>{});
if(!reduce){} start();
if(!reduce){const m=document.querySelector('.about');}

/* card glow */
document.querySelectorAll('.gate').forEach(g=>g.addEventListener('pointermove',e=>{const r=g.getBoundingClientRect();g.style.setProperty('--mx',e.clientX-r.left+'px');g.style.setProperty('--my',e.clientY-r.top+'px')}));

/* real status from status.json */
async function check(){
 const el=$('#status');
 try{const r=await fetch('status.json',{cache:'no-store'});if(!r.ok)throw 0;const j=await r.json();
  const s=j.status==='operational'?'up':j.status==='degraded'?'degraded':'down';
  el.dataset.s=s;stKey={up:'stUp',degraded:'stDegraded',down:'stDown'}[s]}
 catch(e){el.dataset.s='unknown';stKey='stErr'}
 $('#statusTxt').textContent=L[lang][stKey];
}
check();setInterval(check,60000);
})();
