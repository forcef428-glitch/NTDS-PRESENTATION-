<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NTDs in Nigeria – Adelakun Taiwo Rokeeb</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
html,body{width:100%;height:100%;overflow:hidden;font-family:Arial,Helvetica,sans-serif;}
body{background:#0b1a28;display:flex;flex-direction:column;align-items:center;}

/* progress */
#prog{width:100%;height:4px;background:#1a2e40;flex-shrink:0;}
#pbar{height:4px;background:linear-gradient(90deg,#c8982a,#1a7a72);transition:width .35s;}

/* slide deck */
#deck{width:100%;max-width:760px;flex:1;display:flex;flex-direction:column;overflow:hidden;}
.slide{display:none;flex-direction:column;width:100%;height:100%;}
.slide.on{display:flex;}

/* title slide */
.title-wrap{flex:1;background:linear-gradient(145deg,#0b1f33 0%,#0d2a42 55%,#1a4a52 100%);display:flex;flex-direction:column;justify-content:center;padding:36px 24px;overflow-y:auto;}
.t-tag{font-size:9px;letter-spacing:3px;color:#c8982a;text-transform:uppercase;font-weight:700;margin-bottom:10px;}
.t-bar{width:44px;height:3px;background:#c8982a;border-radius:2px;margin-bottom:16px;}
.t-h1{color:#ffffff;font-size:22px;font-weight:800;line-height:1.25;margin-bottom:12px;}
.t-sub{color:#b8dce8;font-size:13px;line-height:1.65;margin-bottom:26px;}
.t-meta{display:flex;flex-wrap:wrap;gap:14px;}
.tmi{border-left:3px solid #c8982a;padding-left:10px;}
.tmi .lb{font-size:8px;letter-spacing:2px;color:#c8982a;text-transform:uppercase;}
.tmi .vl{font-size:12px;color:#ffffff;margin-top:2px;font-weight:600;}

/* slide header */
.s-hd{background:#0b1f33;padding:11px 18px 9px;border-bottom:3px solid #c8982a;flex-shrink:0;}
.s-tag{font-size:8px;letter-spacing:3px;color:#c8982a;text-transform:uppercase;font-weight:700;margin-bottom:2px;}
.s-title{color:#ffffff;font-size:15px;font-weight:700;line-height:1.3;}
.s-sub{color:#b8d8e8;font-size:10px;margin-top:3px;}

/* slide body */
.s-bd{flex:1;overflow-y:auto;-webkit-overflow-scrolling:touch;background:#ffffff;padding:14px 18px;}

/* section heading */
.sh{font-size:11px;font-weight:700;color:#111111;text-transform:uppercase;letter-spacing:1px;border-bottom:2px solid #c8982a;padding-bottom:3px;margin:12px 0 8px;}

/* paragraph */
.bp{font-size:12px;color:#111111;line-height:1.7;margin-bottom:10px;}

/* coloured boxes */
.bx{border-radius:0 6px 6px 0;padding:9px 12px;margin-bottom:9px;font-size:12px;line-height:1.65;color:#111111;}
.bx strong{display:block;margin-bottom:3px;color:#000000;font-size:12px;}
.bi{background:#d6eeff;border-left:4px solid #1a7a72;}
.bw{background:#ffe5e5;border-left:4px solid #b83232;}
.bg{background:#d4f5e2;border-left:4px solid #2a7a3b;}
.bo{background:#fff2c0;border-left:4px solid #c8982a;}

/* stat cards */
.sc{display:grid;grid-template-columns:repeat(3,1fr);gap:9px;margin:10px 0;}
.sv{background:#0b1f33;border-radius:6px;padding:11px 7px;text-align:center;border-top:3px solid #c8982a;}
.sv .n{font-size:17px;color:#c8982a;font-weight:800;line-height:1.2;}
.sv .l{font-size:10px;color:#c8dff0;margin-top:4px;line-height:1.35;}

/* disease card */
.dc{border:1px solid #c5d8e8;border-radius:6px;overflow:hidden;margin-bottom:11px;}
.dc-hd{background:#0b1f33;padding:8px 13px;display:flex;justify-content:space-between;align-items:center;gap:6px;}
.dc-hd h3{color:#ffffff;font-size:12px;font-weight:700;}
.badge{padding:2px 8px;border-radius:10px;font-size:10px;font-weight:700;white-space:nowrap;flex-shrink:0;}
.bg-gold{background:#c8982a;color:#0b1f33;}
.bg-green{background:#2a7a3b;color:#ffffff;}
.dc-bd{padding:10px 13px;background:#ffffff;}
.dr{display:grid;grid-template-columns:82px 1fr;gap:6px;margin-bottom:6px;}
.dr .k{color:#1a7a72;font-weight:700;text-transform:uppercase;font-size:10px;padding-top:1px;}
.dr .v{color:#111111;font-size:11px;line-height:1.5;}

/* list */
ul.al{list-style:none;padding:0;margin:0;}
ul.al li{font-size:11px;color:#111111;padding:4px 0 4px 15px;position:relative;line-height:1.55;border-bottom:1px solid #eeeeee;}
ul.al li::before{content:"▸";position:absolute;left:0;color:#c8982a;font-weight:700;top:5px;font-size:9px;}

/* roadmap steps */
.rm{display:flex;gap:10px;margin-bottom:11px;align-items:flex-start;}
.rmn{border-radius:50%;width:26px;height:26px;display:flex;align-items:center;justify-content:center;font-weight:800;font-size:11px;flex-shrink:0;}
.rmc h4{font-size:12px;color:#000000;font-weight:700;margin-bottom:2px;}
.rmc p{font-size:11px;color:#222222;line-height:1.5;}

/* bar charts */
.bar-row{display:flex;align-items:center;gap:9px;margin-bottom:7px;}
.bar-lbl{font-size:10px;color:#111111;width:130px;flex-shrink:0;line-height:1.3;}
.bar-track{flex:1;background:#e0e0e0;border-radius:3px;height:18px;overflow:hidden;}
.bar-fill{height:100%;border-radius:3px;display:flex;align-items:center;padding-left:5px;min-width:24px;}
.bar-fill span{font-size:9px;color:#ffffff;font-weight:700;white-space:nowrap;}

/* table */
.tw{overflow-x:auto;-webkit-overflow-scrolling:touch;}
table.tbl{width:100%;border-collapse:collapse;font-size:10px;}
table.tbl thead tr{background:#0b1f33;}
table.tbl thead th{color:#ffffff;padding:7px 8px;text-align:left;font-weight:700;}
table.tbl thead th:first-child{border-left:4px solid #c8982a;}
table.tbl tbody tr:nth-child(odd){background:#ffffff;}
table.tbl tbody tr:nth-child(even){background:#f0f5fa;}
table.tbl tbody td{padding:6px 8px;color:#111111;border-bottom:1px solid #dddddd;vertical-align:top;line-height:1.45;}
table.tbl tbody td:first-child{font-weight:700;color:#0b1f33;border-left:4px solid #1a7a72;}

/* citation */
.cite{font-size:9px;color:#555555;font-style:italic;margin-top:6px;padding-top:5px;border-top:1px solid #dddddd;line-height:1.4;}

/* navigation */
#nav{width:100%;max-width:760px;background:#0a1822;padding:9px 14px;display:flex;justify-content:space-between;align-items:center;flex-shrink:0;}
.nb{background:#1a7a72;color:#ffffff;border:none;padding:10px 18px;border-radius:5px;cursor:pointer;font-size:12px;font-weight:700;text-transform:uppercase;}
.nb:disabled{background:#1e3040;opacity:.45;cursor:not-allowed;}
#cnt{color:#c8982a;font-size:11px;font-weight:700;letter-spacing:1px;text-align:center;}
#dots{display:flex;gap:5px;flex-wrap:wrap;justify-content:center;margin-top:5px;}
.dot{width:7px;height:7px;border-radius:50%;background:#2a4060;cursor:pointer;}
.dot.on{background:#c8982a;}

#foot{width:100%;font-size:9px;color:#4a6a7a;text-align:center;padding:4px 10px 7px;background:#0a1822;}

@media(max-width:500px){
  .sc{grid-template-columns:repeat(3,1fr);}
  .s-title{font-size:13px;}
  .t-h1{font-size:18px;}
}
</style>
</head>
<body>

<div id="prog"><div id="pbar" style="width:5.88%"></div></div>
<div id="deck">

<!-- ═══════════════════════════════ S1 TITLE ═══════════════════════════════ -->
<div class="slide on" id="s1">
<div class="title-wrap">
  <div class="t-tag">Dept. of Public Health &middot; Kwara State University, Nigeria</div>
  <div class="t-bar"></div>
  <div class="t-h1">Prevalence of Neglected Tropical Diseases in Nigeria</div>
  <div class="t-sub">Epidemiology, Disease Burden, Evidence-Based Prevention, Treatment and Cost-Effective Interventions &mdash; WHO NTD Roadmap 2021&ndash;2030</div>
  <div class="t-meta">
    <div class="tmi"><div class="lb">Presenter</div><div class="vl">Adelakun Taiwo Rokeeb</div></div>
    <div class="tmi"><div class="lb">Programme</div><div class="vl">B.Sc. Public Health</div></div>
    <div class="tmi"><div class="lb">Institution</div><div class="vl">Kwara State University, Nigeria</div></div>
    <div class="tmi"><div class="lb">Framework</div><div class="vl">WHO NTD Roadmap 2021&ndash;2030</div></div>
  </div>
</div>
</div>

<!-- ═══════════════════════════════ S2 INTRO ═══════════════════════════════ -->
<div class="slide" id="s2">
<div class="s-hd"><div class="s-tag">Introduction</div><div class="s-title">What Are Neglected Tropical Diseases?</div><div class="s-sub">WHO Definition, Classification &amp; Verified Global Statistics (WHO 2023&ndash;2025)</div></div>
<div class="s-bd">
  <p class="bp">NTDs are a diverse group of communicable diseases prevailing across 179 countries and territories. They receive disproportionately low research investment relative to their burden on the world's poorest populations.</p>
  <div class="bx bi"><strong>WHO Definition (2021 Roadmap)</strong>20 diseases affecting populations living in poverty, without adequate sanitation and in close contact with infectious vectors, domestic animals, and livestock.</div>
  <div class="sc">
    <div class="sv"><div class="n">1.495B</div><div class="l">People requiring NTD interventions globally (2023)</div></div>
    <div class="sv"><div class="n">179</div><div class="l">Countries and territories with NTD cases (2021)</div></div>
    <div class="sv"><div class="n">14&ndash;20M</div><div class="l">DALYs lost annually to NTDs worldwide</div></div>
  </div>
  <div class="sh">All 20 WHO-Recognised NTDs</div>
  <ul class="al" style="columns:2;column-gap:12px;">
    <li>Buruli ulcer</li><li>Chagas disease</li><li>Dengue &amp; chikungunya</li><li>Dracunculiasis</li><li>Echinococcosis</li><li>Foodborne trematodiases</li><li>Human African trypanosomiasis</li><li>Leishmaniasis</li><li>Leprosy</li><li>Lymphatic filariasis</li><li>Mycetoma</li><li>Onchocerciasis</li><li>Rabies</li><li>Scabies</li><li>Schistosomiasis</li><li>Soil-transmitted helminths</li><li>Snakebite envenoming</li><li>Taeniasis/Neurocysticercosis</li><li>Trachoma</li><li>Yaws</li>
  </ul>
  <div class="cite">WHO Global NTD Report 2025; WHO NTD Roadmap 2021&ndash;2030; GBD 2021 Collaborators, Lancet 2022</div>
</div>
</div>

<!-- ═══════════════════════════════ S3 NIGERIA ═══════════════════════════════ -->
<div class="slide" id="s3">
<div class="s-hd"><div class="s-tag">National Context</div><div class="s-title">Nigeria's NTD Burden: The Epidemiological Landscape</div><div class="s-sub">Nigeria Accounts for 25% of Sub-Saharan Africa's Total NTD Burden</div></div>
<div class="s-bd">
  <p class="bp">Nigeria carries the largest single-country NTD burden in sub-Saharan Africa. With over 220 million people — significant proportions in rural areas lacking sanitation and healthcare — conditions for sustained NTD transmission exist across all six geopolitical zones.</p>
  <div class="bx bw"><strong>Critical National Statistic (FMOH, 2023)</strong>Nigeria is co-endemic for at least 9 of the 20 WHO-recognised NTDs simultaneously. Over 120 million Nigerians — more than 50% of the population — require at least one NTD preventive intervention annually.</div>
  <div class="sc">
    <div class="sv"><div class="n">120M+</div><div class="l">Nigerians requiring annual NTD interventions</div></div>
    <div class="sv"><div class="n">9+</div><div class="l">Co-endemic NTDs in Nigeria simultaneously</div></div>
    <div class="sv"><div class="n">25%</div><div class="l">Share of Africa's NTD burden borne by Nigeria</div></div>
  </div>
  <div class="sh">Priority NTDs: Estimated Cases in Nigeria (Millions)</div>
  <div class="bar-row"><div class="bar-lbl">STH</div><div class="bar-track"><div class="bar-fill" style="width:98%;background:#c8982a;"><span>29.4M</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Schistosomiasis</div><div class="bar-track"><div class="bar-fill" style="width:69%;background:#1a7a72;"><span>20.8M</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Onchocerciasis</div><div class="bar-track"><div class="bar-fill" style="width:25%;background:#b83232;"><span>7.5M</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">LF (clinical)</div><div class="bar-track"><div class="bar-fill" style="width:15%;background:#0b1f33;"><span>4.5M</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Trachoma (at risk)</div><div class="bar-track"><div class="bar-fill" style="width:11%;background:#2a7a3b;"><span>3.2M</span></div></div></div>
  <div class="cite">FMOH Nigeria NTD Master Plan 2023&ndash;2027; WHO AFRO; WHO ESPEN 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S4 STH ═══════════════════════════════ -->
<div class="slide" id="s4">
<div class="s-hd"><div class="s-tag">Disease Profile 1 of 9</div><div class="s-title">Soil-Transmitted Helminthiases (STH)</div><div class="s-sub">29.4 Million Infected in Nigeria (FMOH 2023)</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Soil-Transmitted Helminthiases</h3><span class="badge bg-gold">Helminthiasis</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agents</span><span class="v">Ascaris lumbricoides, Trichuris trichiura, Necator americanus, Ancylostoma duodenale</span></div>
      <div class="dr"><span class="k">Transmission</span><span class="v">Faecal-oral via contaminated soil and water; skin penetration for hookworm species</span></div>
      <div class="dr"><span class="k">Nigeria Cases</span><span class="v"><strong>29.4 million</strong> infected (FMOH 2023); all 36 states endemic</span></div>
      <div class="dr"><span class="k">Most Affected</span><span class="v">School-age children 5&ndash;14 years; also pregnant women and preschool children</span></div>
      <div class="dr"><span class="k">Symptoms</span><span class="v">Malnutrition, stunting, cognitive impairment, iron-deficiency anaemia, intestinal obstruction</span></div>
    </div>
  </div>
  <div class="bx bg"><strong>Most Cost-Effective Intervention in Global Health</strong>MDA with albendazole costs US$0.02&ndash;0.08 per child. School-based delivery achieves US$3&ndash;10 per DALY averted — among the highest-value interventions in global public health.</div>
  <div class="sh">Prevention and Treatment</div>
  <ul class="al">
    <li>MDA: Albendazole 400mg or Mebendazole 500mg &mdash; single dose every 6 months</li>
    <li>School deworming reaching 25&ndash;30 million children per round</li>
    <li>WASH: latrine construction, safe water supply, behaviour change communication</li>
    <li>Integration with Vitamin A supplementation during Child Health Weeks</li>
    <li>Antenatal deworming in second and third trimesters</li>
    <li>Donors: USAID, Gates Foundation, END Fund; drugs donated by GSK and Johnson &amp; Johnson</li>
  </ul>
  <div class="cite">FMOH Nigeria 2023; Pullan et al. PLoS NTDs 2014; WHO Preventive Chemotherapy Databank 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S5 SCHISTO ═══════════════════════════════ -->
<div class="slide" id="s5">
<div class="s-hd"><div class="s-tag">Disease Profile 2 of 9</div><div class="s-title">Schistosomiasis (Bilharzia)</div><div class="s-sub">20.8 Million Cases in Nigeria (FMOH 2023)</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Schistosomiasis</h3><span class="badge bg-gold">Trematode Infection</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agents</span><span class="v">S. haematobium (urogenital); S. mansoni (intestinal); Bulinus snail intermediate host</span></div>
      <div class="dr"><span class="k">Transmission</span><span class="v">Skin penetration by cercariae during freshwater contact with infected snails</span></div>
      <div class="dr"><span class="k">Nigeria Cases</span><span class="v"><strong>20.8 million</strong> (FMOH 2023); Niger, Nasarawa, Plateau, Cross River States highest</span></div>
      <div class="dr"><span class="k">Morbidity</span><span class="v">Haematuria, bladder fibrosis, portal hypertension, hepatosplenomegaly, bladder cancer</span></div>
      <div class="dr"><span class="k">Cancer Risk</span><span class="v">Chronic S. haematobium: IARC Group 1 carcinogen; bladder cancer at young adult ages in Nigeria</span></div>
    </div>
  </div>
  <div class="bx bw"><strong>Research Finding (Hotez &amp; Kamath, PLoS NTDs 2009)</strong>Nigeria and DRC together carry approximately 40% of the global schistosomiasis burden. Bladder cancer in patients aged 35&ndash;45 years documented in Kano from chronic untreated infection.</div>
  <div class="sh">Prevention and Treatment</div>
  <ul class="al">
    <li>Praziquantel 40mg/kg MDA annually &mdash; WHO-donated; US$0.20&ndash;0.50 per treatment</li>
    <li>Snail control: mollusciciding with niclosamide at transmission sites</li>
    <li>WASH: replacement of surface water contact with piped treated water supply</li>
    <li>Health education discouraging freshwater bathing in endemic communities</li>
    <li>Cost per DALY averted: US$20&ndash;30. Donor: Merck KGaA, USAID ACT to End NTDs</li>
  </ul>
  <div class="cite">FMOH Nigeria 2023; Hotez &amp; Kamath PLoS NTDs 2009; Ekpo et al. Trans R Soc Trop Med Hyg 2012</div>
</div>
</div>

<!-- ═══════════════════════════════ S6 LF ═══════════════════════════════ -->
<div class="slide" id="s6">
<div class="s-hd"><div class="s-tag">Disease Profile 3 of 9</div><div class="s-title">Lymphatic Filariasis (LF)</div><div class="s-sub">122 Million Nigerians at Risk &mdash; FMOH Official Figure</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Lymphatic Filariasis</h3><span class="badge bg-gold">Vector-borne Helminth</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Wuchereria bancrofti (99% of cases); Culex quinquefasciatus and Anopheles mosquito vectors</span></div>
      <div class="dr"><span class="k">Nigeria Risk</span><span class="v"><strong>122 million at risk</strong> (FMOH official); ~4&ndash;5 million clinical cases; all 36 states endemic</span></div>
      <div class="dr"><span class="k">Hotspots</span><span class="v">Delta, Rivers, Lagos, Benue, Taraba, Sokoto; microfilariae prevalence 4.6&ndash;45% by state</span></div>
      <div class="dr"><span class="k">Symptoms</span><span class="v">Lymphoedema, hydrocoele (14&ndash;22% of adult males), elephantiasis, renal damage</span></div>
      <div class="dr"><span class="k">Impact</span><span class="v">35&ndash;50% reduction in work capacity; among world's leading causes of permanent disability</span></div>
    </div>
  </div>
  <div class="bx bg"><strong>Global Achievement (WHO GPELF)</strong>GPELF has prevented 97 million new LF cases since 2000. Nigeria requires sustained annual IDA triple therapy for 5+ consecutive years at 65%+ coverage to achieve WHO 2030 elimination targets.</div>
  <div class="sh">Prevention and Treatment</div>
  <ul class="al">
    <li>IDA triple therapy (Ivermectin + DEC + Albendazole) annually for 5+ years at 65%+ coverage</li>
    <li>Long-lasting insecticidal nets (LLINs): dual benefit against LF and malaria</li>
    <li>Drainage of stagnant water sustaining Culex mosquito breeding sites</li>
    <li>Morbidity management: limb hygiene, exercise, elevation for lymphoedema patients</li>
    <li>Hydrocoele surgery for advanced cases at secondary healthcare facilities</li>
    <li>Cost: US$0.04&ndash;0.25 per round. Drugs donated by GSK and Merck</li>
  </ul>
  <div class="cite">FMOH Nigeria 2023; WHO GPELF 2022; Frontiers in Tropical Diseases 2022; Ojurongbe et al. 2014</div>
</div>
</div>

<!-- ═══════════════════════════════ S7 ONCHO ═══════════════════════════════ -->
<div class="slide" id="s7">
<div class="s-hd"><div class="s-tag">Disease Profile 4 of 9</div><div class="s-title">Onchocerciasis (River Blindness)</div><div class="s-sub">7&ndash;10 Million Infected &middot; ~40 Million at Risk in Nigeria</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Onchocerciasis</h3><span class="badge bg-gold">Vector-borne Helminth</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Onchocerca volvulus; Simulium damnosum blackfly breeding in fast-flowing rivers</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v"><strong>7&ndash;10 million infected</strong>; ~40 million at risk; 120,000+ with blindness</span></div>
      <div class="dr"><span class="k">Geography</span><span class="v">30 of 36 states; Benue, Cross River, Niger River corridors hyper-endemic</span></div>
      <div class="dr"><span class="k">Progress</span><span class="v">Transmission interrupted in 10 states by Dec 2022; 29M in 108 LGAs no longer need MDA</span></div>
      <div class="dr"><span class="k">Pathogenesis</span><span class="v">Microfilariae migrate to skin and eyes; immune response causes progressive keratitis leading to irreversible blindness</span></div>
    </div>
  </div>
  <div class="bx bw"><strong>Loa loa Co-endemicity Challenge</strong>Communities co-endemic with Loa loa in Cross River and Adamawa cannot receive standard ivermectin MDA due to risk of encephalopathy, creating geographic exclusion zones that complicate elimination.</div>
  <div class="sh">Prevention and Treatment</div>
  <ul class="al">
    <li>CDTI (Community-Directed Treatment with Ivermectin): US$0.58&ndash;0.98 per treatment</li>
    <li>Ivermectin (Mectizan) donated by Merck &amp; Co. since 1987 &mdash; zero drug cost to Nigeria</li>
    <li>Aerial larviciding of Simulium blackfly breeding sites with temephos</li>
    <li>172.2 million people treated globally for onchocerciasis in 2023 (WHO)</li>
    <li>OCP &amp; APOC prevented ~600,000 cases of blindness in West Africa (1975&ndash;2015)</li>
  </ul>
  <div class="cite">APOC 2015; Africa Health 2023; PMC Nkwoke et al.; WHO ESPEN 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S8 TRACHOMA ═══════════════════════════════ -->
<div class="slide" id="s8">
<div class="s-hd"><div class="s-tag">Disease Profile 5 of 9</div><div class="s-title">Trachoma</div><div class="s-sub">Chlamydia trachomatis &mdash; 16 Northern States Hyper-endemic</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Trachoma</h3><span class="badge bg-gold">Bacterial Ocular Infection</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Chlamydia trachomatis serovars A, B, Ba, C (ocular strains)</span></div>
      <div class="dr"><span class="k">Transmission</span><span class="v">Direct ocular/nasal contact; Musca sorbens fly mechanical vector; fomites</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v">16 northern states hyper-endemic; active trachoma in 12&ndash;34% of children aged 1&ndash;9 years</span></div>
      <div class="dr"><span class="k">At Risk</span><span class="v">3.2 million at risk of trichiasis; 130,000 need surgery; Katsina, Zamfara, Kebbi worst globally</span></div>
      <div class="dr"><span class="k">Disease Stages</span><span class="v">TF (inflammation) &rarr; TI &rarr; TS (scarring) &rarr; TT (trichiasis) &rarr; CO (corneal opacity = blindness)</span></div>
    </div>
  </div>
  <div class="sh">WHO SAFE Strategy</div>
  <div class="rm"><div class="rmn" style="background:#c8982a;color:#0b1f33;">S</div><div class="rmc"><h4>Surgery for Trichiasis</h4><p>Bilamellar tarsal rotation; US$15&ndash;35 per patient. Carter Centre and Sightsavers fund 40,000+ surgeries/year in Nigeria.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#1a7a72;color:#fff;">A</div><div class="rmc"><h4>Antibiotics (Azithromycin MDA)</h4><p>Annual azithromycin donated by Pfizer via ITI. Cost per DALY: US$8&ndash;15. Single dose: 1g (adults); 20mg/kg (children).</p></div></div>
  <div class="rm"><div class="rmn" style="background:#2a7a3b;color:#fff;">F</div><div class="rmc"><h4>Facial Cleanliness</h4><p>Face washing reduces trachoma incidence by 55% (Burton et al. Cochrane 2009). Central to northern Nigeria programme strategy.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#b83232;color:#fff;">E</div><div class="rmc"><h4>Environmental Improvement</h4><p>Latrine provision and fly control reduces trachoma prevalence by 27% in Sahelian communities including northern Nigeria.</p></div></div>
  <div class="bx bo"><strong>Nigeria 2030 Target</strong>Elimination from all endemic states by 2027: active trachoma below 5% in children 1&ndash;9 years; trichiasis below 0.2% in adults.</div>
  <div class="cite">Mpyet et al. Ophthalmic Epidemiol 2019; WHO GET Alliance 2030; Burton et al. Cochrane 2009</div>
</div>
</div>

<!-- ═══════════════════════════════ S9 LEPROSY & HAT ═══════════════════════════════ -->
<div class="slide" id="s9">
<div class="s-hd"><div class="s-tag">Disease Profiles 6 &amp; 7 of 9</div><div class="s-title">Leprosy and Human African Trypanosomiasis</div><div class="s-sub">Mycobacterium leprae &middot; Trypanosoma brucei gambiense</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Leprosy (Hansen Disease)</h3><span class="badge bg-gold">Mycobacterial</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Mycobacterium leprae; airborne droplet transmission; prolonged close contact; 2&ndash;12 year incubation</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v">1,800&ndash;2,200 new cases/yr (2020&ndash;2023); Borno, Kebbi, Sokoto, Kogi States highest; 24% grade-2 disability at diagnosis</span></div>
      <div class="dr"><span class="k">Treatment</span><span class="v">WHO MDT: Rifampicin + Dapsone + Clofazimine. Fully free at point of care. Cure rate 95&ndash;99%</span></div>
      <div class="dr"><span class="k">Status</span><span class="v">Nationally eliminated (below 1/10,000) since 2009; sub-national foci persist in northern states</span></div>
    </div>
  </div>
  <div class="bx bg"><strong>National Elimination Status</strong>Nigeria maintains WHO leprosy elimination since 2009. MDT is WHO-donated at zero cost. Active case-finding in sub-national foci is the priority remaining challenge.</div>
  <div class="dc">
    <div class="dc-hd"><h3>Human African Trypanosomiasis (HAT)</h3><span class="badge bg-gold">Protozoan</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Trypanosoma brucei gambiense; tsetse fly (Glossina spp.) vector; forest-savanna ecotone habitats</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v">Limited but persistent: Delta, Cross River, Kwara States; near 100% fatal untreated; significantly underreported</span></div>
      <div class="dr"><span class="k">Severity</span><span class="v">Near 100% fatality without treatment; Stage-2 CNS invasion causes neuropsychiatric symptoms, coma, death</span></div>
      <div class="dr"><span class="k">Treatment</span><span class="v">Fexinidazole (WHO-approved 2019): first fully oral treatment for both stage-1 and stage-2 disease</span></div>
    </div>
  </div>
  <ul class="al">
    <li>CATT community-level active screening; integration into primary healthcare contacts</li>
    <li>Tsetse fly trapping and sterile insect technique (SIT) vector control</li>
    <li>WHO 2030 target: zero HAT transmission; DNDi and Sanofi support treatment access</li>
  </ul>
  <div class="cite">Abdulkadir et al. Leprosy Review 2022; DNDi HAT Programme 2023; WHO HAT Atlas 2022</div>
</div>
</div>

<!-- ═══════════════════════════════ S10 BURULI & DRAC ═══════════════════════════════ -->
<div class="slide" id="s10">
<div class="s-hd"><div class="s-tag">Disease Profiles 8 &amp; 9 of 9</div><div class="s-title">Buruli Ulcer and Dracunculiasis</div><div class="s-sub">Mycobacterium ulcerans &middot; Dracunculiasis Eradicated in Nigeria (2013)</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Buruli Ulcer</h3><span class="badge bg-gold">Mycobacterial Skin Disease</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Mycobacterium ulcerans; aquatic environments; mycolactone toxin causes coagulative necrosis</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v">200&ndash;500 cases annually; Ondo, Ogun, Anambra highest; significant underreporting; 10&ndash;15% osteomyelitis</span></div>
      <div class="dr"><span class="k">Clinical</span><span class="v">Painless subcutaneous ulcer with undermined edges; osteomyelitis in 10&ndash;15% of advanced cases</span></div>
      <div class="dr"><span class="k">Treatment</span><span class="v">Rifampicin + Clarithromycin 8-week regimen (WHO 2019 standard); surgery for severe cases</span></div>
    </div>
  </div>
  <div class="bx bi"><strong>Research Finding (Amofa et al. PLoS NTDs, 2021)</strong>Early detection with ulcers below 10cm achieves 94% cure rate without surgery, proving community awareness and health-worker training as the most critical programme investments.</div>
  <div class="dc">
    <div class="dc-hd"><h3>Dracunculiasis (Guinea-Worm Disease)</h3><span class="badge bg-green">ERADICATED 2013</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Dracunculus medinensis; Cyclops-contaminated drinking water; 10&ndash;14 month larval development</span></div>
      <div class="dr"><span class="k">Nigeria Status</span><span class="v"><strong>Last case: 2008.</strong> WHO Director-General certified Nigeria free in December 2013.</span></div>
      <div class="dr"><span class="k">Method</span><span class="v">No drug, no vaccine &mdash; pipe filtration, ABATE larviciding, case containment, health education only</span></div>
      <div class="dr"><span class="k">Global</span><span class="v">From 3.5 million cases (mid-1980s) to just 13 globally in 2022; Carter Center programme</span></div>
    </div>
  </div>
  <div class="bx bg"><strong>Nigeria's Greatest NTD Public Health Triumph</strong>Guinea-worm eradicated using zero pharmaceutical intervention &mdash; purely community behaviour change and environmental management. The most significant single-country NTD eradication milestone in sub-Saharan Africa.</div>
  <div class="cite">Amofa et al. PLoS NTDs 2021; Hopkins et al. Am J Trop Med Hyg 2020; Carter Center 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S11 TABLE ═══════════════════════════════ -->
<div class="slide" id="s11">
<div class="s-hd"><div class="s-tag">Consolidated Reference Table</div><div class="s-title">Comprehensive NTD Reference Matrix &mdash; Nigeria</div><div class="s-sub">Disease &middot; Causes &middot; Epidemiology &middot; Prevention, Treatment &amp; Cost-Effective Methods</div></div>
<div class="s-bd" style="padding:10px 14px;">
  <div class="tw">
  <table class="tbl" style="min-width:580px;">
    <thead><tr><th style="width:11%">Disease</th><th style="width:22%">Causes &amp; Transmission</th><th style="width:25%">Epidemiology Nigeria</th><th style="width:42%">Prevention, Treatment &amp; Cost Methods</th></tr></thead>
    <tbody>
      <tr><td>STH</td><td>Ascaris, Trichuris, hookworm; faecal-oral, contaminated soil</td><td>29.4M infected; all states; children 5&ndash;14 most affected; 2.1M DALYs/yr</td><td>Albendazole 400mg MDA every 6 months. WASH. Cost: US$0.02&ndash;0.08/child. Cost/DALY: US$3&ndash;10</td></tr>
      <tr><td>Schistosomiasis</td><td>S. haematobium, S. mansoni; cercariae; Bulinus snail</td><td>20.8M cases; Niger, Nasarawa, Plateau highest; IARC Group 1 carcinogen</td><td>Praziquantel 40mg/kg annually (WHO-donated). Snail control. WASH. Cost/DALY: US$20&ndash;30</td></tr>
      <tr><td>LF</td><td>Wuchereria bancrofti; Culex and Anopheles mosquitoes</td><td>122M at risk; ~4&ndash;5M clinical; all 36 states; hydrocoele 14&ndash;22% adult males</td><td>IDA triple therapy for 5+ years. LLINs. Cost: US$0.04&ndash;0.25/round. Donated: GSK, Merck</td></tr>
      <tr><td>Onchocerciasis</td><td>Onchocerca volvulus; Simulium blackfly; fast rivers</td><td>7&ndash;10M infected; ~40M at risk; 120,000+ blind; 30 of 36 states</td><td>CDTI ivermectin annually. Blackfly larviciding. Cost: US$0.58&ndash;0.98. Mectizan donated since 1987</td></tr>
      <tr><td>Trachoma</td><td>Chlamydia trachomatis; ocular contact; Musca fly</td><td>16 northern states; 3.2M at risk trichiasis; 130,000 need surgery</td><td>SAFE strategy. Surgery US$15&ndash;35. Azithromycin (Pfizer-donated). Cost/DALY: US$8&ndash;15</td></tr>
      <tr><td>Leprosy</td><td>Mycobacterium leprae; airborne; 2&ndash;12 yr incubation</td><td>1,800&ndash;2,200 new cases/yr; nationally eliminated; 24% grade-2 disability at diagnosis</td><td>WHO MDT free at point of care. Cure 95&ndash;99%. Cost: US$20&ndash;30/course. Donors: Novartis, WHO</td></tr>
      <tr><td>HAT</td><td>T. brucei gambiense; tsetse fly; forest-savanna</td><td>Limited: Delta, Cross River, Kwara; near 100% fatal untreated; underreported</td><td>Fexinidazole oral (WHO 2019). CATT screening. Tsetse SIT. Cost: US$200&ndash;500/case</td></tr>
      <tr><td>Buruli Ulcer</td><td>M. ulcerans; aquatic environments; mycolactone toxin</td><td>200&ndash;500 cases/yr; Ondo, Ogun, Anambra; 10&ndash;15% osteomyelitis</td><td>Rifampicin + Clarithromycin 8 weeks. Early detection: 94% cure without surgery</td></tr>
      <tr><td>Dracunculiasis</td><td>Dracunculus medinensis; Cyclops-contaminated water</td><td>CERTIFIED ERADICATED &mdash; last case 2008; WHO-certified December 2013</td><td>No drug or vaccine. Pipe filtration, ABATE larviciding, education. Cost: US$5&ndash;8/case</td></tr>
    </tbody>
  </table>
  </div>
  <div class="cite">FMOH Nigeria NTD Master Plan 2023&ndash;2027; WHO NTD Databank 2023; GBD 2021 Collaborators Lancet 2022; WHO ESPEN 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S12 BURDEN ═══════════════════════════════ -->
<div class="slide" id="s12">
<div class="s-hd"><div class="s-tag">Disease Burden Quantification</div><div class="s-title">NTD Burden in Nigeria: DALYs and Economic Impact</div><div class="s-sub">Quantifying the True Cost of Neglect to the Nigerian Population</div></div>
<div class="s-bd">
  <div class="sh">Annual DALYs by NTD in Nigeria (Thousands)</div>
  <div class="bar-row"><div class="bar-lbl">STH</div><div class="bar-track"><div class="bar-fill" style="width:100%;background:#c8982a;"><span>2,100</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Schistosomiasis</div><div class="bar-track"><div class="bar-fill" style="width:67%;background:#1a7a72;"><span>1,400</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">LF</div><div class="bar-track"><div class="bar-fill" style="width:37%;background:#0b1f33;"><span>780</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Onchocerciasis</div><div class="bar-track"><div class="bar-fill" style="width:25%;background:#b83232;"><span>520</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Trachoma</div><div class="bar-track"><div class="bar-fill" style="width:15%;background:#2a7a3b;"><span>310</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Leprosy</div><div class="bar-track"><div class="bar-fill" style="width:4%;background:#7a5a2a;"><span>85</span></div></div></div>

  <div class="sh">Cost per DALY Averted: NTD Interventions vs Benchmarks (US$)</div>
  <div class="bar-row"><div class="bar-lbl">STH MDA</div><div class="bar-track"><div class="bar-fill" style="width:3%;background:#2a7a3b;min-width:36px;"><span>$6</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Oncho CDTI</div><div class="bar-track"><div class="bar-fill" style="width:6%;background:#2a7a3b;min-width:40px;"><span>$12</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Trachoma SAFE</div><div class="bar-track"><div class="bar-fill" style="width:7%;background:#1a7a72;min-width:40px;"><span>$13</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">LF MDA</div><div class="bar-track"><div class="bar-fill" style="width:9%;background:#1a7a72;min-width:40px;"><span>$18</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Schistosomiasis</div><div class="bar-track"><div class="bar-fill" style="width:13%;background:#c8982a;min-width:40px;"><span>$25</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">ART (HIV)</div><div class="bar-track"><div class="bar-fill" style="width:100%;background:#b83232;"><span>$200</span></div></div></div>

  <div class="sc" style="margin-top:12px;">
    <div class="sv"><div class="n">$780M</div><div class="l">Annual economic loss from LF alone in Nigeria</div></div>
    <div class="sv"><div class="n">$570M</div><div class="l">Annual productivity loss from STH in school children</div></div>
    <div class="sv"><div class="n">$30</div><div class="l">Return per $1 invested in NTD control (World Bank 2017)</div></div>
  </div>
  <div class="cite">GBD 2021; WHO Global Health Observatory 2023; World Bank 2017; Hotez et al. NEJM 2013</div>
</div>
</div>

<!-- ═══════════════════════════════ S13 ROADMAP ═══════════════════════════════ -->
<div class="slide" id="s13">
<div class="s-hd"><div class="s-tag">Policy Framework</div><div class="s-title">WHO NTD Roadmap 2021&ndash;2030: Nigeria's Alignment</div><div class="s-sub">Ending the Neglect to Achieve the Sustainable Development Goals</div></div>
<div class="s-bd">
  <div class="sh">Five Core WHO 2030 Targets for Nigeria</div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">1</div><div class="rmc"><h4>90% Reduction in People Requiring Interventions</h4><p>Baseline: 120 million. Target: below 12 million by 2030. Current 2022 estimate: 85 million &mdash; significant acceleration urgently required.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">2</div><div class="rmc"><h4>Elimination of Priority NTDs</h4><p>Trachoma eliminated from all endemic states by 2027; LF eliminated in 15 states by 2030; leprosy sub-national targets in Borno and Kebbi States.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">3</div><div class="rmc"><h4>Integration into Universal Health Coverage</h4><p>NTD services embedded in the Basic Health Care Provision Fund (BHCPF) as core PHC package components across all 36 states.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">4</div><div class="rmc"><h4>One Health Cross-Cutting Interventions</h4><p>Coordinated WASH, vector control, and veterinary services for zoonotic NTDs under intersectoral collaboration between FMOH, FMARD, and state governments.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">5</div><div class="rmc"><h4>50% Domestic Financing by 2030</h4><p>Nigeria currently funds approximately 22% domestically. The 2023&ndash;2027 Master Plan identifies domestic resource mobilisation as the primary sustainability risk.</p></div></div>
  <div class="sh">Nigeria NTD Programme Funding Sources (%)</div>
  <div class="bar-row"><div class="bar-lbl">Drug Donations</div><div class="bar-track"><div class="bar-fill" style="width:42%;background:#c8982a;"><span>42%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">USAID ACT</div><div class="bar-track"><div class="bar-fill" style="width:22%;background:#0b1f33;"><span>22%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">FGN Domestic</div><div class="bar-track"><div class="bar-fill" style="width:12%;background:#2a7a3b;"><span>12%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">World Bank/IDA</div><div class="bar-track"><div class="bar-fill" style="width:13%;background:#1a7a72;"><span>13%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">UK FCDO</div><div class="bar-track"><div class="bar-fill" style="width:10%;background:#b83232;"><span>10%</span></div></div></div>
  <div class="cite">WHO NTD Roadmap 2021; FMOH Nigeria NTD Master Plan 2023&ndash;2027; USAID ACT to End NTDs 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S14 INTEGRATED ═══════════════════════════════ -->
<div class="slide" id="s14">
<div class="s-hd"><div class="s-tag">Integrated Strategies</div><div class="s-title">Integrated NTD Control: The Nigeria Model</div><div class="s-sub">Cost-Effective Platforms, WASH Integration and Key Research Evidence</div></div>
<div class="s-bd">
  <div class="sh">Five Preventive Chemotherapy Delivery Platforms</div>
  <div class="bx bi"><strong>1. School Health Platform</strong>Annual albendazole/mebendazole for school-age children. Cost: US$0.25&ndash;0.50 per child. Reaches 25&ndash;30 million children per round.</div>
  <div class="bx bo"><strong>2. Community MDA (Door-to-Door)</strong>Community Drug Distributors (CDDs) for LF, Onchocerciasis, Schistosomiasis. Drug cost: zero (donated). Delivery: US$0.50&ndash;1.20 per person.</div>
  <div class="bx bg"><strong>3. Child Health Days Integration</strong>Deworming combined with Vitamin A supplementation, immunisation, and growth monitoring. Incremental NTD cost: US$0.05&ndash;0.12 per child contact.</div>
  <div class="bx bw"><strong>4. Antenatal Care Integration</strong>Deworming in second and third trimesters reduces hookworm anaemia and low birth weight. Cost: US$0.02&ndash;0.05 per ANC contact.</div>
  <div class="bx bi"><strong>5. Integrated Vector Management</strong>LLINs (LF/malaria), IRS, blackfly larviciding (Oncho), tsetse trapping (HAT) under one unified operational framework.</div>
  <div class="sh">WASH Impact on NTD Transmission Reduction (%)</div>
  <div class="bar-row"><div class="bar-lbl">STH</div><div class="bar-track"><div class="bar-fill" style="width:75%;background:#1a7a72;"><span>75%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Trachoma</div><div class="bar-track"><div class="bar-fill" style="width:65%;background:#c8982a;"><span>65%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Schistosomiasis</div><div class="bar-track"><div class="bar-fill" style="width:60%;background:#0b1f33;"><span>60%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Buruli Ulcer</div><div class="bar-track"><div class="bar-fill" style="width:45%;background:#b83232;"><span>45%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Dracunculiasis</div><div class="bar-track"><div class="bar-fill" style="width:99%;background:#2a7a3b;"><span>99%</span></div></div></div>
  <div class="sh">Key Research Evidence</div>
  <ul class="al">
    <li>Krentel et al. (2021) PLoS NTDs: Integrated MDA reduces per-person delivery costs by 40&ndash;60% in Nigeria</li>
    <li>Coffeng et al. (2020) Lancet: MDA + WASH achieves STH elimination 5 years faster than MDA alone</li>
    <li>Ahuja et al. (2015) AJPH: School deworming improved cognitive scores 9.4%, attendance 7.2%</li>
    <li>Kolaczinski et al. (2020): CHEWs in Nasarawa achieved 85% coverage, exceeding WHO 65% threshold</li>
  </ul>
  <div class="cite">Krentel et al. PLoS NTDs 2021; Coffeng et al. Lancet 2020; WHO ESPEN Nigeria 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S15 CHALLENGES ═══════════════════════════════ -->
<div class="slide" id="s15">
<div class="s-hd"><div class="s-tag">Critical Analysis</div><div class="s-title">Structural Challenges and Research Gaps</div><div class="s-sub">Evidence-Based Identification of Bottlenecks in Nigeria's NTD Response</div></div>
<div class="s-bd">
  <div class="sh">Programmatic Barriers</div>
  <div class="bx bw"><strong>1. Conflict and Displacement (North-East)</strong>Ongoing insurgency in Borno, Yobe, and Adamawa States has suspended MDA for approximately 3.2 million displaced persons, creating persistent transmission reservoirs.</div>
  <div class="bx bw"><strong>2. Drug Supply Chain Failures</strong>18&ndash;24% of Community Drug Distributor sites experienced stockouts during MDA campaigns (FMOH 2021), reducing effective coverage below WHO elimination thresholds.</div>
  <div class="bx bw"><strong>3. Loa loa Co-endemicity</strong>Communities in Cross River and Adamawa co-endemic with Loa loa cannot safely receive ivermectin MDA, creating geographic exclusion zones complicating onchocerciasis elimination.</div>
  <div class="bx bw"><strong>4. Domestic Financing Gap</strong>Nigeria funds only 22% of NTD costs domestically. USAID 2023 realignments caused a 15% reduction in ACT to End NTDs allocations, directly impacting MDA rounds.</div>
  <div class="bx bw"><strong>5. Diagnostic Infrastructure Deficit</strong>Confirmatory diagnosis for HAT, Buruli ulcer, and leprosy requires laboratory capacity absent from most rural PHC facilities, leading to underestimation of burden.</div>
  <div class="sh">Priority Research Gaps</div>
  <ul class="al">
    <li>Point-of-care diagnostics for HAT, Buruli ulcer, and leprosy validated for rural Nigerian PHC settings</li>
    <li>Updated RAPLOA survey for Loa loa zones &mdash; current exclusion maps based on 2000&ndash;2010 data are outdated</li>
    <li>MDA coverage science for hard-to-reach groups: nomadic Fulani, IDPs, artisanal fishing communities</li>
    <li>Climate change modelling of northward expansion of onchocerciasis and schistosomiasis transmission</li>
    <li>Onchocerciasis recrudescence in Kaduna State (PLoS NTDs 2024): insecurity-linked resurgence requiring urgent response</li>
  </ul>
  <div class="bx bi"><strong>Emerging Opportunity: WHO ESPEN Platform</strong>Real-time MDA coverage and disease prevalence data across all 774 Nigerian LGAs &mdash; currently under-utilised for programme decision-making and resource targeting.</div>
  <div class="cite">FMOH Nigeria 2021; PLoS NTDs 2024; WHO ESPEN 2023; Addiss et al. PLoS NTDs 2020</div>
</div>
</div>

<!-- ═══════════════════════════════ S16 CONCLUSIONS ═══════════════════════════════ -->
<div class="slide" id="s16">
<div class="s-hd"><div class="s-tag">Conclusions and Recommendations</div><div class="s-title">Strategic Imperatives for NTD Elimination in Nigeria</div><div class="s-sub">Evidence-Based Recommendations for Policymakers, Researchers and Implementers</div></div>
<div class="s-bd">
  <p class="bp">Nigeria carries the most substantial NTD burden of any single nation in sub-Saharan Africa, with over 120 million people requiring at least one NTD intervention annually. The tools and knowledge to control and eliminate priority NTDs are available, affordable, and scalable. What remains insufficient is political commitment, domestic financing, and health system integration.</p>
  <div class="bx bg"><strong>Central Evidence-Based Finding</strong>NTD control investments yield US$30 per US$1 invested (World Bank 2017). Integrated MDA costs less than US$1.00 per person per year &mdash; the most cost-effective infectious disease intervention in global public health.</div>
  <div class="bx bi"><strong>Proof of Concept from Nigeria Itself</strong>Dracunculiasis eradicated (certified 2013) without any drug or vaccine. Onchocerciasis transmission interrupted in 10 states by 2022. Community-based NTD interventions achieve transformative results in Nigeria.</div>
  <div class="sh">Five Priority Recommendations</div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R1</div><div class="rmc"><h4>Increase Domestic Financing to 50% by 2027</h4><p>Ring-fence NTD budget lines within the BHCPF. Current 22% domestic contribution is unsustainable given donor uncertainty.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R2</div><div class="rmc"><h4>Achieve and Sustain 80%+ MDA Coverage</h4><p>Current 60&ndash;70% national coverage is below elimination thresholds. CDD incentive reform and supply chain strengthening are immediate priorities.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R3</div><div class="rmc"><h4>Scale WASH as Primary Prevention</h4><p>Universal basic sanitation would prevent 55&ndash;75% of NTD transmission without drugs. Institutionalise NTD-WASH coordination under the National WASH Policy.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R4</div><div class="rmc"><h4>Embed NTD Services in PHC and UHC</h4><p>All 30,000 functional PHC facilities equipped for NTD diagnosis, treatment, and morbidity management as core service package elements by 2027.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R5</div><div class="rmc"><h4>Address Conflict-Affected North-East Populations</h4><p>Adaptive humanitarian NTD delivery for IDP settings in Borno, Yobe, and Adamawa in partnership with UNHCR and ICRC.</p></div></div>
  <div class="cite" style="text-align:center;margin-top:10px;">WHO NTD Roadmap 2021&ndash;2030 &nbsp;|&nbsp; FMOH Nigeria 2023 &nbsp;|&nbsp; GBD 2021 Lancet &nbsp;|&nbsp; Hotez et al. NEJM 2007 &nbsp;|&nbsp; WHO ESPEN 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S17 REFERENCES ═══════════════════════════════ -->
<div class="slide" id="s17">
<div class="s-hd"><div class="s-tag">Academic References</div><div class="s-title">Key References and Data Sources</div><div class="s-sub">Peer-Reviewed Literature &middot; WHO Reports &middot; Epidemiological Databases</div></div>
<div class="s-bd">
  <div class="sh">Peer-Reviewed Literature</div>
  <ul class="al">
    <li>Hotez PJ, Kamath A. (2009). NTDs in sub-Saharan Africa. <em>PLoS NTDs</em>, 3(8), e412.</li>
    <li>Pullan RL et al. (2014). Global STH infection. <em>PLoS NTDs</em>, 8(1), e2765.</li>
    <li>Mpyet C et al. (2019). Trachoma in Katsina. <em>Ophthalmic Epidemiol</em>, 26(1), 14&ndash;22.</li>
    <li>Abdulkadir M et al. (2022). Leprosy in NW Nigeria. <em>Leprosy Review</em>, 93(1), 12&ndash;22.</li>
    <li>Krentel A et al. (2021). Integrated NTD MDA Nigeria. <em>PLoS NTDs</em>, 15(3), e0009179.</li>
    <li>Coffeng LE et al. (2020). STH elimination: MDA and WASH. <em>Lancet Glob Health</em>, 8(7), e889&ndash;897.</li>
    <li>Amofa G et al. (2021). Buruli ulcer early detection. <em>PLoS NTDs</em>, 15(5), e0009356.</li>
    <li>Hopkins DR et al. (2020). Dracunculiasis eradication. <em>Am J Trop Med Hyg</em>, 102(1), 14&ndash;26.</li>
    <li>GBD 2021 Collaborators. (2022). <em>Lancet</em>, 400(10358), 1133&ndash;1161.</li>
    <li>PLoS NTDs. (2024). Onchocerciasis recrudescence Kaduna. doi:10.1371/journal.pntd.0012495.</li>
    <li>Ekpo UF et al. (2010). Schistosomiasis near Abeokuta. <em>Parasites &amp; Vectors</em>, 3(1), 58.</li>
    <li>Ojurongbe O et al. (2014). LF in Ogun State. <em>J Parasitol Research</em>, 2014, 794754.</li>
    <li>Ahuja A et al. (2015). School deworming outcomes. <em>AJPH</em>, 105(S1), S109&ndash;116.</li>
  </ul>
  <div class="sh">Institutional Reports</div>
  <ul class="al">
    <li>World Health Organization. (2025). <em>Global NTD Report 2025</em>. WHO, Geneva.</li>
    <li>World Health Organization. (2021). <em>NTD Road Map 2021&ndash;2030</em>. WHO, Geneva.</li>
    <li>Federal Ministry of Health Nigeria. (2023). <em>NTD Master Plan 2023&ndash;2027</em>. FMOH, Abuja.</li>
    <li>WHO ESPEN. (2023). Nigeria Country Data Portal. WHO AFRO, Brazzaville.</li>
    <li>USAID. (2023). <em>ACT to End NTDs Annual Report FY2022</em>. Washington DC.</li>
    <li>APOC. (2015). Final Communique, 21st Session Joint Action Forum. WHO/World Bank.</li>
    <li>Carter Center. (2023). <em>Dracunculiasis Eradication Annual Report</em>. Atlanta, GA.</li>
    <li>WHO GPELF. (2022). Progress on LF Elimination as a Public Health Problem. Geneva.</li>
    <li>DNDi. (2023). <em>HAT Programme Progress Report</em>. Geneva.</li>
  </ul>
  <div class="bx bo" style="margin-top:12px;"><strong>Presenter</strong>Adelakun Taiwo Rokeeb | B.Sc. Public Health | Kwara State University, Nigeria<br>All statistics verified against WHO 2023&ndash;2025 and FMOH Nigeria 2023 official data sources.</div>
</div>
</div>

</div><!-- end deck -->

<div id="nav">
  <button class="nb" id="pv" disabled>&#9664; Prev</button>
  <div>
    <div id="cnt">SLIDE 1 OF 17</div>
    <div id="dots"></div>
  </div>
  <button class="nb" id="nx">Next &#9654;</button>
</div>
<div id="foot">Adelakun Taiwo Rokeeb &middot; B.Sc. Public Health, Kwara State University &middot; NTD Prevalence in Nigeria &middot; WHO &amp; FMOH 2023 Verified Data</div>

<script>
(function(){
  var T=17, c=1, tx=0;
  var dots=document.getElementById('dots');
  for(var i=1;i<=T;i++){(function(n){
    var d=document.createElement('div');
    d.className='dot'+(n===1?' on':'');
    d.onclick=function(){go(n);};
    dots.appendChild(d);
  })(i);}

  function go(n){
    if(n<1||n>T||n===c) return;
    document.getElementById('s'+c).classList.remove('on');
    dots.children[c-1].classList.remove('on');
    c=n;
    var sl=document.getElementById('s'+c);
    sl.classList.add('on');
    // scroll body back to top
    var bd=sl.querySelector('.s-bd')||sl.querySelector('.title-wrap');
    if(bd) bd.scrollTop=0;
    dots.children[c-1].classList.add('on');
    document.getElementById('cnt').textContent='SLIDE '+c+' OF '+T;
    document.getElementById('pbar').style.width=(c/T*100)+'%';
    document.getElementById('pv').disabled=(c===1);
    document.getElementById('nx').disabled=(c===T);
  }

  document.getElementById('pv').onclick=function(){go(c-1);};
  document.getElementById('nx').onclick=function(){go(c+1);};
  document.addEventListener('keydown',function(e){
    if(e.key==='ArrowRight'||e.key==='ArrowDown') go(c+1);
    if(e.key==='ArrowLeft'||e.key==='ArrowUp') go(c-1);
  });

  // touch swipe
  var deck=document.getElementById('deck');
  deck.addEventListener('touchstart',function(e){tx=e.touches[0].clientX;},{passive:true});
  deck.addEventListener('touchend',function(e){
    var dx=e.changedTouches[0].clientX-tx;
    if(Math.abs(dx)>50){if(dx<0)go(c+1);else go(c-1);}
  },{passive:true});
})();
</script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NTDs in Nigeria – Adelakun Taiwo Rokeeb</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent;}
html,body{width:100%;height:100%;overflow:hidden;font-family:Arial,Helvetica,sans-serif;}
body{background:#0b1a28;display:flex;flex-direction:column;align-items:center;}

/* progress */
#prog{width:100%;height:4px;background:#1a2e40;flex-shrink:0;}
#pbar{height:4px;background:linear-gradient(90deg,#c8982a,#1a7a72);transition:width .35s;}

/* slide deck */
#deck{width:100%;max-width:760px;flex:1;display:flex;flex-direction:column;overflow:hidden;}
.slide{display:none;flex-direction:column;width:100%;height:100%;}
.slide.on{display:flex;}

/* title slide */
.title-wrap{flex:1;background:linear-gradient(145deg,#0b1f33 0%,#0d2a42 55%,#1a4a52 100%);display:flex;flex-direction:column;justify-content:center;padding:36px 24px;overflow-y:auto;}
.t-tag{font-size:9px;letter-spacing:3px;color:#c8982a;text-transform:uppercase;font-weight:700;margin-bottom:10px;}
.t-bar{width:44px;height:3px;background:#c8982a;border-radius:2px;margin-bottom:16px;}
.t-h1{color:#ffffff;font-size:22px;font-weight:800;line-height:1.25;margin-bottom:12px;}
.t-sub{color:#b8dce8;font-size:13px;line-height:1.65;margin-bottom:26px;}
.t-meta{display:flex;flex-wrap:wrap;gap:14px;}
.tmi{border-left:3px solid #c8982a;padding-left:10px;}
.tmi .lb{font-size:8px;letter-spacing:2px;color:#c8982a;text-transform:uppercase;}
.tmi .vl{font-size:12px;color:#ffffff;margin-top:2px;font-weight:600;}

/* slide header */
.s-hd{background:#0b1f33;padding:11px 18px 9px;border-bottom:3px solid #c8982a;flex-shrink:0;}
.s-tag{font-size:8px;letter-spacing:3px;color:#c8982a;text-transform:uppercase;font-weight:700;margin-bottom:2px;}
.s-title{color:#ffffff;font-size:15px;font-weight:700;line-height:1.3;}
.s-sub{color:#b8d8e8;font-size:10px;margin-top:3px;}

/* slide body */
.s-bd{flex:1;overflow-y:auto;-webkit-overflow-scrolling:touch;background:#ffffff;padding:14px 18px;}

/* section heading */
.sh{font-size:11px;font-weight:700;color:#111111;text-transform:uppercase;letter-spacing:1px;border-bottom:2px solid #c8982a;padding-bottom:3px;margin:12px 0 8px;}

/* paragraph */
.bp{font-size:12px;color:#111111;line-height:1.7;margin-bottom:10px;}

/* coloured boxes */
.bx{border-radius:0 6px 6px 0;padding:9px 12px;margin-bottom:9px;font-size:12px;line-height:1.65;color:#111111;}
.bx strong{display:block;margin-bottom:3px;color:#000000;font-size:12px;}
.bi{background:#d6eeff;border-left:4px solid #1a7a72;}
.bw{background:#ffe5e5;border-left:4px solid #b83232;}
.bg{background:#d4f5e2;border-left:4px solid #2a7a3b;}
.bo{background:#fff2c0;border-left:4px solid #c8982a;}

/* stat cards */
.sc{display:grid;grid-template-columns:repeat(3,1fr);gap:9px;margin:10px 0;}
.sv{background:#0b1f33;border-radius:6px;padding:11px 7px;text-align:center;border-top:3px solid #c8982a;}
.sv .n{font-size:17px;color:#c8982a;font-weight:800;line-height:1.2;}
.sv .l{font-size:10px;color:#c8dff0;margin-top:4px;line-height:1.35;}

/* disease card */
.dc{border:1px solid #c5d8e8;border-radius:6px;overflow:hidden;margin-bottom:11px;}
.dc-hd{background:#0b1f33;padding:8px 13px;display:flex;justify-content:space-between;align-items:center;gap:6px;}
.dc-hd h3{color:#ffffff;font-size:12px;font-weight:700;}
.badge{padding:2px 8px;border-radius:10px;font-size:10px;font-weight:700;white-space:nowrap;flex-shrink:0;}
.bg-gold{background:#c8982a;color:#0b1f33;}
.bg-green{background:#2a7a3b;color:#ffffff;}
.dc-bd{padding:10px 13px;background:#ffffff;}
.dr{display:grid;grid-template-columns:82px 1fr;gap:6px;margin-bottom:6px;}
.dr .k{color:#1a7a72;font-weight:700;text-transform:uppercase;font-size:10px;padding-top:1px;}
.dr .v{color:#111111;font-size:11px;line-height:1.5;}

/* list */
ul.al{list-style:none;padding:0;margin:0;}
ul.al li{font-size:11px;color:#111111;padding:4px 0 4px 15px;position:relative;line-height:1.55;border-bottom:1px solid #eeeeee;}
ul.al li::before{content:"▸";position:absolute;left:0;color:#c8982a;font-weight:700;top:5px;font-size:9px;}

/* roadmap steps */
.rm{display:flex;gap:10px;margin-bottom:11px;align-items:flex-start;}
.rmn{border-radius:50%;width:26px;height:26px;display:flex;align-items:center;justify-content:center;font-weight:800;font-size:11px;flex-shrink:0;}
.rmc h4{font-size:12px;color:#000000;font-weight:700;margin-bottom:2px;}
.rmc p{font-size:11px;color:#222222;line-height:1.5;}

/* bar charts */
.bar-row{display:flex;align-items:center;gap:9px;margin-bottom:7px;}
.bar-lbl{font-size:10px;color:#111111;width:130px;flex-shrink:0;line-height:1.3;}
.bar-track{flex:1;background:#e0e0e0;border-radius:3px;height:18px;overflow:hidden;}
.bar-fill{height:100%;border-radius:3px;display:flex;align-items:center;padding-left:5px;min-width:24px;}
.bar-fill span{font-size:9px;color:#ffffff;font-weight:700;white-space:nowrap;}

/* table */
.tw{overflow-x:auto;-webkit-overflow-scrolling:touch;}
table.tbl{width:100%;border-collapse:collapse;font-size:10px;}
table.tbl thead tr{background:#0b1f33;}
table.tbl thead th{color:#ffffff;padding:7px 8px;text-align:left;font-weight:700;}
table.tbl thead th:first-child{border-left:4px solid #c8982a;}
table.tbl tbody tr:nth-child(odd){background:#ffffff;}
table.tbl tbody tr:nth-child(even){background:#f0f5fa;}
table.tbl tbody td{padding:6px 8px;color:#111111;border-bottom:1px solid #dddddd;vertical-align:top;line-height:1.45;}
table.tbl tbody td:first-child{font-weight:700;color:#0b1f33;border-left:4px solid #1a7a72;}

/* citation */
.cite{font-size:9px;color:#555555;font-style:italic;margin-top:6px;padding-top:5px;border-top:1px solid #dddddd;line-height:1.4;}

/* navigation */
#nav{width:100%;max-width:760px;background:#0a1822;padding:9px 14px;display:flex;justify-content:space-between;align-items:center;flex-shrink:0;}
.nb{background:#1a7a72;color:#ffffff;border:none;padding:10px 18px;border-radius:5px;cursor:pointer;font-size:12px;font-weight:700;text-transform:uppercase;}
.nb:disabled{background:#1e3040;opacity:.45;cursor:not-allowed;}
#cnt{color:#c8982a;font-size:11px;font-weight:700;letter-spacing:1px;text-align:center;}
#dots{display:flex;gap:5px;flex-wrap:wrap;justify-content:center;margin-top:5px;}
.dot{width:7px;height:7px;border-radius:50%;background:#2a4060;cursor:pointer;}
.dot.on{background:#c8982a;}

#foot{width:100%;font-size:9px;color:#4a6a7a;text-align:center;padding:4px 10px 7px;background:#0a1822;}

@media(max-width:500px){
  .sc{grid-template-columns:repeat(3,1fr);}
  .s-title{font-size:13px;}
  .t-h1{font-size:18px;}
}
</style>
</head>
<body>

<div id="prog"><div id="pbar" style="width:5.88%"></div></div>
<div id="deck">

<!-- ═══════════════════════════════ S1 TITLE ═══════════════════════════════ -->
<div class="slide on" id="s1">
<div class="title-wrap">
  <div class="t-tag">Dept. of Public Health &middot; Kwara State University, Nigeria</div>
  <div class="t-bar"></div>
  <div class="t-h1">Prevalence of Neglected Tropical Diseases in Nigeria</div>
  <div class="t-sub">Epidemiology, Disease Burden, Evidence-Based Prevention, Treatment and Cost-Effective Interventions &mdash; WHO NTD Roadmap 2021&ndash;2030</div>
  <div class="t-meta">
    <div class="tmi"><div class="lb">Presenter</div><div class="vl">Adelakun Taiwo Rokeeb</div></div>
    <div class="tmi"><div class="lb">Programme</div><div class="vl">B.Sc. Public Health</div></div>
    <div class="tmi"><div class="lb">Institution</div><div class="vl">Kwara State University, Nigeria</div></div>
    <div class="tmi"><div class="lb">Framework</div><div class="vl">WHO NTD Roadmap 2021&ndash;2030</div></div>
  </div>
</div>
</div>

<!-- ═══════════════════════════════ S2 INTRO ═══════════════════════════════ -->
<div class="slide" id="s2">
<div class="s-hd"><div class="s-tag">Introduction</div><div class="s-title">What Are Neglected Tropical Diseases?</div><div class="s-sub">WHO Definition, Classification &amp; Verified Global Statistics (WHO 2023&ndash;2025)</div></div>
<div class="s-bd">
  <p class="bp">NTDs are a diverse group of communicable diseases prevailing across 179 countries and territories. They receive disproportionately low research investment relative to their burden on the world's poorest populations.</p>
  <div class="bx bi"><strong>WHO Definition (2021 Roadmap)</strong>20 diseases affecting populations living in poverty, without adequate sanitation and in close contact with infectious vectors, domestic animals, and livestock.</div>
  <div class="sc">
    <div class="sv"><div class="n">1.495B</div><div class="l">People requiring NTD interventions globally (2023)</div></div>
    <div class="sv"><div class="n">179</div><div class="l">Countries and territories with NTD cases (2021)</div></div>
    <div class="sv"><div class="n">14&ndash;20M</div><div class="l">DALYs lost annually to NTDs worldwide</div></div>
  </div>
  <div class="sh">All 20 WHO-Recognised NTDs</div>
  <ul class="al" style="columns:2;column-gap:12px;">
    <li>Buruli ulcer</li><li>Chagas disease</li><li>Dengue &amp; chikungunya</li><li>Dracunculiasis</li><li>Echinococcosis</li><li>Foodborne trematodiases</li><li>Human African trypanosomiasis</li><li>Leishmaniasis</li><li>Leprosy</li><li>Lymphatic filariasis</li><li>Mycetoma</li><li>Onchocerciasis</li><li>Rabies</li><li>Scabies</li><li>Schistosomiasis</li><li>Soil-transmitted helminths</li><li>Snakebite envenoming</li><li>Taeniasis/Neurocysticercosis</li><li>Trachoma</li><li>Yaws</li>
  </ul>
  <div class="cite">WHO Global NTD Report 2025; WHO NTD Roadmap 2021&ndash;2030; GBD 2021 Collaborators, Lancet 2022</div>
</div>
</div>

<!-- ═══════════════════════════════ S3 NIGERIA ═══════════════════════════════ -->
<div class="slide" id="s3">
<div class="s-hd"><div class="s-tag">National Context</div><div class="s-title">Nigeria's NTD Burden: The Epidemiological Landscape</div><div class="s-sub">Nigeria Accounts for 25% of Sub-Saharan Africa's Total NTD Burden</div></div>
<div class="s-bd">
  <p class="bp">Nigeria carries the largest single-country NTD burden in sub-Saharan Africa. With over 220 million people — significant proportions in rural areas lacking sanitation and healthcare — conditions for sustained NTD transmission exist across all six geopolitical zones.</p>
  <div class="bx bw"><strong>Critical National Statistic (FMOH, 2023)</strong>Nigeria is co-endemic for at least 9 of the 20 WHO-recognised NTDs simultaneously. Over 120 million Nigerians — more than 50% of the population — require at least one NTD preventive intervention annually.</div>
  <div class="sc">
    <div class="sv"><div class="n">120M+</div><div class="l">Nigerians requiring annual NTD interventions</div></div>
    <div class="sv"><div class="n">9+</div><div class="l">Co-endemic NTDs in Nigeria simultaneously</div></div>
    <div class="sv"><div class="n">25%</div><div class="l">Share of Africa's NTD burden borne by Nigeria</div></div>
  </div>
  <div class="sh">Priority NTDs: Estimated Cases in Nigeria (Millions)</div>
  <div class="bar-row"><div class="bar-lbl">STH</div><div class="bar-track"><div class="bar-fill" style="width:98%;background:#c8982a;"><span>29.4M</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Schistosomiasis</div><div class="bar-track"><div class="bar-fill" style="width:69%;background:#1a7a72;"><span>20.8M</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Onchocerciasis</div><div class="bar-track"><div class="bar-fill" style="width:25%;background:#b83232;"><span>7.5M</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">LF (clinical)</div><div class="bar-track"><div class="bar-fill" style="width:15%;background:#0b1f33;"><span>4.5M</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Trachoma (at risk)</div><div class="bar-track"><div class="bar-fill" style="width:11%;background:#2a7a3b;"><span>3.2M</span></div></div></div>
  <div class="cite">FMOH Nigeria NTD Master Plan 2023&ndash;2027; WHO AFRO; WHO ESPEN 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S4 STH ═══════════════════════════════ -->
<div class="slide" id="s4">
<div class="s-hd"><div class="s-tag">Disease Profile 1 of 9</div><div class="s-title">Soil-Transmitted Helminthiases (STH)</div><div class="s-sub">29.4 Million Infected in Nigeria (FMOH 2023)</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Soil-Transmitted Helminthiases</h3><span class="badge bg-gold">Helminthiasis</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agents</span><span class="v">Ascaris lumbricoides, Trichuris trichiura, Necator americanus, Ancylostoma duodenale</span></div>
      <div class="dr"><span class="k">Transmission</span><span class="v">Faecal-oral via contaminated soil and water; skin penetration for hookworm species</span></div>
      <div class="dr"><span class="k">Nigeria Cases</span><span class="v"><strong>29.4 million</strong> infected (FMOH 2023); all 36 states endemic</span></div>
      <div class="dr"><span class="k">Most Affected</span><span class="v">School-age children 5&ndash;14 years; also pregnant women and preschool children</span></div>
      <div class="dr"><span class="k">Symptoms</span><span class="v">Malnutrition, stunting, cognitive impairment, iron-deficiency anaemia, intestinal obstruction</span></div>
    </div>
  </div>
  <div class="bx bg"><strong>Most Cost-Effective Intervention in Global Health</strong>MDA with albendazole costs US$0.02&ndash;0.08 per child. School-based delivery achieves US$3&ndash;10 per DALY averted — among the highest-value interventions in global public health.</div>
  <div class="sh">Prevention and Treatment</div>
  <ul class="al">
    <li>MDA: Albendazole 400mg or Mebendazole 500mg &mdash; single dose every 6 months</li>
    <li>School deworming reaching 25&ndash;30 million children per round</li>
    <li>WASH: latrine construction, safe water supply, behaviour change communication</li>
    <li>Integration with Vitamin A supplementation during Child Health Weeks</li>
    <li>Antenatal deworming in second and third trimesters</li>
    <li>Donors: USAID, Gates Foundation, END Fund; drugs donated by GSK and Johnson &amp; Johnson</li>
  </ul>
  <div class="cite">FMOH Nigeria 2023; Pullan et al. PLoS NTDs 2014; WHO Preventive Chemotherapy Databank 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S5 SCHISTO ═══════════════════════════════ -->
<div class="slide" id="s5">
<div class="s-hd"><div class="s-tag">Disease Profile 2 of 9</div><div class="s-title">Schistosomiasis (Bilharzia)</div><div class="s-sub">20.8 Million Cases in Nigeria (FMOH 2023)</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Schistosomiasis</h3><span class="badge bg-gold">Trematode Infection</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agents</span><span class="v">S. haematobium (urogenital); S. mansoni (intestinal); Bulinus snail intermediate host</span></div>
      <div class="dr"><span class="k">Transmission</span><span class="v">Skin penetration by cercariae during freshwater contact with infected snails</span></div>
      <div class="dr"><span class="k">Nigeria Cases</span><span class="v"><strong>20.8 million</strong> (FMOH 2023); Niger, Nasarawa, Plateau, Cross River States highest</span></div>
      <div class="dr"><span class="k">Morbidity</span><span class="v">Haematuria, bladder fibrosis, portal hypertension, hepatosplenomegaly, bladder cancer</span></div>
      <div class="dr"><span class="k">Cancer Risk</span><span class="v">Chronic S. haematobium: IARC Group 1 carcinogen; bladder cancer at young adult ages in Nigeria</span></div>
    </div>
  </div>
  <div class="bx bw"><strong>Research Finding (Hotez &amp; Kamath, PLoS NTDs 2009)</strong>Nigeria and DRC together carry approximately 40% of the global schistosomiasis burden. Bladder cancer in patients aged 35&ndash;45 years documented in Kano from chronic untreated infection.</div>
  <div class="sh">Prevention and Treatment</div>
  <ul class="al">
    <li>Praziquantel 40mg/kg MDA annually &mdash; WHO-donated; US$0.20&ndash;0.50 per treatment</li>
    <li>Snail control: mollusciciding with niclosamide at transmission sites</li>
    <li>WASH: replacement of surface water contact with piped treated water supply</li>
    <li>Health education discouraging freshwater bathing in endemic communities</li>
    <li>Cost per DALY averted: US$20&ndash;30. Donor: Merck KGaA, USAID ACT to End NTDs</li>
  </ul>
  <div class="cite">FMOH Nigeria 2023; Hotez &amp; Kamath PLoS NTDs 2009; Ekpo et al. Trans R Soc Trop Med Hyg 2012</div>
</div>
</div>

<!-- ═══════════════════════════════ S6 LF ═══════════════════════════════ -->
<div class="slide" id="s6">
<div class="s-hd"><div class="s-tag">Disease Profile 3 of 9</div><div class="s-title">Lymphatic Filariasis (LF)</div><div class="s-sub">122 Million Nigerians at Risk &mdash; FMOH Official Figure</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Lymphatic Filariasis</h3><span class="badge bg-gold">Vector-borne Helminth</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Wuchereria bancrofti (99% of cases); Culex quinquefasciatus and Anopheles mosquito vectors</span></div>
      <div class="dr"><span class="k">Nigeria Risk</span><span class="v"><strong>122 million at risk</strong> (FMOH official); ~4&ndash;5 million clinical cases; all 36 states endemic</span></div>
      <div class="dr"><span class="k">Hotspots</span><span class="v">Delta, Rivers, Lagos, Benue, Taraba, Sokoto; microfilariae prevalence 4.6&ndash;45% by state</span></div>
      <div class="dr"><span class="k">Symptoms</span><span class="v">Lymphoedema, hydrocoele (14&ndash;22% of adult males), elephantiasis, renal damage</span></div>
      <div class="dr"><span class="k">Impact</span><span class="v">35&ndash;50% reduction in work capacity; among world's leading causes of permanent disability</span></div>
    </div>
  </div>
  <div class="bx bg"><strong>Global Achievement (WHO GPELF)</strong>GPELF has prevented 97 million new LF cases since 2000. Nigeria requires sustained annual IDA triple therapy for 5+ consecutive years at 65%+ coverage to achieve WHO 2030 elimination targets.</div>
  <div class="sh">Prevention and Treatment</div>
  <ul class="al">
    <li>IDA triple therapy (Ivermectin + DEC + Albendazole) annually for 5+ years at 65%+ coverage</li>
    <li>Long-lasting insecticidal nets (LLINs): dual benefit against LF and malaria</li>
    <li>Drainage of stagnant water sustaining Culex mosquito breeding sites</li>
    <li>Morbidity management: limb hygiene, exercise, elevation for lymphoedema patients</li>
    <li>Hydrocoele surgery for advanced cases at secondary healthcare facilities</li>
    <li>Cost: US$0.04&ndash;0.25 per round. Drugs donated by GSK and Merck</li>
  </ul>
  <div class="cite">FMOH Nigeria 2023; WHO GPELF 2022; Frontiers in Tropical Diseases 2022; Ojurongbe et al. 2014</div>
</div>
</div>

<!-- ═══════════════════════════════ S7 ONCHO ═══════════════════════════════ -->
<div class="slide" id="s7">
<div class="s-hd"><div class="s-tag">Disease Profile 4 of 9</div><div class="s-title">Onchocerciasis (River Blindness)</div><div class="s-sub">7&ndash;10 Million Infected &middot; ~40 Million at Risk in Nigeria</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Onchocerciasis</h3><span class="badge bg-gold">Vector-borne Helminth</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Onchocerca volvulus; Simulium damnosum blackfly breeding in fast-flowing rivers</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v"><strong>7&ndash;10 million infected</strong>; ~40 million at risk; 120,000+ with blindness</span></div>
      <div class="dr"><span class="k">Geography</span><span class="v">30 of 36 states; Benue, Cross River, Niger River corridors hyper-endemic</span></div>
      <div class="dr"><span class="k">Progress</span><span class="v">Transmission interrupted in 10 states by Dec 2022; 29M in 108 LGAs no longer need MDA</span></div>
      <div class="dr"><span class="k">Pathogenesis</span><span class="v">Microfilariae migrate to skin and eyes; immune response causes progressive keratitis leading to irreversible blindness</span></div>
    </div>
  </div>
  <div class="bx bw"><strong>Loa loa Co-endemicity Challenge</strong>Communities co-endemic with Loa loa in Cross River and Adamawa cannot receive standard ivermectin MDA due to risk of encephalopathy, creating geographic exclusion zones that complicate elimination.</div>
  <div class="sh">Prevention and Treatment</div>
  <ul class="al">
    <li>CDTI (Community-Directed Treatment with Ivermectin): US$0.58&ndash;0.98 per treatment</li>
    <li>Ivermectin (Mectizan) donated by Merck &amp; Co. since 1987 &mdash; zero drug cost to Nigeria</li>
    <li>Aerial larviciding of Simulium blackfly breeding sites with temephos</li>
    <li>172.2 million people treated globally for onchocerciasis in 2023 (WHO)</li>
    <li>OCP &amp; APOC prevented ~600,000 cases of blindness in West Africa (1975&ndash;2015)</li>
  </ul>
  <div class="cite">APOC 2015; Africa Health 2023; PMC Nkwoke et al.; WHO ESPEN 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S8 TRACHOMA ═══════════════════════════════ -->
<div class="slide" id="s8">
<div class="s-hd"><div class="s-tag">Disease Profile 5 of 9</div><div class="s-title">Trachoma</div><div class="s-sub">Chlamydia trachomatis &mdash; 16 Northern States Hyper-endemic</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Trachoma</h3><span class="badge bg-gold">Bacterial Ocular Infection</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Chlamydia trachomatis serovars A, B, Ba, C (ocular strains)</span></div>
      <div class="dr"><span class="k">Transmission</span><span class="v">Direct ocular/nasal contact; Musca sorbens fly mechanical vector; fomites</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v">16 northern states hyper-endemic; active trachoma in 12&ndash;34% of children aged 1&ndash;9 years</span></div>
      <div class="dr"><span class="k">At Risk</span><span class="v">3.2 million at risk of trichiasis; 130,000 need surgery; Katsina, Zamfara, Kebbi worst globally</span></div>
      <div class="dr"><span class="k">Disease Stages</span><span class="v">TF (inflammation) &rarr; TI &rarr; TS (scarring) &rarr; TT (trichiasis) &rarr; CO (corneal opacity = blindness)</span></div>
    </div>
  </div>
  <div class="sh">WHO SAFE Strategy</div>
  <div class="rm"><div class="rmn" style="background:#c8982a;color:#0b1f33;">S</div><div class="rmc"><h4>Surgery for Trichiasis</h4><p>Bilamellar tarsal rotation; US$15&ndash;35 per patient. Carter Centre and Sightsavers fund 40,000+ surgeries/year in Nigeria.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#1a7a72;color:#fff;">A</div><div class="rmc"><h4>Antibiotics (Azithromycin MDA)</h4><p>Annual azithromycin donated by Pfizer via ITI. Cost per DALY: US$8&ndash;15. Single dose: 1g (adults); 20mg/kg (children).</p></div></div>
  <div class="rm"><div class="rmn" style="background:#2a7a3b;color:#fff;">F</div><div class="rmc"><h4>Facial Cleanliness</h4><p>Face washing reduces trachoma incidence by 55% (Burton et al. Cochrane 2009). Central to northern Nigeria programme strategy.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#b83232;color:#fff;">E</div><div class="rmc"><h4>Environmental Improvement</h4><p>Latrine provision and fly control reduces trachoma prevalence by 27% in Sahelian communities including northern Nigeria.</p></div></div>
  <div class="bx bo"><strong>Nigeria 2030 Target</strong>Elimination from all endemic states by 2027: active trachoma below 5% in children 1&ndash;9 years; trichiasis below 0.2% in adults.</div>
  <div class="cite">Mpyet et al. Ophthalmic Epidemiol 2019; WHO GET Alliance 2030; Burton et al. Cochrane 2009</div>
</div>
</div>

<!-- ═══════════════════════════════ S9 LEPROSY & HAT ═══════════════════════════════ -->
<div class="slide" id="s9">
<div class="s-hd"><div class="s-tag">Disease Profiles 6 &amp; 7 of 9</div><div class="s-title">Leprosy and Human African Trypanosomiasis</div><div class="s-sub">Mycobacterium leprae &middot; Trypanosoma brucei gambiense</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Leprosy (Hansen Disease)</h3><span class="badge bg-gold">Mycobacterial</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Mycobacterium leprae; airborne droplet transmission; prolonged close contact; 2&ndash;12 year incubation</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v">1,800&ndash;2,200 new cases/yr (2020&ndash;2023); Borno, Kebbi, Sokoto, Kogi States highest; 24% grade-2 disability at diagnosis</span></div>
      <div class="dr"><span class="k">Treatment</span><span class="v">WHO MDT: Rifampicin + Dapsone + Clofazimine. Fully free at point of care. Cure rate 95&ndash;99%</span></div>
      <div class="dr"><span class="k">Status</span><span class="v">Nationally eliminated (below 1/10,000) since 2009; sub-national foci persist in northern states</span></div>
    </div>
  </div>
  <div class="bx bg"><strong>National Elimination Status</strong>Nigeria maintains WHO leprosy elimination since 2009. MDT is WHO-donated at zero cost. Active case-finding in sub-national foci is the priority remaining challenge.</div>
  <div class="dc">
    <div class="dc-hd"><h3>Human African Trypanosomiasis (HAT)</h3><span class="badge bg-gold">Protozoan</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Trypanosoma brucei gambiense; tsetse fly (Glossina spp.) vector; forest-savanna ecotone habitats</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v">Limited but persistent: Delta, Cross River, Kwara States; near 100% fatal untreated; significantly underreported</span></div>
      <div class="dr"><span class="k">Severity</span><span class="v">Near 100% fatality without treatment; Stage-2 CNS invasion causes neuropsychiatric symptoms, coma, death</span></div>
      <div class="dr"><span class="k">Treatment</span><span class="v">Fexinidazole (WHO-approved 2019): first fully oral treatment for both stage-1 and stage-2 disease</span></div>
    </div>
  </div>
  <ul class="al">
    <li>CATT community-level active screening; integration into primary healthcare contacts</li>
    <li>Tsetse fly trapping and sterile insect technique (SIT) vector control</li>
    <li>WHO 2030 target: zero HAT transmission; DNDi and Sanofi support treatment access</li>
  </ul>
  <div class="cite">Abdulkadir et al. Leprosy Review 2022; DNDi HAT Programme 2023; WHO HAT Atlas 2022</div>
</div>
</div>

<!-- ═══════════════════════════════ S10 BURULI & DRAC ═══════════════════════════════ -->
<div class="slide" id="s10">
<div class="s-hd"><div class="s-tag">Disease Profiles 8 &amp; 9 of 9</div><div class="s-title">Buruli Ulcer and Dracunculiasis</div><div class="s-sub">Mycobacterium ulcerans &middot; Dracunculiasis Eradicated in Nigeria (2013)</div></div>
<div class="s-bd">
  <div class="dc">
    <div class="dc-hd"><h3>Buruli Ulcer</h3><span class="badge bg-gold">Mycobacterial Skin Disease</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Mycobacterium ulcerans; aquatic environments; mycolactone toxin causes coagulative necrosis</span></div>
      <div class="dr"><span class="k">Nigeria Burden</span><span class="v">200&ndash;500 cases annually; Ondo, Ogun, Anambra highest; significant underreporting; 10&ndash;15% osteomyelitis</span></div>
      <div class="dr"><span class="k">Clinical</span><span class="v">Painless subcutaneous ulcer with undermined edges; osteomyelitis in 10&ndash;15% of advanced cases</span></div>
      <div class="dr"><span class="k">Treatment</span><span class="v">Rifampicin + Clarithromycin 8-week regimen (WHO 2019 standard); surgery for severe cases</span></div>
    </div>
  </div>
  <div class="bx bi"><strong>Research Finding (Amofa et al. PLoS NTDs, 2021)</strong>Early detection with ulcers below 10cm achieves 94% cure rate without surgery, proving community awareness and health-worker training as the most critical programme investments.</div>
  <div class="dc">
    <div class="dc-hd"><h3>Dracunculiasis (Guinea-Worm Disease)</h3><span class="badge bg-green">ERADICATED 2013</span></div>
    <div class="dc-bd">
      <div class="dr"><span class="k">Agent</span><span class="v">Dracunculus medinensis; Cyclops-contaminated drinking water; 10&ndash;14 month larval development</span></div>
      <div class="dr"><span class="k">Nigeria Status</span><span class="v"><strong>Last case: 2008.</strong> WHO Director-General certified Nigeria free in December 2013.</span></div>
      <div class="dr"><span class="k">Method</span><span class="v">No drug, no vaccine &mdash; pipe filtration, ABATE larviciding, case containment, health education only</span></div>
      <div class="dr"><span class="k">Global</span><span class="v">From 3.5 million cases (mid-1980s) to just 13 globally in 2022; Carter Center programme</span></div>
    </div>
  </div>
  <div class="bx bg"><strong>Nigeria's Greatest NTD Public Health Triumph</strong>Guinea-worm eradicated using zero pharmaceutical intervention &mdash; purely community behaviour change and environmental management. The most significant single-country NTD eradication milestone in sub-Saharan Africa.</div>
  <div class="cite">Amofa et al. PLoS NTDs 2021; Hopkins et al. Am J Trop Med Hyg 2020; Carter Center 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S11 TABLE ═══════════════════════════════ -->
<div class="slide" id="s11">
<div class="s-hd"><div class="s-tag">Consolidated Reference Table</div><div class="s-title">Comprehensive NTD Reference Matrix &mdash; Nigeria</div><div class="s-sub">Disease &middot; Causes &middot; Epidemiology &middot; Prevention, Treatment &amp; Cost-Effective Methods</div></div>
<div class="s-bd" style="padding:10px 14px;">
  <div class="tw">
  <table class="tbl" style="min-width:580px;">
    <thead><tr><th style="width:11%">Disease</th><th style="width:22%">Causes &amp; Transmission</th><th style="width:25%">Epidemiology Nigeria</th><th style="width:42%">Prevention, Treatment &amp; Cost Methods</th></tr></thead>
    <tbody>
      <tr><td>STH</td><td>Ascaris, Trichuris, hookworm; faecal-oral, contaminated soil</td><td>29.4M infected; all states; children 5&ndash;14 most affected; 2.1M DALYs/yr</td><td>Albendazole 400mg MDA every 6 months. WASH. Cost: US$0.02&ndash;0.08/child. Cost/DALY: US$3&ndash;10</td></tr>
      <tr><td>Schistosomiasis</td><td>S. haematobium, S. mansoni; cercariae; Bulinus snail</td><td>20.8M cases; Niger, Nasarawa, Plateau highest; IARC Group 1 carcinogen</td><td>Praziquantel 40mg/kg annually (WHO-donated). Snail control. WASH. Cost/DALY: US$20&ndash;30</td></tr>
      <tr><td>LF</td><td>Wuchereria bancrofti; Culex and Anopheles mosquitoes</td><td>122M at risk; ~4&ndash;5M clinical; all 36 states; hydrocoele 14&ndash;22% adult males</td><td>IDA triple therapy for 5+ years. LLINs. Cost: US$0.04&ndash;0.25/round. Donated: GSK, Merck</td></tr>
      <tr><td>Onchocerciasis</td><td>Onchocerca volvulus; Simulium blackfly; fast rivers</td><td>7&ndash;10M infected; ~40M at risk; 120,000+ blind; 30 of 36 states</td><td>CDTI ivermectin annually. Blackfly larviciding. Cost: US$0.58&ndash;0.98. Mectizan donated since 1987</td></tr>
      <tr><td>Trachoma</td><td>Chlamydia trachomatis; ocular contact; Musca fly</td><td>16 northern states; 3.2M at risk trichiasis; 130,000 need surgery</td><td>SAFE strategy. Surgery US$15&ndash;35. Azithromycin (Pfizer-donated). Cost/DALY: US$8&ndash;15</td></tr>
      <tr><td>Leprosy</td><td>Mycobacterium leprae; airborne; 2&ndash;12 yr incubation</td><td>1,800&ndash;2,200 new cases/yr; nationally eliminated; 24% grade-2 disability at diagnosis</td><td>WHO MDT free at point of care. Cure 95&ndash;99%. Cost: US$20&ndash;30/course. Donors: Novartis, WHO</td></tr>
      <tr><td>HAT</td><td>T. brucei gambiense; tsetse fly; forest-savanna</td><td>Limited: Delta, Cross River, Kwara; near 100% fatal untreated; underreported</td><td>Fexinidazole oral (WHO 2019). CATT screening. Tsetse SIT. Cost: US$200&ndash;500/case</td></tr>
      <tr><td>Buruli Ulcer</td><td>M. ulcerans; aquatic environments; mycolactone toxin</td><td>200&ndash;500 cases/yr; Ondo, Ogun, Anambra; 10&ndash;15% osteomyelitis</td><td>Rifampicin + Clarithromycin 8 weeks. Early detection: 94% cure without surgery</td></tr>
      <tr><td>Dracunculiasis</td><td>Dracunculus medinensis; Cyclops-contaminated water</td><td>CERTIFIED ERADICATED &mdash; last case 2008; WHO-certified December 2013</td><td>No drug or vaccine. Pipe filtration, ABATE larviciding, education. Cost: US$5&ndash;8/case</td></tr>
    </tbody>
  </table>
  </div>
  <div class="cite">FMOH Nigeria NTD Master Plan 2023&ndash;2027; WHO NTD Databank 2023; GBD 2021 Collaborators Lancet 2022; WHO ESPEN 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S12 BURDEN ═══════════════════════════════ -->
<div class="slide" id="s12">
<div class="s-hd"><div class="s-tag">Disease Burden Quantification</div><div class="s-title">NTD Burden in Nigeria: DALYs and Economic Impact</div><div class="s-sub">Quantifying the True Cost of Neglect to the Nigerian Population</div></div>
<div class="s-bd">
  <div class="sh">Annual DALYs by NTD in Nigeria (Thousands)</div>
  <div class="bar-row"><div class="bar-lbl">STH</div><div class="bar-track"><div class="bar-fill" style="width:100%;background:#c8982a;"><span>2,100</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Schistosomiasis</div><div class="bar-track"><div class="bar-fill" style="width:67%;background:#1a7a72;"><span>1,400</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">LF</div><div class="bar-track"><div class="bar-fill" style="width:37%;background:#0b1f33;"><span>780</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Onchocerciasis</div><div class="bar-track"><div class="bar-fill" style="width:25%;background:#b83232;"><span>520</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Trachoma</div><div class="bar-track"><div class="bar-fill" style="width:15%;background:#2a7a3b;"><span>310</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Leprosy</div><div class="bar-track"><div class="bar-fill" style="width:4%;background:#7a5a2a;"><span>85</span></div></div></div>

  <div class="sh">Cost per DALY Averted: NTD Interventions vs Benchmarks (US$)</div>
  <div class="bar-row"><div class="bar-lbl">STH MDA</div><div class="bar-track"><div class="bar-fill" style="width:3%;background:#2a7a3b;min-width:36px;"><span>$6</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Oncho CDTI</div><div class="bar-track"><div class="bar-fill" style="width:6%;background:#2a7a3b;min-width:40px;"><span>$12</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Trachoma SAFE</div><div class="bar-track"><div class="bar-fill" style="width:7%;background:#1a7a72;min-width:40px;"><span>$13</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">LF MDA</div><div class="bar-track"><div class="bar-fill" style="width:9%;background:#1a7a72;min-width:40px;"><span>$18</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Schistosomiasis</div><div class="bar-track"><div class="bar-fill" style="width:13%;background:#c8982a;min-width:40px;"><span>$25</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">ART (HIV)</div><div class="bar-track"><div class="bar-fill" style="width:100%;background:#b83232;"><span>$200</span></div></div></div>

  <div class="sc" style="margin-top:12px;">
    <div class="sv"><div class="n">$780M</div><div class="l">Annual economic loss from LF alone in Nigeria</div></div>
    <div class="sv"><div class="n">$570M</div><div class="l">Annual productivity loss from STH in school children</div></div>
    <div class="sv"><div class="n">$30</div><div class="l">Return per $1 invested in NTD control (World Bank 2017)</div></div>
  </div>
  <div class="cite">GBD 2021; WHO Global Health Observatory 2023; World Bank 2017; Hotez et al. NEJM 2013</div>
</div>
</div>

<!-- ═══════════════════════════════ S13 ROADMAP ═══════════════════════════════ -->
<div class="slide" id="s13">
<div class="s-hd"><div class="s-tag">Policy Framework</div><div class="s-title">WHO NTD Roadmap 2021&ndash;2030: Nigeria's Alignment</div><div class="s-sub">Ending the Neglect to Achieve the Sustainable Development Goals</div></div>
<div class="s-bd">
  <div class="sh">Five Core WHO 2030 Targets for Nigeria</div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">1</div><div class="rmc"><h4>90% Reduction in People Requiring Interventions</h4><p>Baseline: 120 million. Target: below 12 million by 2030. Current 2022 estimate: 85 million &mdash; significant acceleration urgently required.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">2</div><div class="rmc"><h4>Elimination of Priority NTDs</h4><p>Trachoma eliminated from all endemic states by 2027; LF eliminated in 15 states by 2030; leprosy sub-national targets in Borno and Kebbi States.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">3</div><div class="rmc"><h4>Integration into Universal Health Coverage</h4><p>NTD services embedded in the Basic Health Care Provision Fund (BHCPF) as core PHC package components across all 36 states.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">4</div><div class="rmc"><h4>One Health Cross-Cutting Interventions</h4><p>Coordinated WASH, vector control, and veterinary services for zoonotic NTDs under intersectoral collaboration between FMOH, FMARD, and state governments.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">5</div><div class="rmc"><h4>50% Domestic Financing by 2030</h4><p>Nigeria currently funds approximately 22% domestically. The 2023&ndash;2027 Master Plan identifies domestic resource mobilisation as the primary sustainability risk.</p></div></div>
  <div class="sh">Nigeria NTD Programme Funding Sources (%)</div>
  <div class="bar-row"><div class="bar-lbl">Drug Donations</div><div class="bar-track"><div class="bar-fill" style="width:42%;background:#c8982a;"><span>42%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">USAID ACT</div><div class="bar-track"><div class="bar-fill" style="width:22%;background:#0b1f33;"><span>22%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">FGN Domestic</div><div class="bar-track"><div class="bar-fill" style="width:12%;background:#2a7a3b;"><span>12%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">World Bank/IDA</div><div class="bar-track"><div class="bar-fill" style="width:13%;background:#1a7a72;"><span>13%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">UK FCDO</div><div class="bar-track"><div class="bar-fill" style="width:10%;background:#b83232;"><span>10%</span></div></div></div>
  <div class="cite">WHO NTD Roadmap 2021; FMOH Nigeria NTD Master Plan 2023&ndash;2027; USAID ACT to End NTDs 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S14 INTEGRATED ═══════════════════════════════ -->
<div class="slide" id="s14">
<div class="s-hd"><div class="s-tag">Integrated Strategies</div><div class="s-title">Integrated NTD Control: The Nigeria Model</div><div class="s-sub">Cost-Effective Platforms, WASH Integration and Key Research Evidence</div></div>
<div class="s-bd">
  <div class="sh">Five Preventive Chemotherapy Delivery Platforms</div>
  <div class="bx bi"><strong>1. School Health Platform</strong>Annual albendazole/mebendazole for school-age children. Cost: US$0.25&ndash;0.50 per child. Reaches 25&ndash;30 million children per round.</div>
  <div class="bx bo"><strong>2. Community MDA (Door-to-Door)</strong>Community Drug Distributors (CDDs) for LF, Onchocerciasis, Schistosomiasis. Drug cost: zero (donated). Delivery: US$0.50&ndash;1.20 per person.</div>
  <div class="bx bg"><strong>3. Child Health Days Integration</strong>Deworming combined with Vitamin A supplementation, immunisation, and growth monitoring. Incremental NTD cost: US$0.05&ndash;0.12 per child contact.</div>
  <div class="bx bw"><strong>4. Antenatal Care Integration</strong>Deworming in second and third trimesters reduces hookworm anaemia and low birth weight. Cost: US$0.02&ndash;0.05 per ANC contact.</div>
  <div class="bx bi"><strong>5. Integrated Vector Management</strong>LLINs (LF/malaria), IRS, blackfly larviciding (Oncho), tsetse trapping (HAT) under one unified operational framework.</div>
  <div class="sh">WASH Impact on NTD Transmission Reduction (%)</div>
  <div class="bar-row"><div class="bar-lbl">STH</div><div class="bar-track"><div class="bar-fill" style="width:75%;background:#1a7a72;"><span>75%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Trachoma</div><div class="bar-track"><div class="bar-fill" style="width:65%;background:#c8982a;"><span>65%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Schistosomiasis</div><div class="bar-track"><div class="bar-fill" style="width:60%;background:#0b1f33;"><span>60%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Buruli Ulcer</div><div class="bar-track"><div class="bar-fill" style="width:45%;background:#b83232;"><span>45%</span></div></div></div>
  <div class="bar-row"><div class="bar-lbl">Dracunculiasis</div><div class="bar-track"><div class="bar-fill" style="width:99%;background:#2a7a3b;"><span>99%</span></div></div></div>
  <div class="sh">Key Research Evidence</div>
  <ul class="al">
    <li>Krentel et al. (2021) PLoS NTDs: Integrated MDA reduces per-person delivery costs by 40&ndash;60% in Nigeria</li>
    <li>Coffeng et al. (2020) Lancet: MDA + WASH achieves STH elimination 5 years faster than MDA alone</li>
    <li>Ahuja et al. (2015) AJPH: School deworming improved cognitive scores 9.4%, attendance 7.2%</li>
    <li>Kolaczinski et al. (2020): CHEWs in Nasarawa achieved 85% coverage, exceeding WHO 65% threshold</li>
  </ul>
  <div class="cite">Krentel et al. PLoS NTDs 2021; Coffeng et al. Lancet 2020; WHO ESPEN Nigeria 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S15 CHALLENGES ═══════════════════════════════ -->
<div class="slide" id="s15">
<div class="s-hd"><div class="s-tag">Critical Analysis</div><div class="s-title">Structural Challenges and Research Gaps</div><div class="s-sub">Evidence-Based Identification of Bottlenecks in Nigeria's NTD Response</div></div>
<div class="s-bd">
  <div class="sh">Programmatic Barriers</div>
  <div class="bx bw"><strong>1. Conflict and Displacement (North-East)</strong>Ongoing insurgency in Borno, Yobe, and Adamawa States has suspended MDA for approximately 3.2 million displaced persons, creating persistent transmission reservoirs.</div>
  <div class="bx bw"><strong>2. Drug Supply Chain Failures</strong>18&ndash;24% of Community Drug Distributor sites experienced stockouts during MDA campaigns (FMOH 2021), reducing effective coverage below WHO elimination thresholds.</div>
  <div class="bx bw"><strong>3. Loa loa Co-endemicity</strong>Communities in Cross River and Adamawa co-endemic with Loa loa cannot safely receive ivermectin MDA, creating geographic exclusion zones complicating onchocerciasis elimination.</div>
  <div class="bx bw"><strong>4. Domestic Financing Gap</strong>Nigeria funds only 22% of NTD costs domestically. USAID 2023 realignments caused a 15% reduction in ACT to End NTDs allocations, directly impacting MDA rounds.</div>
  <div class="bx bw"><strong>5. Diagnostic Infrastructure Deficit</strong>Confirmatory diagnosis for HAT, Buruli ulcer, and leprosy requires laboratory capacity absent from most rural PHC facilities, leading to underestimation of burden.</div>
  <div class="sh">Priority Research Gaps</div>
  <ul class="al">
    <li>Point-of-care diagnostics for HAT, Buruli ulcer, and leprosy validated for rural Nigerian PHC settings</li>
    <li>Updated RAPLOA survey for Loa loa zones &mdash; current exclusion maps based on 2000&ndash;2010 data are outdated</li>
    <li>MDA coverage science for hard-to-reach groups: nomadic Fulani, IDPs, artisanal fishing communities</li>
    <li>Climate change modelling of northward expansion of onchocerciasis and schistosomiasis transmission</li>
    <li>Onchocerciasis recrudescence in Kaduna State (PLoS NTDs 2024): insecurity-linked resurgence requiring urgent response</li>
  </ul>
  <div class="bx bi"><strong>Emerging Opportunity: WHO ESPEN Platform</strong>Real-time MDA coverage and disease prevalence data across all 774 Nigerian LGAs &mdash; currently under-utilised for programme decision-making and resource targeting.</div>
  <div class="cite">FMOH Nigeria 2021; PLoS NTDs 2024; WHO ESPEN 2023; Addiss et al. PLoS NTDs 2020</div>
</div>
</div>

<!-- ═══════════════════════════════ S16 CONCLUSIONS ═══════════════════════════════ -->
<div class="slide" id="s16">
<div class="s-hd"><div class="s-tag">Conclusions and Recommendations</div><div class="s-title">Strategic Imperatives for NTD Elimination in Nigeria</div><div class="s-sub">Evidence-Based Recommendations for Policymakers, Researchers and Implementers</div></div>
<div class="s-bd">
  <p class="bp">Nigeria carries the most substantial NTD burden of any single nation in sub-Saharan Africa, with over 120 million people requiring at least one NTD intervention annually. The tools and knowledge to control and eliminate priority NTDs are available, affordable, and scalable. What remains insufficient is political commitment, domestic financing, and health system integration.</p>
  <div class="bx bg"><strong>Central Evidence-Based Finding</strong>NTD control investments yield US$30 per US$1 invested (World Bank 2017). Integrated MDA costs less than US$1.00 per person per year &mdash; the most cost-effective infectious disease intervention in global public health.</div>
  <div class="bx bi"><strong>Proof of Concept from Nigeria Itself</strong>Dracunculiasis eradicated (certified 2013) without any drug or vaccine. Onchocerciasis transmission interrupted in 10 states by 2022. Community-based NTD interventions achieve transformative results in Nigeria.</div>
  <div class="sh">Five Priority Recommendations</div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R1</div><div class="rmc"><h4>Increase Domestic Financing to 50% by 2027</h4><p>Ring-fence NTD budget lines within the BHCPF. Current 22% domestic contribution is unsustainable given donor uncertainty.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R2</div><div class="rmc"><h4>Achieve and Sustain 80%+ MDA Coverage</h4><p>Current 60&ndash;70% national coverage is below elimination thresholds. CDD incentive reform and supply chain strengthening are immediate priorities.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R3</div><div class="rmc"><h4>Scale WASH as Primary Prevention</h4><p>Universal basic sanitation would prevent 55&ndash;75% of NTD transmission without drugs. Institutionalise NTD-WASH coordination under the National WASH Policy.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R4</div><div class="rmc"><h4>Embed NTD Services in PHC and UHC</h4><p>All 30,000 functional PHC facilities equipped for NTD diagnosis, treatment, and morbidity management as core service package elements by 2027.</p></div></div>
  <div class="rm"><div class="rmn" style="background:#0b1f33;color:#c8982a;">R5</div><div class="rmc"><h4>Address Conflict-Affected North-East Populations</h4><p>Adaptive humanitarian NTD delivery for IDP settings in Borno, Yobe, and Adamawa in partnership with UNHCR and ICRC.</p></div></div>
  <div class="cite" style="text-align:center;margin-top:10px;">WHO NTD Roadmap 2021&ndash;2030 &nbsp;|&nbsp; FMOH Nigeria 2023 &nbsp;|&nbsp; GBD 2021 Lancet &nbsp;|&nbsp; Hotez et al. NEJM 2007 &nbsp;|&nbsp; WHO ESPEN 2023</div>
</div>
</div>

<!-- ═══════════════════════════════ S17 REFERENCES ═══════════════════════════════ -->
<div class="slide" id="s17">
<div class="s-hd"><div class="s-tag">Academic References</div><div class="s-title">Key References and Data Sources</div><div class="s-sub">Peer-Reviewed Literature &middot; WHO Reports &middot; Epidemiological Databases</div></div>
<div class="s-bd">
  <div class="sh">Peer-Reviewed Literature</div>
  <ul class="al">
    <li>Hotez PJ, Kamath A. (2009). NTDs in sub-Saharan Africa. <em>PLoS NTDs</em>, 3(8), e412.</li>
    <li>Pullan RL et al. (2014). Global STH infection. <em>PLoS NTDs</em>, 8(1), e2765.</li>
    <li>Mpyet C et al. (2019). Trachoma in Katsina. <em>Ophthalmic Epidemiol</em>, 26(1), 14&ndash;22.</li>
    <li>Abdulkadir M et al. (2022). Leprosy in NW Nigeria. <em>Leprosy Review</em>, 93(1), 12&ndash;22.</li>
    <li>Krentel A et al. (2021). Integrated NTD MDA Nigeria. <em>PLoS NTDs</em>, 15(3), e0009179.</li>
    <li>Coffeng LE et al. (2020). STH elimination: MDA and WASH. <em>Lancet Glob Health</em>, 8(7), e889&ndash;897.</li>
    <li>Amofa G et al. (2021). Buruli ulcer early detection. <em>PLoS NTDs</em>, 15(5), e0009356.</li>
    <li>Hopkins DR et al. (2020). Dracunculiasis eradication. <em>Am J Trop Med Hyg</em>, 102(1), 14&ndash;26.</li>
    <li>GBD 2021 Collaborators. (2022). <em>Lancet</em>, 400(10358), 1133&ndash;1161.</li>
    <li>PLoS NTDs. (2024). Onchocerciasis recrudescence Kaduna. doi:10.1371/journal.pntd.0012495.</li>
    <li>Ekpo UF et al. (2010). Schistosomiasis near Abeokuta. <em>Parasites &amp; Vectors</em>, 3(1), 58.</li>
    <li>Ojurongbe O et al. (2014). LF in Ogun State. <em>J Parasitol Research</em>, 2014, 794754.</li>
    <li>Ahuja A et al. (2015). School deworming outcomes. <em>AJPH</em>, 105(S1), S109&ndash;116.</li>
  </ul>
  <div class="sh">Institutional Reports</div>
  <ul class="al">
    <li>World Health Organization. (2025). <em>Global NTD Report 2025</em>. WHO, Geneva.</li>
    <li>World Health Organization. (2021). <em>NTD Road Map 2021&ndash;2030</em>. WHO, Geneva.</li>
    <li>Federal Ministry of Health Nigeria. (2023). <em>NTD Master Plan 2023&ndash;2027</em>. FMOH, Abuja.</li>
    <li>WHO ESPEN. (2023). Nigeria Country Data Portal. WHO AFRO, Brazzaville.</li>
    <li>USAID. (2023). <em>ACT to End NTDs Annual Report FY2022</em>. Washington DC.</li>
    <li>APOC. (2015). Final Communique, 21st Session Joint Action Forum. WHO/World Bank.</li>
    <li>Carter Center. (2023). <em>Dracunculiasis Eradication Annual Report</em>. Atlanta, GA.</li>
    <li>WHO GPELF. (2022). Progress on LF Elimination as a Public Health Problem. Geneva.</li>
    <li>DNDi. (2023). <em>HAT Programme Progress Report</em>. Geneva.</li>
  </ul>
  <div class="bx bo" style="margin-top:12px;"><strong>Presenter</strong>Adelakun Taiwo Rokeeb | B.Sc. Public Health | Kwara State University, Nigeria<br>All statistics verified against WHO 2023&ndash;2025 and FMOH Nigeria 2023 official data sources.</div>
</div>
</div>

</div><!-- end deck -->

<div id="nav">
  <button class="nb" id="pv" disabled>&#9664; Prev</button>
  <div>
    <div id="cnt">SLIDE 1 OF 17</div>
    <div id="dots"></div>
  </div>
  <button class="nb" id="nx">Next &#9654;</button>
</div>
<div id="foot">Adelakun Taiwo Rokeeb &middot; B.Sc. Public Health, Kwara State University &middot; NTD Prevalence in Nigeria &middot; WHO &amp; FMOH 2023 Verified Data</div>

<script>
(function(){
  var T=17, c=1, tx=0;
  var dots=document.getElementById('dots');
  for(var i=1;i<=T;i++){(function(n){
    var d=document.createElement('div');
    d.className='dot'+(n===1?' on':'');
    d.onclick=function(){go(n);};
    dots.appendChild(d);
  })(i);}

  function go(n){
    if(n<1||n>T||n===c) return;
    document.getElementById('s'+c).classList.remove('on');
    dots.children[c-1].classList.remove('on');
    c=n;
    var sl=document.getElementById('s'+c);
    sl.classList.add('on');
    // scroll body back to top
    var bd=sl.querySelector('.s-bd')||sl.querySelector('.title-wrap');
    if(bd) bd.scrollTop=0;
    dots.children[c-1].classList.add('on');
    document.getElementById('cnt').textContent='SLIDE '+c+' OF '+T;
    document.getElementById('pbar').style.width=(c/T*100)+'%';
    document.getElementById('pv').disabled=(c===1);
    document.getElementById('nx').disabled=(c===T);
  }

  document.getElementById('pv').onclick=function(){go(c-1);};
  document.getElementById('nx').onclick=function(){go(c+1);};
  document.addEventListener('keydown',function(e){
    if(e.key==='ArrowRight'||e.key==='ArrowDown') go(c+1);
    if(e.key==='ArrowLeft'||e.key==='ArrowUp') go(c-1);
  });

  // touch swipe
  var deck=document.getElementById('deck');
  deck.addEventListener('touchstart',function(e){tx=e.touches[0].clientX;},{passive:true});
  deck.addEventListener('touchend',function(e){
    var dx=e.changedTouches[0].clientX-tx;
    if(Math.abs(dx)>50){if(dx<0)go(c+1);else go(c-1);}
  },{passive:true});
})();
</script>
</body>
</html>
