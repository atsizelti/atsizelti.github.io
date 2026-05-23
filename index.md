<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Şükrü Atsızelti | Ph.D. Candidate in Sociology</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400&display=swap" rel="stylesheet">
    <style>
        *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

        :root {
            --slate-900: #0f172a;
            --slate-800: #1e293b;
            --slate-700: #334155;
            --slate-600: #475569;
            --slate-400: #94a3b8;
            --slate-300: #cbd5e1;
            --slate-200: #e2e8f0;
            --slate-100: #f1f5f9;
            --slate-50:  #f8fafc;
            --teal-700:  #0f766e;
            --teal-600:  #0d9488;
            --teal-500:  #14b8a6;
            --teal-200:  #99f6e4;
            --teal-100:  #ccfbf1;
        }

        html { scroll-behavior: smooth; }

        body {
            font-family: 'Inter', system-ui, sans-serif;
            background: var(--slate-100);
            color: var(--slate-700);
            line-height: 1.6;
        }

        /* ── Layout ─────────────────────────────────────── */
        .layout {
            display: flex;
            min-height: 100vh;
            max-width: 1080px;
            margin: 0 auto;
            box-shadow: 0 4px 60px rgba(0,0,0,.15);
        }

        /* ── Sidebar ─────────────────────────────────────── */
        .sidebar {
            width: 270px;
            flex-shrink: 0;
            background: var(--slate-800);
            color: #fff;
            padding: 44px 28px 40px;
            display: flex;
            flex-direction: column;
            gap: 28px;
            position: sticky;
            top: 0;
            height: 100vh;
            overflow-y: auto;
        }

        .sidebar::-webkit-scrollbar { width: 4px; }
        .sidebar::-webkit-scrollbar-thumb { background: var(--slate-700); border-radius: 2px; }

        .sb-photo {
            width: 96px; height: 96px;
            border-radius: 50%;
            border: 3px solid var(--teal-500);
            overflow: hidden;
            margin: 0 auto;
            background: var(--slate-700);
            display: flex; align-items: center; justify-content: center;
            flex-shrink: 0;
        }
        .sb-photo img { width: 100%; height: 100%; object-fit: cover; }
        .sb-photo-initials {
            font-size: 26px; font-weight: 700;
            color: var(--teal-500); letter-spacing: -1px;
            display: none;
        }

        .sb-identity { text-align: center; }
        .sb-name { font-size: 17px; font-weight: 700; line-height: 1.3; color: #fff; }
        .sb-role {
            font-size: 11px; font-weight: 500; letter-spacing: .07em;
            text-transform: uppercase; color: var(--teal-500); margin-top: 4px;
        }

        .sb-divider { height: 1px; background: var(--slate-700); }

        .sb-label {
            font-size: 10px; font-weight: 700; letter-spacing: .12em;
            text-transform: uppercase; color: var(--teal-500); margin-bottom: 10px;
        }

        .sb-contact-item {
            display: flex; align-items: flex-start; gap: 8px;
            font-size: 12.5px; color: var(--slate-400); margin-bottom: 8px;
        }
        .sb-contact-item a { color: var(--slate-400); text-decoration: none; word-break: break-all; }
        .sb-contact-item a:hover { color: var(--teal-500); }
        .sb-icon { flex-shrink: 0; margin-top: 1px; }

        .sb-tags { display: flex; flex-wrap: wrap; gap: 5px; }
        .sb-tag {
            background: var(--slate-700); color: var(--slate-300);
            font-size: 11px; font-weight: 500; padding: 3px 8px; border-radius: 4px;
        }

        /* ── Main ─────────────────────────────────────────── */
        .main { flex: 1; background: #fff; overflow: hidden; min-width: 0; }

        .main-hero {
            background: var(--slate-900);
            padding: 44px 52px 36px;
            border-bottom: 3px solid var(--teal-600);
        }
        .hero-name {
            font-size: 34px; font-weight: 700; letter-spacing: -.02em;
            color: #fff; line-height: 1.2; margin-bottom: 6px;
        }
        .hero-sub { font-size: 14.5px; color: var(--teal-500); font-weight: 400; }

        .main-body { padding: 44px 52px; }

        /* ── Section ─────────────────────────────────────── */
        .section { margin-bottom: 48px; }

        .section-head {
            display: flex; align-items: center; gap: 14px;
            margin-bottom: 24px;
        }
        .section-title {
            font-size: 11px; font-weight: 700; letter-spacing: .12em;
            text-transform: uppercase; color: var(--slate-600); white-space: nowrap;
        }
        .section-rule { flex: 1; height: 1px; background: var(--slate-200); }

        /* ── Timeline entry ──────────────────────────────── */
        .entry {
            display: grid;
            grid-template-columns: 88px 1fr;
            gap: 0 20px;
            margin-bottom: 22px;
            padding-bottom: 22px;
            border-bottom: 1px solid var(--slate-100);
        }
        .entry:last-child { border-bottom: none; margin-bottom: 0; padding-bottom: 0; }

        .entry-date {
            font-size: 11.5px; font-weight: 600; color: var(--teal-600);
            text-align: right; padding-top: 3px; line-height: 1.5;
        }

        .entry-title { font-size: 14.5px; font-weight: 600; color: var(--slate-800); margin-bottom: 2px; }
        .entry-org   { font-size: 13px; font-weight: 500; color: var(--teal-700); margin-bottom: 5px; }
        .entry-desc  { font-size: 13px; color: var(--slate-600); line-height: 1.65; }
        .entry-desc a { color: var(--teal-600); text-decoration: none; }
        .entry-desc a:hover { text-decoration: underline; }

        /* ── Publication entry ───────────────────────────── */
        .pub {
            font-size: 13.5px; color: var(--slate-700); line-height: 1.75;
            margin-bottom: 18px; padding-bottom: 18px;
            border-bottom: 1px solid var(--slate-100);
            padding-left: 14px;
            border-left: 3px solid var(--teal-200);
        }
        .pub:last-child { border-bottom: none; margin-bottom: 0; }
        .pub-year {
            font-size: 10.5px; font-weight: 700; letter-spacing: .06em;
            color: var(--teal-600); text-transform: uppercase; margin-bottom: 3px;
        }
        .pub a { color: var(--teal-600); text-decoration: none; }
        .pub a:hover { text-decoration: underline; }
        .pub em { font-style: italic; }

        .badge {
            display: inline-block; font-size: 9.5px; font-weight: 700;
            padding: 2px 6px; border-radius: 3px; text-transform: uppercase;
            letter-spacing: .05em; margin-left: 5px; vertical-align: middle;
        }
        .badge-review   { background: var(--teal-100); color: var(--teal-700); }
        .badge-revision { background: #fef9c3; color: #854d0e; }

        /* ── Presentation list ───────────────────────────── */
        .pres-list { list-style: none; }
        .pres-item {
            display: grid; grid-template-columns: 36px 1fr;
            gap: 0 12px; margin-bottom: 10px;
            font-size: 13px; color: var(--slate-700); line-height: 1.65;
        }
        .pres-year { font-size: 11.5px; font-weight: 600; color: var(--teal-600); padding-top: 2px; }

        /* ── Responsive ──────────────────────────────────── */
        @media (max-width: 780px) {
            .layout { flex-direction: column; }
            .sidebar { width: 100%; height: auto; position: static; }
            .main-hero { padding: 32px 28px 24px; }
            .main-body { padding: 32px 28px; }
            .entry { grid-template-columns: 1fr; }
            .entry-date { text-align: left; margin-bottom: 4px; }
        }
    </style>
</head>
<body>
<div class="layout">

    <!-- ════════════════ SIDEBAR ════════════════ -->
    <aside class="sidebar">

        <div class="sb-photo">
            <img src="assets/images/profile.jpg" alt="Şükrü Atsızelti"
                 onerror="this.style.display='none';this.nextElementSibling.style.display='flex';">
            <span class="sb-photo-initials">ŞA</span>
        </div>

        <div class="sb-identity">
            <div class="sb-name">Şükrü Atsızelti</div>
            <div class="sb-role">Ph.D. Candidate · Sociology</div>
        </div>

        <div class="sb-divider"></div>

        <div>
            <div class="sb-label">Contact</div>
            <div class="sb-contact-item">
                <span class="sb-icon">✉</span>
                <a href="mailto:satsizelti22@ku.edu.tr">satsizelti22@ku.edu.tr</a>
            </div>
            <div class="sb-contact-item">
                <span class="sb-icon">🏛</span>
                <span>Koç University, Istanbul, Turkey</span>
            </div>
        </div>

        <div class="sb-divider"></div>

        <div>
            <div class="sb-label">Research</div>
            <div class="sb-tags">
                <span class="sb-tag">Computational Social Science</span>
                <span class="sb-tag">LLMs &amp; Surveys</span>
                <span class="sb-tag">Public Opinion</span>
                <span class="sb-tag">Migration</span>
                <span class="sb-tag">Social Movements</span>
                <span class="sb-tag">NLP</span>
            </div>
        </div>

        <div class="sb-divider"></div>

        <div>
            <div class="sb-label">Languages</div>
            <div class="sb-tags">
                <span class="sb-tag">Turkish</span>
                <span class="sb-tag">English</span>
                <span class="sb-tag">Arabic</span>
            </div>
        </div>

    </aside>

    <!-- ════════════════ MAIN ════════════════ -->
    <main class="main">

        <div class="main-hero">
            <div class="hero-name">Şükrü Atsızelti</div>
            <div class="hero-sub">Ph.D. Candidate in Sociology — Koç University</div>
        </div>

        <div class="main-body">

            <!-- Education -->
            <section class="section">
                <div class="section-head">
                    <div class="section-title">Education</div>
                    <div class="section-rule"></div>
                </div>

                <div class="entry">
                    <div class="entry-date">2022–<br>Present</div>
                    <div>
                        <div class="entry-title">Ph.D. in Sociology</div>
                        <div class="entry-org">Koç University, Turkey</div>
                    </div>
                </div>

                <div class="entry">
                    <div class="entry-date">2017–2021</div>
                    <div>
                        <div class="entry-title">M.A. in Migration Studies</div>
                        <div class="entry-org">Istanbul University, Turkey</div>
                        <div class="entry-desc">Thesis: "The use of big data in migration management"</div>
                    </div>
                </div>

                <div class="entry">
                    <div class="entry-date">2013–2017</div>
                    <div>
                        <div class="entry-title">B.A. in Psychology</div>
                        <div class="entry-org">Fatih Sultan Mehmet Waqf University, Turkey</div>
                    </div>
                </div>
            </section>

            <!-- Work Experience -->
            <section class="section">
                <div class="section-head">
                    <div class="section-title">Work Experience</div>
                    <div class="section-rule"></div>
                </div>

                <div class="entry">
                    <div class="entry-date">2022–<br>Present</div>
                    <div>
                        <div class="entry-title">Researcher</div>
                        <div class="entry-org">Enlighty AI</div>
                    </div>
                </div>

                <div class="entry">
                    <div class="entry-date">2018–2019</div>
                    <div>
                        <div class="entry-title">Psychologist</div>
                        <div class="entry-org">World Academy of Local Government and Democracy</div>
                    </div>
                </div>

                <div class="entry">
                    <div class="entry-date">2017–2019</div>
                    <div>
                        <div class="entry-title">Coordinator</div>
                        <div class="entry-org">Press and Publication Association</div>
                    </div>
                </div>

                <div class="entry">
                    <div class="entry-date">2014–2022</div>
                    <div>
                        <div class="entry-title">Freelance Translator</div>
                        <div class="entry-org">Turkish ↔ English · Academic &amp; Technical</div>
                    </div>
                </div>
            </section>

            <!-- Publications -->
            <section class="section">
                <div class="section-head">
                    <div class="section-title">Publications</div>
                    <div class="section-rule"></div>
                </div>

                <div class="pub">
                    <div class="pub-year">2025</div>
                    Atsızelti, Ş. (2025). Computational Research in Ethnic and Migration Studies [Book Review]. <em>International Migration</em>, 63: e70073. <a href="https://doi.org/10.1111/imig.70073">https://doi.org/10.1111/imig.70073</a>
                </div>

                <div class="pub">
                    <div class="pub-year">2025</div>
                    Yörük, E., Atsızelti, Ş., Kına, M.F., Duruşan, F., Gürerk, O., Yardı, M.C., Hürriyetoğlu, A., Mutlu, O., Etgü, T., Koyuncu, M. &amp; Topçu, I. (2025). A Computational Analysis Of Ideological Positions, Emotional Stance, And Support For Presidential Candidates In Turkey. <em>The Developing Economies</em>. <a href="https://doi.org/10.1111/deve.12424">https://doi.org/10.1111/deve.12424</a>
                </div>

                <div class="pub">
                    <div class="pub-year">2024</div>
                    Barkhordar, E., &amp; Atsızelti, Ş. (2024). Assessing the predictive power of social media data-fed large language models on voter behavior. In <em>WebSci Companion '24</em>, Stuttgart, Germany. ACM. <a href="https://doi.org/10.1145/3630744.3659831">https://doi.org/10.1145/3630744.3659831</a>
                </div>

                <div class="pub">
                    <div class="pub-year">2024</div>
                    Kına, M. F., Atsızelti, Ş., Yörük, E., Hürriyetoğlu, A., Yardı, M. C., Duruşan, F., Gürerk, O., Etgü, T., Nişancı, Z., Turbic, G. B., &amp; Akbulut, Y. (2024). Validating digital traces with survey data: The use case of religiosity. In <em>WebSci Companion '24</em>, Stuttgart, Germany. ACM. <a href="https://doi.org/10.1145/3630744.3660242">https://doi.org/10.1145/3630744.3660242</a>
                </div>

                <div class="pub">
                    <div class="pub-year">2023</div>
                    Atsızelti, Ş. (2023). Göçmenler ve Büyük Veri. In Adıgüzel, Y. (ed), <em>Türkiye'nin Yeni Göçmenleri: Suriyeliler</em> (pp. 219–235). Palet Yayınları.
                </div>

                <div class="pub">
                    <div class="pub-year">2022</div>
                    Weinstein, N., Wolf, L., Legault, L., Atsızelti, Ş., Karyofylli, A. &amp; Legate, N. (2022). Will Outgroup Members Satisfy My Need for Autonomy? The Role of Need Expectations in Outgroup Attitudes. <em>Journal of Social and Political Psychology</em>.
                </div>

                <div class="pub">
                    <div class="pub-year">2021</div>
                    Atsızelti, Ş. (2021). The use of big data in migration management. [Master's thesis, Istanbul University].
                </div>
            </section>

            <!-- Conferences & Presentations -->
            <section class="section">
                <div class="section-head">
                    <div class="section-title">Conferences, Presentations &amp; Summer Schools</div>
                    <div class="section-rule"></div>
                </div>

                <ul class="pres-list">
                    <li class="pres-item"><span class="pres-year">2025</span><span>Atsızelti, Ş. Toplumsal Hareketlere Halk Tepkisi: EYT Hareketi Örneği. 18. Ulusal Sosyal Bilimler Kongresi, Ankara, Turkey.</span></li>
                    <li class="pres-item"><span class="pres-year">2025</span><span>Yılmaz, Y., Atsızelti, N. Ş., Uğur, Y., Atsızelti, Ş., Şensin, R. Datafication of Ottoman Sijils Using Large Language Models. Poster at IC2S2 2025, Norrköping, Sweden.</span></li>
                    <li class="pres-item"><span class="pres-year">2025</span><span>Atsızelti, Ş. Total Error Framework for LLM-Based Survey Simulations. Poster at IC2S2 2025, Norrköping, Sweden.</span></li>
                    <li class="pres-item"><span class="pres-year">2025</span><span>Atsızelti, Ş., Hürriyetoğlu, A., Yörük, E., Duruşan, F., Kına, F., Yardı, M. C., Tan, Ş. De-Biasing Large Language Models: Fine-Tuning with in-Group Texts. 5th ISA Forum of Sociology, Rabat, Morocco.</span></li>
                    <li class="pres-item"><span class="pres-year">2025</span><span>Atsızelti, Ş. Simulating Culture Without Twisting It: A Total Error Framework for LLM-Based Survey Simulations. Measuring Culture Workshop, Heidelberg Academy of Sciences, Germany.</span></li>
                    <li class="pres-item"><span class="pres-year">2025</span><span>Atsızelti, Ş. Total Error Framework for LLM-based Survey Simulations. TCSS III, Koç University, Turkey.</span></li>
                    <li class="pres-item"><span class="pres-year">2025</span><span>Atsızelti, Ş. Total Error Framework for LLM-based Survey Simulations. SsaLM: Social Science and Language Models Workshop, Weizenbaum Institut, Germany.</span></li>
                    <li class="pres-item"><span class="pres-year">2025</span><span>Erasmus+ Exchange, Department of Sociology, Egyptology and Anthropology, The American University in Cairo, Egypt.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>Atsızelti, Ş. Büyük Dil Modelleri ile Tarihsel Kamuoyu Simülasyonu. III. Ulusal Siyaset Bilimi Kongresi, Yeditepe Üniversitesi, Turkey.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>Atsızelti, Ş., Hürriyetoğlu, A. Cultural Repertoires and Symbolic Boundaries in Arabic Tweets within the Turkish Twittersphere. Poster at KONVENS 2024, University of Vienna, Austria.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>AI in History – Challenges, Opportunities, and Questions Workshop, University of Heidelberg, Germany.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>Wealth Data Science Summer/Winter School 2024, Constructor University, Germany.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>Hürriyetoğlu, A., Yörük, E., Duruşan, F., et al. How to Use AI to Obtain Representative Public Opinion from X. Poster at IC2S2 2024, Philadelphia, USA.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>Atsızelti, Ş., Duruşan, F., Yardı, M.C., et al. Fine-Tuning Pre-Trained Models by LLM-Generated Annotations. Generative AI as a Method of Social Sciences, Monash University / Aalto University.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>Kına, M. F., Atsızelti, Ş., et al. Validating Digital Traces with Survey Data: The Use Case of Religiosity. WebSci 2024, University of Stuttgart, Germany.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>Atsızelti, Ş. Arab Users' Stances Toward Turkey within Turkish Twittersphere. TCSS 2024, Koç University, Turkey.</span></li>
                    <li class="pres-item"><span class="pres-year">2024</span><span>Kına, F., Atsızelti, Ş. Linking Surveys and Social Media Data. Web Data Opp Workshop, University Pompeu Fabra, Spain.</span></li>
                    <li class="pres-item"><span class="pres-year">2023</span><span>Atsızelti, Ş. Mimicking Surveys within Turkish Context using ChatGPT. TCSS, Koç University, Turkey.</span></li>
                    <li class="pres-item"><span class="pres-year">2023</span><span>Social ComQuant Summer School: Recent Advances in Computational Social Science Methods, ISI, Italy.</span></li>
                    <li class="pres-item"><span class="pres-year">2023</span><span>Computational Social Science Summer School on Democratic Debate, Constructor University, Germany.</span></li>
                    <li class="pres-item"><span class="pres-year">2023</span><span>5th Interdisciplinary Summerschool on Privacy, Radboud University, Netherlands.</span></li>
                    <li class="pres-item"><span class="pres-year">2023</span><span>Social ComQuant Exchange Program, GESIS, Germany.</span></li>
                    <li class="pres-item"><span class="pres-year">2022</span><span>Social ComQuant Summer School: Text Mining and NLP for Computational Social Sciences, Koç University, Turkey.</span></li>
                    <li class="pres-item"><span class="pres-year">2021</span><span>Atsızelti, Ş. Göç Yönetimi Çalışmalarında Büyük Veri Kaynaklarının Kullanımı. III. Göç Çalışmaları Lisansüstü Öğrenci Konferansı, Bilgi University, Turkey.</span></li>
                    <li class="pres-item"><span class="pres-year">2019</span><span>8. Yılında Türkiye'de Suriyeliler Atölyesi, İstanbul University, Turkey.</span></li>
                    <li class="pres-item"><span class="pres-year">2019</span><span>Analytics &amp; Data Science Summer School, Essex University, United Kingdom.</span></li>
                    <li class="pres-item"><span class="pres-year">2016</span><span>Erasmus+ Internship, School of Psychology, Cardiff University, United Kingdom.</span></li>
                </ul>
            </section>

            <!-- Organized Events -->
            <section class="section">
                <div class="section-head">
                    <div class="section-title">Organized Events</div>
                    <div class="section-rule"></div>
                </div>

                <div class="entry">
                    <div class="entry-date">2026</div>
                    <div>
                        <div class="entry-desc">Turkey Computational Social Sciences Conference TCSS IV, Istanbul, Turkey.</div>
                    </div>
                </div>

                <div class="entry">
                    <div class="entry-date">2025</div>
                    <div>
                        <div class="entry-desc">Turkey Computational Social Sciences Conference TCSS III, Istanbul, Turkey.</div>
                    </div>
                </div>

                <div class="entry">
                    <div class="entry-date">2024</div>
                    <div>
                        <div class="entry-desc">Kına, M. F., Atsızelti, Ş., Gürerk, O., Yörük, E., Hürriyetoğlu, A. 16th ACM Web Science Conference WebSci'24 — Linking Surveys and Social Media Data: Advancing Public Opinion Research (LASER) Workshop, University of Stuttgart, Germany.</div>
                    </div>
                </div>

                <div class="entry">
                    <div class="entry-date">2019</div>
                    <div>
                        <div class="entry-desc">Türkiye'de Uluslararası Göç ve Hak Savunuculuğu, Müştereklerimiz Atölyeleri (International Migration and Rights Advocacy in Turkey, Our Commons Workshops).</div>
                    </div>
                </div>
            </section>

        </div>
    </main>

</div>
</body>
</html>
