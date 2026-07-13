<!-- README Aura animated SVG header -->
```aura width=1200 height=420
<div
  style={{
    width: '100%',
    height: '100%',
    display: 'flex',
    position: 'relative',
    overflow: 'hidden',
    background: '#020617',
    borderRadius: 24,
    alignItems: 'center',
    justifyContent: 'center',
    fontFamily: 'Inter',
  }}
>
  <style>{`
    @keyframes driftA {
      from { transform: translateX(0px) translateY(0px); opacity: .82; }
      to { transform: translateX(-70px) translateY(18px); opacity: 1; }
    }
    @keyframes driftB {
      from { transform: translateX(0px) translateY(0px); opacity: .55; }
      to { transform: translateX(90px) translateY(-18px); opacity: .9; }
    }
    @keyframes spinSlow {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }
    @keyframes spinReverse {
      from { transform: rotate(360deg); }
      to { transform: rotate(0deg); }
    }
    @keyframes pulseCore {
      0%, 100% { opacity: .30; transform: scale(1); }
      50% { opacity: .55; transform: scale(1.08); }
    }
    @keyframes titleGlow {
      0%, 100% { opacity: .72; }
      50% { opacity: 1; }
    }
    #starLayerA { animation: driftA 18s linear infinite alternate; transform-origin: 600px 210px; }
    #starLayerB { animation: driftB 28s linear infinite alternate; transform-origin: 600px 210px; }
    #orbitA { animation: spinSlow 26s linear infinite; transform-origin: 600px 210px; }
    #orbitB { animation: spinReverse 38s linear infinite; transform-origin: 600px 210px; }
    #coreGlow { animation: pulseCore 4s ease-in-out infinite; transform-origin: 600px 210px; }
    #titleHalo { animation: titleGlow 3.5s ease-in-out infinite; }
  `}</style>

  <svg width="1200" height="420" viewBox="0 0 1200 420" style={{ position: 'absolute', left: 0, top: 0 }}>
    <defs>
      <radialGradient id="heroGlow" cx="50%" cy="50%" r="55%">
        <stop offset="0%" stopColor="#2563eb" stopOpacity="0.34" />
        <stop offset="45%" stopColor="#7c3aed" stopOpacity="0.16" />
        <stop offset="100%" stopColor="#020617" stopOpacity="0" />
      </radialGradient>
    </defs>
    <rect width="1200" height="420" fill="#020617" />
    <circle id="coreGlow" cx="600" cy="210" r="260" fill="url(#heroGlow)" />
    <g id="orbitA" opacity=".8">
      <ellipse cx="600" cy="210" rx="450" ry="106" fill="none" stroke="#2563eb" strokeWidth="1.5" strokeDasharray="10 20" />
      <circle cx="150" cy="210" r="5" fill="#38bdf8" />
      <circle cx="1050" cy="210" r="3" fill="#a78bfa" />
    </g>
    <g id="orbitB" opacity=".65">
      <ellipse cx="600" cy="210" rx="330" ry="78" fill="none" stroke="#a78bfa" strokeWidth="1" strokeDasharray="4 16" />
      <circle cx="270" cy="210" r="4" fill="#f8fafc" />
      <circle cx="930" cy="210" r="4" fill="#60a5fa" />
    </g>
    <g id="starLayerA">
      <circle cx="1170" cy="16" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="422" cy="236" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="70" cy="266" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="511" cy="381" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="284" cy="308" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="580" cy="345" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="620" cy="338" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="490" cy="225" r="2" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="1193" cy="2" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="620" cy="274" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="1124" cy="230" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="1197" cy="166" r="2" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="845" cy="122" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="616" cy="418" r="2" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="306" cy="196" r="2" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="231" cy="397" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="391" cy="178" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="502" cy="348" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="244" cy="136" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="356" cy="398" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="671" cy="222" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="679" cy="163" r="1" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="917" cy="207" r="2" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="1015" cy="344" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="1065" cy="247" r="2" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="340" cy="250" r="2" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="278" cy="215" r="2" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="1103" cy="198" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="202" cy="212" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="1096" cy="33" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="311" cy="55" r="2" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="285" cy="234" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="702" cy="371" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="672" cy="332" r="2" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="486" cy="165" r="2" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="1178" cy="321" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="606" cy="222" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="94" cy="305" r="2" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="333" cy="343" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="820" cy="402" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="163" cy="302" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="196" cy="350" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="916" cy="340" r="2" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="544" cy="305" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="429" cy="217" r="2" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="409" cy="35" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="712" cy="130" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="396" cy="321" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="602" cy="259" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="828" cy="226" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="567" cy="247" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="171" cy="353" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="345" cy="308" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="627" cy="8" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="151" cy="379" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="578" cy="310" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="630" cy="48" r="2" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="1167" cy="381" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="1166" cy="292" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="803" cy="103" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="1070" cy="414" r="2" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="1184" cy="25" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="813" cy="166" r="2" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="240" cy="310" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="1099" cy="261" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="899" cy="295" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="910" cy="361" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="905" cy="309" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="703" cy="286" r="2" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="398" cy="49" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="383" cy="327" r="2" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="737" cy="286" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="338" cy="159" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="204" cy="325" r="2" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="619" cy="21" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="159" cy="176" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="344" cy="207" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="354" cy="90" r="2" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="1051" cy="328" r="2" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="812" cy="416" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="865" cy="369" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="1092" cy="332" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="500" cy="272" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="791" cy="355" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="204" cy="295" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="588" cy="181" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="153" cy="204" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="693" cy="91" r="2" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="664" cy="320" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="421" cy="65" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="504" cy="197" r="2" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="1128" cy="389" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="252" cy="14" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="789" cy="34" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="863" cy="24" r="2" fill="#ffffff" fillOpacity="0.45" />
    </g>
    <g id="starLayerB">
      <circle cx="228" cy="12" r="3" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="457" cy="71" r="3" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="864" cy="16" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="476" cy="258" r="3" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="1116" cy="214" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="13" cy="388" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="569" cy="79" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="189" cy="194" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="541" cy="413" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="775" cy="40" r="3" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="1182" cy="98" r="3" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="466" cy="395" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="206" cy="194" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="333" cy="189" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="146" cy="311" r="3" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="334" cy="236" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="664" cy="393" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="646" cy="205" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="1161" cy="367" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="810" cy="329" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="285" cy="126" r="3" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="1197" cy="219" r="3" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="449" cy="70" r="3" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="96" cy="56" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="130" cy="197" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="1083" cy="128" r="3" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="1099" cy="384" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="601" cy="222" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="539" cy="256" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="611" cy="327" r="3" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="313" cy="191" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="663" cy="250" r="1" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="629" cy="122" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="175" cy="374" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="262" cy="337" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="542" cy="270" r="3" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="1104" cy="386" r="3" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="817" cy="343" r="3" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="1059" cy="231" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="131" cy="173" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="451" cy="3" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="138" cy="16" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="570" cy="342" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="1169" cy="295" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="833" cy="97" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="725" cy="216" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="201" cy="31" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="509" cy="98" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="287" cy="216" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="511" cy="38" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="103" cy="333" r="3" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="484" cy="85" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="437" cy="205" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="4" cy="199" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="866" cy="356" r="3" fill="#a78bfa" fillOpacity="0.90" />
    </g>
    <g>
      <line id="meteor0" x1="397" y1="186" x2="492" y2="214" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="4.6s" begin="1.2s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="4.6s" begin="1.2s" repeatCount="indefinite" />
      </line>
      <line id="meteor1" x1="115" y1="169" x2="245" y2="197" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="4.6s" begin="0.9s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="4.6s" begin="0.9s" repeatCount="indefinite" />
      </line>
      <line id="meteor2" x1="1018" y1="276" x2="1088" y2="304" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="5.4s" begin="0.1s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="5.4s" begin="0.1s" repeatCount="indefinite" />
      </line>
      <line id="meteor3" x1="898" y1="108" x2="992" y2="136" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="6.2s" begin="1.1s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="6.2s" begin="1.1s" repeatCount="indefinite" />
      </line>
      <line id="meteor4" x1="558" y1="184" x2="643" y2="212" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="3.8s" begin="3.5s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="3.8s" begin="3.5s" repeatCount="indefinite" />
      </line>
      <line id="meteor5" x1="413" y1="293" x2="543" y2="321" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="4.6s" begin="1.4s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="4.6s" begin="1.4s" repeatCount="indefinite" />
      </line>
      <line id="meteor6" x1="272" y1="56" x2="352" y2="84" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="4.6s" begin="3.5s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="4.6s" begin="3.5s" repeatCount="indefinite" />
      </line>
      <line id="meteor7" x1="776" y1="324" x2="914" y2="352" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="3.8s" begin="0.6s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="3.8s" begin="0.6s" repeatCount="indefinite" />
      </line>
      <line id="meteor8" x1="314" y1="188" x2="395" y2="216" stroke="#93c5fd" strokeWidth="2" strokeLinecap="round" opacity="0">
        <animate attributeName="opacity" values="0;0.95;0" dur="3.8s" begin="3.6s" repeatCount="indefinite" />
        <animateTransform attributeName="transform" type="translate" from="0 0" to="230 48" dur="3.8s" begin="3.6s" repeatCount="indefinite" />
      </line>
    </g>
  </svg>

  <div
    style={{
      position: 'absolute',
      left: 70,
      right: 70,
      top: 70,
      bottom: 60,
      display: 'flex',
      flexDirection: 'column',
      alignItems: 'center',
      justifyContent: 'center',
      textAlign: 'center',
    }}
  >
    <div id="titleHalo" style={{ position: 'absolute', width: 700, height: 126, borderRadius: 999, background: 'radial-gradient(circle, rgba(59, 130, 246, .24), rgba(124, 58, 237, .10), rgba(2, 6, 23, 0))' }} />
    <div style={{ fontSize: 72, fontWeight: 800, color: '#f8fafc', lineHeight: 1.08 }}>
      Faizan Aslam
    </div>
    <div style={{ marginTop: 18, fontSize: 30, color: '#bfdbfe', fontWeight: 600 }}>
      Full-Stack Developer | AI Applications | Unity 3D
    </div>
    <div style={{ marginTop: 20, fontSize: 23, color: '#e2e8f0', maxWidth: 980, lineHeight: 1.45 }}>
      I build production-ready web platforms, AI-powered tools, and interactive 3D experiences.
    </div>
    <div style={{ marginTop: 30, display: 'flex', gap: 14, flexWrap: 'wrap', justifyContent: 'center' }}>
      <div style={{ padding: '8px 18px', borderRadius: 999, border: '1px solid #38bdf8', background: 'rgba(15, 23, 42, .72)', color: '#f8fafc', fontSize: 18, fontWeight: 700 }}>Next.js</div>
      <div style={{ padding: '8px 18px', borderRadius: 999, border: '1px solid #a78bfa', background: 'rgba(15, 23, 42, .72)', color: '#f8fafc', fontSize: 18, fontWeight: 700 }}>RAG</div>
      <div style={{ padding: '8px 18px', borderRadius: 999, border: '1px solid #22d3ee', background: 'rgba(15, 23, 42, .72)', color: '#f8fafc', fontSize: 18, fontWeight: 700 }}>OpenCV</div>
      <div style={{ padding: '8px 18px', borderRadius: 999, border: '1px solid #e2e8f0', background: 'rgba(15, 23, 42, .72)', color: '#f8fafc', fontSize: 18, fontWeight: 700 }}>Unity</div>
      <div style={{ padding: '8px 18px', borderRadius: 999, border: '1px solid #60a5fa', background: 'rgba(15, 23, 42, .72)', color: '#f8fafc', fontSize: 18, fontWeight: 700 }}>Postgres</div>
    </div>
  </div>
</div>
```

<p align="center">
  <a href="https://github.com/FaizanAslam10"><img src="assets/contact-github.svg" width="286" alt="GitHub - FaizanAslam10" /></a><a href="https://linkedin.com/in/faizan-aslam10"><img src="assets/contact-linkedin.svg" width="286" alt="LinkedIn - faizan-aslam10" /></a><a href="mailto:m.faizanaslam10@gmail.com"><img src="assets/contact-email.svg" width="286" alt="Email - m.faizanaslam10@gmail.com" /></a><img src="assets/contact-views.svg" width="286" alt="Visitor telemetry" />
</p>

```aura width=1200 height=84
<div
  style={{
    width: '100%',
    height: '100%',
    display: 'flex',
    position: 'relative',
    overflow: 'hidden',
    background: '#020617',
    borderRadius: 18,
  }}
>
  <style>{`
    @keyframes sweep {
      from { transform: translateX(-80px); opacity: .65; }
      to { transform: translateX(80px); opacity: 1; }
    }
    #dividerStars201 { animation: sweep 16s linear infinite alternate; }
  `}</style>
  <svg width="1200" height="84" viewBox="0 0 1200 84" style={{ position: 'absolute', left: 0, top: 0 }}>
    <defs>
      <linearGradient id="line201" x1="0" x2="1" y1="0" y2="0">
        <stop offset="0%" stopColor="#020617" />
        <stop offset="35%" stopColor="#2563eb" />
        <stop offset="65%" stopColor="#7c3aed" />
        <stop offset="100%" stopColor="#020617" />
      </linearGradient>
    </defs>
    <rect width="1200" height="84" fill="#020617" />
    <g id="dividerStars201">
      <circle cx="137" cy="41" r="1" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="668" cy="60" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="987" cy="71" r="2" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="1160" cy="61" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="440" cy="24" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="490" cy="71" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="62" cy="73" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="993" cy="12" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="1149" cy="48" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="902" cy="5" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="413" cy="52" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="515" cy="75" r="2" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="549" cy="43" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="368" cy="62" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="1168" cy="67" r="1" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="1042" cy="65" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="76" cy="68" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="927" cy="0" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="944" cy="74" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="842" cy="21" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="46" cy="14" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="733" cy="55" r="2" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="697" cy="26" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="868" cy="76" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="935" cy="30" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="489" cy="22" r="2" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="294" cy="69" r="2" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="612" cy="45" r="2" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="282" cy="5" r="2" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="1153" cy="11" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="273" cy="67" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="344" cy="54" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="771" cy="13" r="2" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="1085" cy="10" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="995" cy="13" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="54" cy="62" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="613" cy="42" r="2" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="68" cy="0" r="2" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="1182" cy="38" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="888" cy="69" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="626" cy="47" r="2" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="817" cy="5" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="13" cy="8" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="101" cy="19" r="2" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="496" cy="0" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="229" cy="57" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="27" cy="76" r="2" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="488" cy="37" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="905" cy="40" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="818" cy="36" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="925" cy="19" r="2" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="939" cy="10" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="37" cy="51" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="756" cy="21" r="2" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="853" cy="30" r="2" fill="#93c5fd" fillOpacity="0.90" />
    </g>
    <rect x="120" y="41" width="960" height="2" rx="1" fill="url(#line201)" opacity=".95" />
  </svg>
</div>
```

## Transmission: About Me

> Incoming signal from **Lahore, Pakistan**

I'm a Computer Science student and Full-Stack Developer building software that actually ships: AI legal research, RAG pipelines, business websites, e-commerce systems, computer vision tools, and Unity games.

I build products **end to end** - interface, backend, database, authentication, deployment, and polish. From the first commit to the final orbit.

## Constellation of Highlights

- Built **Qanoon**, an AI legal research assistant grounded in **1,000+ Pakistani statutes**
- Implemented RAG pipelines with vector embeddings, semantic search, and Postgres vector storage
- Built a 2D floor plan to 3D visualization workflow using OpenCV and CNN-based recognition
- Shipped full-stack business websites with frontend, backend, database, auth, and deployment
- Built Unity projects including 2D games and ongoing 3D AI-driven gameplay systems

```aura width=1200 height=310
<div
  style={{
    width: '100%',
    height: '100%',
    display: 'flex',
    position: 'relative',
    overflow: 'hidden',
    background: '#030712',
    borderRadius: 22,
    fontFamily: 'Inter',
  }}
>
  <style>{`
    @keyframes orbitDash {
      from { stroke-dashoffset: 0; }
      to { stroke-dashoffset: -220; }
    }
    @keyframes scanLine {
      0% { transform: translateX(-260px); opacity: 0; }
      20% { opacity: .95; }
      100% { transform: translateX(1240px); opacity: 0; }
    }
    @keyframes nodePulse {
      0%, 100% { opacity: .45; transform: scale(1); }
      50% { opacity: 1; transform: scale(1.4); }
    }
    #missionOrbit { animation: orbitDash 10s linear infinite; }
    #missionScan { animation: scanLine 4.6s ease-in-out infinite; }
    #nodeA { animation: nodePulse 2.4s ease-in-out infinite; transform-origin: 282px 154px; }
    #nodeB { animation: nodePulse 3.0s ease-in-out infinite; transform-origin: 600px 74px; }
    #nodeC { animation: nodePulse 2.7s ease-in-out infinite; transform-origin: 920px 154px; }
  `}</style>
  <svg width="1200" height="310" viewBox="0 0 1200 310" style={{ position: 'absolute', left: 0, top: 0 }}>
    <defs>
      <radialGradient id="consoleGlow" cx="50%" cy="50%" r="65%">
        <stop offset="0%" stopColor="#0ea5e9" stopOpacity=".26" />
        <stop offset="55%" stopColor="#7c3aed" stopOpacity=".12" />
        <stop offset="100%" stopColor="#030712" stopOpacity="0" />
      </radialGradient>
      <linearGradient id="scanGrad" x1="0" x2="1" y1="0" y2="0">
        <stop offset="0%" stopColor="#38bdf8" stopOpacity="0" />
        <stop offset="50%" stopColor="#38bdf8" stopOpacity=".95" />
        <stop offset="100%" stopColor="#38bdf8" stopOpacity="0" />
      </linearGradient>
    </defs>
    <rect width="1200" height="310" fill="#030712" />
    <circle cx="600" cy="154" r="320" fill="url(#consoleGlow)" />
    <g opacity=".55">
      <circle cx="179" cy="207" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="195" cy="170" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="43" cy="245" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="366" cy="299" r="2" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="289" cy="259" r="2" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="836" cy="136" r="2" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="695" cy="279" r="2" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="107" cy="139" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="879" cy="308" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="225" cy="259" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="1070" cy="164" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="857" cy="108" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="529" cy="129" r="2" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="1070" cy="21" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="936" cy="5" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="211" cy="263" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="556" cy="282" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="578" cy="102" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="1168" cy="43" r="2" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="537" cy="219" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="836" cy="64" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="406" cy="128" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="139" cy="49" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="283" cy="270" r="2" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="933" cy="263" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="962" cy="244" r="2" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="1075" cy="247" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="167" cy="228" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="93" cy="216" r="2" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="307" cy="299" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="385" cy="156" r="2" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="158" cy="270" r="2" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="12" cy="127" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="74" cy="63" r="2" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="1011" cy="125" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="29" cy="234" r="2" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="946" cy="290" r="1" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="289" cy="287" r="2" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="172" cy="225" r="2" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="761" cy="217" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="833" cy="19" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="369" cy="182" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="836" cy="303" r="2" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="1002" cy="72" r="2" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="183" cy="251" r="2" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="821" cy="282" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="990" cy="100" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="318" cy="6" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="263" cy="259" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="211" cy="285" r="2" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="546" cy="7" r="2" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="1093" cy="159" r="2" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="702" cy="248" r="2" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="338" cy="160" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="858" cy="281" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="1129" cy="158" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="469" cy="63" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="215" cy="78" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="1043" cy="282" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="998" cy="292" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="492" cy="146" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="1015" cy="193" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="131" cy="165" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="891" cy="197" r="2" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="801" cy="181" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="915" cy="68" r="2" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="28" cy="152" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="937" cy="127" r="1" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="498" cy="86" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="1107" cy="284" r="1" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="758" cy="5" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="154" cy="195" r="1" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="907" cy="76" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="694" cy="193" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="908" cy="307" r="2" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="637" cy="52" r="2" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="1012" cy="206" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="371" cy="253" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="402" cy="235" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="150" cy="209" r="1" fill="#ffffff" fillOpacity="0.35" />
    </g>
    <line id="missionScan" x1="0" y1="58" x2="260" y2="58" stroke="url(#scanGrad)" strokeWidth="2" />
    <path id="missionOrbit" d="M 170 154 C 340 18, 860 18, 1030 154 C 860 290, 340 290, 170 154 Z" fill="none" stroke="#38bdf8" strokeWidth="2" strokeDasharray="16 14" opacity=".85" />
    <path d="M 280 154 C 410 80, 790 80, 920 154" fill="none" stroke="#7c3aed" strokeWidth="2" strokeDasharray="6 13" opacity=".8" />
    <circle id="nodeA" cx="282" cy="154" r="9" fill="#38bdf8" />
    <circle id="nodeB" cx="600" cy="74" r="9" fill="#a78bfa" />
    <circle id="nodeC" cx="920" cy="154" r="9" fill="#60a5fa" />
  </svg>
  <div style={{ position: 'absolute', left: 60, top: 44, width: 390, display: 'flex', flexDirection: 'column' }}>
    <div style={{ color: '#38bdf8', fontSize: 18, fontWeight: 800, letterSpacing: 2 }}>MISSION CONTROL</div>
    <div style={{ color: '#f8fafc', fontSize: 38, fontWeight: 800, marginTop: 12 }}>Building Useful Systems</div>
    <div style={{ color: '#cbd5e1', fontSize: 19, lineHeight: 1.45, marginTop: 14 }}>AI apps, production websites, 3D experiences, and data-backed tools from idea to deployment.</div>
  </div>
  <div style={{ position: 'absolute', right: 58, top: 54, width: 328, display: 'flex', flexDirection: 'column', gap: 12 }}>
    <div style={{ display: 'flex', justifyContent: 'space-between', padding: '13px 16px', borderRadius: 16, background: 'rgba(15, 23, 42, .72)', border: '1px solid rgba(56, 189, 248, .45)', color: '#e2e8f0', fontSize: 18 }}><span>Frontend</span><strong>Next.js</strong></div>
    <div style={{ display: 'flex', justifyContent: 'space-between', padding: '13px 16px', borderRadius: 16, background: 'rgba(15, 23, 42, .72)', border: '1px solid rgba(167, 139, 250, .45)', color: '#e2e8f0', fontSize: 18 }}><span>AI Layer</span><strong>RAG / OpenCV</strong></div>
    <div style={{ display: 'flex', justifyContent: 'space-between', padding: '13px 16px', borderRadius: 16, background: 'rgba(15, 23, 42, .72)', border: '1px solid rgba(96, 165, 250, .45)', color: '#e2e8f0', fontSize: 18 }}><span>3D</span><strong>Unity</strong></div>
  </div>
</div>
```

## Missions Launched

| Mission | Objective | Propulsion | Status |
|---|---|---|---|
| **PanjtanPak Developers** | Production website for a real estate and development business | Web Development, Hosting, Deployment | [In Orbit](https://www.panjtanpakdevelopers.com/) |
| **Dreams and Diamonds** | Jewelry e-commerce website with a polished customer-facing storefront | E-commerce, Web Development, Deployment | [In Orbit](https://www.dreamsanddiamonds.org/) |
| **Qanoon** | AI legal research assistant for Pakistani law with cited statute-backed answers | Next.js, RAG, Postgres, Vector Search, Vercel | [In Orbit](https://legal-rag-assistant-two.vercel.app/) |
| **2D Floor Plan to 3D** | Converts residential floor plans into interactive 3D walkthrough visualizations | OpenCV, CNNs, 3D Visualization | [In Orbit](https://fypwebsite-black.vercel.app/) |
| **TradeRank** | Marketing platform for local service businesses with dashboards and lead flows | Next.js, Tailwind CSS, SEO | On Launchpad |
| **Unity Horror Adventure** | Narrative 3D horror game with AI-based enemy behavior | Unity, C# | On Launchpad |
| **2D Coloring Game** | Interactive Unity coloring game | Unity, C# | [In Orbit](https://play.unity.com/en/user/a9058027-8fd6-4b7d-ab87-1042f4cb8055) |

<details>
<summary><strong>Open Mission Control Console</strong></summary>

<br />

```bash
$ ssh faizan@dev-station
> establishing uplink... [OK]
> booting profile.os v2.0... [OK]

PILOT    : Faizan Aslam
STACK    : Next.js | RAG | Unity | OpenCV
DATABASE : Postgres + pgvector
FOCUS    : useful products, clean systems
STATUS   : BUILDING

current trajectory:
- AI legal research tools for Pakistani law
- 2D floor plan -> 3D visualization workflows
- SEO-focused business websites and dashboards
- Unity gameplay systems with AI-driven behavior

signal strength: 100%
```

</details>

<details>
<summary><strong>Crew Log: Experience</strong></summary>

<br />

**Full-Stack Developer - ARK TechnoSolution** `2024 - 2025`
- Built and deployed full-stack web applications from frontend to database
- Integrated APIs, authentication systems, and production-ready deployment flows
- Worked with clients and design teams across the software development lifecycle

**Business Websites & E-Commerce** `2025 - 2026`
- PanjtanPak Developers: production deployment and hosting management
- Dreams and Diamonds: jewelry e-commerce platform under active development

</details>

<details>
<summary><strong>Ask Me About (open comms channel)</strong></summary>

<br />

RAG | Next.js | React | Supabase | Firebase | Postgres | OpenCV | Unity | C# | AI-assisted development | turning raw ideas into deployed products

</details>

```aura width=1200 height=84
<div
  style={{
    width: '100%',
    height: '100%',
    display: 'flex',
    position: 'relative',
    overflow: 'hidden',
    background: '#020617',
    borderRadius: 18,
  }}
>
  <style>{`
    @keyframes sweep {
      from { transform: translateX(-80px); opacity: .65; }
      to { transform: translateX(80px); opacity: 1; }
    }
    #dividerStars202 { animation: sweep 16s linear infinite alternate; }
  `}</style>
  <svg width="1200" height="84" viewBox="0 0 1200 84" style={{ position: 'absolute', left: 0, top: 0 }}>
    <defs>
      <linearGradient id="line202" x1="0" x2="1" y1="0" y2="0">
        <stop offset="0%" stopColor="#020617" />
        <stop offset="35%" stopColor="#2563eb" />
        <stop offset="65%" stopColor="#7c3aed" />
        <stop offset="100%" stopColor="#020617" />
      </linearGradient>
    </defs>
    <rect width="1200" height="84" fill="#020617" />
    <g id="dividerStars202">
      <circle cx="789" cy="82" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="401" cy="50" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="924" cy="4" r="2" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="486" cy="63" r="2" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="823" cy="41" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="952" cy="84" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="520" cy="57" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="93" cy="22" r="2" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="778" cy="33" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="413" cy="15" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="405" cy="55" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="392" cy="38" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="496" cy="44" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="786" cy="50" r="2" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="715" cy="52" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="706" cy="14" r="1" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="30" cy="10" r="2" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="1167" cy="40" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="515" cy="76" r="2" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="263" cy="71" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="273" cy="56" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="710" cy="83" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="54" cy="63" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="26" cy="7" r="2" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="785" cy="0" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="421" cy="52" r="1" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="875" cy="63" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="353" cy="9" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="479" cy="10" r="2" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="86" cy="53" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="805" cy="72" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="312" cy="31" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="1015" cy="49" r="2" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="514" cy="31" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="1123" cy="15" r="2" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="752" cy="77" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="304" cy="6" r="2" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="969" cy="43" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="466" cy="10" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="405" cy="38" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="42" cy="5" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="690" cy="25" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="29" cy="2" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="655" cy="17" r="2" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="101" cy="84" r="2" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="257" cy="36" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="666" cy="22" r="2" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="436" cy="52" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="485" cy="36" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="441" cy="26" r="2" fill="#60a5fa" fillOpacity="0.35" />
      <circle cx="689" cy="27" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="681" cy="39" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="341" cy="57" r="2" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="886" cy="48" r="2" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="159" cy="11" r="1" fill="#93c5fd" fillOpacity="0.45" />
    </g>
    <rect x="120" y="41" width="960" height="2" rx="1" fill="url(#line202)" opacity=".95" />
  </svg>
</div>
```

## The Tech Nebula

<h4>Languages</h4>
<p>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/C%23-68217A?style=for-the-badge&logo=csharp&logoColor=white" alt="C#" />
  <img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP" />
</p>

<h4>Frameworks & Engines</h4>
<p>
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white" alt="Three.js" />
  <img src="https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white" alt="Unity" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV" />
</p>

<h4>Data & Deployment</h4>
<p>
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase" />
  <img src="https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black" alt="Firebase" />
  <img src="https://img.shields.io/badge/Postgres-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="Postgres" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
</p>

## Telemetry: GitHub Stats

<p align="center">
  <img src="https://streak-stats.demolab.com?user=FaizanAslam10&theme=tokyonight&hide_border=true&background=0b0b2a&ring=7b2ff7&fire=61dafb&currStreakLabel=e6e6fa&sideLabels=e6e6fa&currStreakNum=ffffff&sideNums=ffffff&dates=8888aa" alt="GitHub Streak" />
</p>

<p align="center">
  <img width="95%" src="https://github-readme-activity-graph.vercel.app/graph?username=FaizanAslam10&bg_color=0b0b2a&color=e6e6fa&line=7b2ff7&point=61dafb&area=true&area_color=1b1b4d&hide_border=true&custom_title=Contribution%20Flight%20Path" alt="Contribution graph" />
</p>

## The Cosmic Snake

<p align="center">
  <img src="https://raw.githubusercontent.com/FaizanAslam10/FaizanAslam10/output/github-contribution-grid-snake.svg" alt="Contribution snake" />
</p>

```aura width=1200 height=84
<div
  style={{
    width: '100%',
    height: '100%',
    display: 'flex',
    position: 'relative',
    overflow: 'hidden',
    background: '#020617',
    borderRadius: 18,
  }}
>
  <style>{`
    @keyframes sweep {
      from { transform: translateX(-80px); opacity: .65; }
      to { transform: translateX(80px); opacity: 1; }
    }
    #dividerStars203 { animation: sweep 16s linear infinite alternate; }
  `}</style>
  <svg width="1200" height="84" viewBox="0 0 1200 84" style={{ position: 'absolute', left: 0, top: 0 }}>
    <defs>
      <linearGradient id="line203" x1="0" x2="1" y1="0" y2="0">
        <stop offset="0%" stopColor="#020617" />
        <stop offset="35%" stopColor="#2563eb" />
        <stop offset="65%" stopColor="#7c3aed" />
        <stop offset="100%" stopColor="#020617" />
      </linearGradient>
    </defs>
    <rect width="1200" height="84" fill="#020617" />
    <g id="dividerStars203">
      <circle cx="185" cy="5" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="59" cy="76" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="45" cy="31" r="1" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="240" cy="13" r="2" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="783" cy="56" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="610" cy="9" r="1" fill="#a78bfa" fillOpacity="0.90" />
      <circle cx="530" cy="78" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="773" cy="76" r="1" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="137" cy="80" r="2" fill="#60a5fa" fillOpacity="0.70" />
      <circle cx="888" cy="43" r="2" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="468" cy="22" r="2" fill="#93c5fd" fillOpacity="0.35" />
      <circle cx="164" cy="11" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="530" cy="33" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="93" cy="23" r="1" fill="#a78bfa" fillOpacity="0.35" />
      <circle cx="1056" cy="4" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="761" cy="5" r="2" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="800" cy="48" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="583" cy="2" r="1" fill="#ffffff" fillOpacity="0.70" />
      <circle cx="495" cy="59" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="444" cy="28" r="2" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="1141" cy="30" r="1" fill="#a78bfa" fillOpacity="0.45" />
      <circle cx="147" cy="32" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="160" cy="32" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="844" cy="13" r="2" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="253" cy="52" r="2" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="155" cy="54" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="227" cy="9" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="364" cy="15" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="982" cy="67" r="2" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="231" cy="32" r="2" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="779" cy="75" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="99" cy="51" r="1" fill="#ffffff" fillOpacity="0.35" />
      <circle cx="847" cy="59" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="865" cy="46" r="2" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="337" cy="22" r="2" fill="#ffffff" fillOpacity="0.55" />
      <circle cx="1108" cy="6" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="683" cy="57" r="2" fill="#60a5fa" fillOpacity="0.90" />
      <circle cx="284" cy="74" r="1" fill="#93c5fd" fillOpacity="0.55" />
      <circle cx="334" cy="57" r="1" fill="#93c5fd" fillOpacity="0.70" />
      <circle cx="705" cy="64" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="1032" cy="7" r="1" fill="#a78bfa" fillOpacity="0.70" />
      <circle cx="98" cy="57" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="571" cy="66" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="1034" cy="49" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="923" cy="4" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="1115" cy="35" r="1" fill="#60a5fa" fillOpacity="0.55" />
      <circle cx="140" cy="34" r="1" fill="#93c5fd" fillOpacity="0.45" />
      <circle cx="426" cy="55" r="1" fill="#60a5fa" fillOpacity="0.45" />
      <circle cx="103" cy="69" r="1" fill="#ffffff" fillOpacity="0.90" />
      <circle cx="271" cy="35" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="425" cy="14" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="94" cy="61" r="1" fill="#93c5fd" fillOpacity="0.90" />
      <circle cx="135" cy="0" r="1" fill="#ffffff" fillOpacity="0.45" />
      <circle cx="24" cy="7" r="1" fill="#a78bfa" fillOpacity="0.55" />
      <circle cx="858" cy="43" r="2" fill="#93c5fd" fillOpacity="0.90" />
    </g>
    <rect x="120" y="41" width="960" height="2" rx="1" fill="url(#line203)" opacity=".95" />
  </svg>
</div>
```

## Establish Contact

<p align="center">
  <a href="https://github.com/FaizanAslam10"><img src="assets/contact-github.svg" width="286" alt="GitHub - FaizanAslam10" /></a><a href="https://linkedin.com/in/faizan-aslam10"><img src="assets/contact-linkedin.svg" width="286" alt="LinkedIn - faizan-aslam10" /></a><a href="mailto:m.faizanaslam10@gmail.com"><img src="assets/contact-email.svg" width="286" alt="Email - m.faizanaslam10@gmail.com" /></a><img src="assets/contact-views.svg" width="286" alt="Visitor telemetry" />
</p>

<p align="center">
  <em>From Earth with code - if a mission caught your eye, drop a star. It helps the constellation grow.</em>
</p>

<!-- GALACTIC FOOTER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=140&color=0:7b2ff7,30:3d2c8d,65:1b1b4d,100:0b0b2a&section=footer" alt="footer wave" />



