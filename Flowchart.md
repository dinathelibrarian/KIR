\### Kollaboration, Affiliation

\`\`\`mermaid

flowchart TD

classDef Werk fill:#A9F5F2;

classDef Person_w fill:#87CEFA;

classDef Ort fill:#A9A9F5;

classDef Sammlung fill:#F781D8;

classDef Person_m fill:#CECEF6;

classDef Institution fill:#FE9A2E;

a*de-blin[Allende de Blin<br>\*1928]:::Person*m;

g*steinke[Günter Steinke<br>\*1956]:::Person*m;

th*neuhaus[Thomas Neuhaus<br>\*1961]:::Person*m;

g*zacher[Gerd Zacher<br>1929-2014]:::Person*m;

k*haussmann[Karin Haußmann<br>\*1962]:::Person*w;

na*huber[Nicolaus A. Huber<br>\*1939]:::Person*m;

Folkwang{Folkwang <br>Universität der<br> Künste}:::Institution

UDE((Universität<br>Duisburg Essen)):::Institution

a*de-blin <-.->|Kollaborierte mit| g*zacher

g_steinke -.->|Lehrt an| Folkwang

g_zacher -.->|Lehrte an| Folkwang

k_haussmann -.->|Lehrt an<br>Studierte an| Folkwang

k_haussmann -.->|Lehrte an| UDE

k*haussmann -.->|Schülerin von| na*huber

na_huber -.->|Lehrte an| Folkwang

th_neuhaus -.->|Lehrt an| Folkwang

\`\`\`

\### Schaffen

\`\`\`mermaid

flowchart

classDef Werk fill:#A9F5F2;

classDef Person_w fill:#87CEFA;

classDef Ort fill:#A9A9F5;

classDef Besetzung fill:#F781D8;

classDef Person_m fill:#CECEF6;

classDef Institution fill:#FE9A2E;

a*de-blin[Allende de Blin<br>\*1928]:::Person*m;

g*steinke[Günter Steinke<br>\*1956]:::Person*m;

th*neuhaus[Thomas Neuhaus<br>\*1961]:::Person*m;

g*zacher[Gerd Zacher<br>1929-2014]:::Person*m;

k*haussmann[Karin Haußmann<br>\*1962]:::Person*w;

na*huber[Nicolaus A. Huber<br>\*1939]:::Person*m;

deblin*2012*memoire(gnd:1028672322<br>Werk der Musik<br>Mémoire de l'oubli<br>2012):::Werk -.->|In memoriam| g_zacher

neuhaus*1989*kunststoff(gnd:1258315785<br>Werk der Musik<br>Kunst-Stoff Drumprojekt<br>1986):::Werk

haussmann*2016*kriegslied(gnd:1231718862<br>Werk der Musik<br>Kriegslied<br>2016):::Werk

steinke*1986*rho(gnd:1069142069<br>Werk der Musik<br>Rho<br>1986):::Werk

zacher*1961*diferencias(gnd:1072015951<br>Werk der Musik<br>Diferencias<br>1961):::Werk

huber*1965*choerecelan(gnd:<br>Werk der Musik<br>Zwei Chöre nach Paul Celan):::Werk

Besetzung_Chor((Chor)):::Besetzung

Besetzung_Orchester((Orchester)):::Besetzung

Besetzung_Kontrafagott((Kontrafagott)):::Besetzung

Besetzung_Orgel((Orgel)):::Besetzung

Besetzung_Schlagzeug((Schlagzeug)):::Besetzung

Besetzung_Tonband((Tonband)):::Besetzung

Besetzung_Computer((Computer)):::Besetzung

a*de-blin -->deblin*2012*memoire --> Besetzung*Orgel

g*steinke --> steinke*1986*rho --> Besetzung*Kontrafagott

g*zacher --> zacher*1961*diferencias --> Besetzung*Orgel

th*neuhaus -->neuhaus*1989_kunststoff

	neuhaus*1989*kunststoff -->|4| Besetzung_Schlagzeug((Schlagzeug)):::Besetzung

	neuhaus*1989*kunststoff --> Besetzung_Computer((Computer)):::Besetzung

	neuhaus*1989*kunststoff -->|Interaktiv| Besetzung_Tonband((Tonband)):::Besetzung

k*haussmann --> haussmann*2016_kriegslied

	haussmann*2016*kriegslied -->|SSATB| Besetzung_Chor

	haussmann*2016*kriegslied --> Besetzung_Orchester 

na*huber --> huber*1965*choerecelan --> Besetzung*Chor

\`\`\`