<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Şükrü Atsızelti | Ph.D. Candidate in Sociology</title>
    <style>
        /* General styling */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Raleway', 'Helvetica Neue', Arial, sans-serif;
        }
        
        body {
            background-color: #ffffff;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 0;
            position: relative;
        }
        
        /* Colors based on LaTeX template */
        :root {
            --accent-color: #ff9600; /* sectcol - orange */
            --dark-bg: #6e6e6e; /* bgcol - dark gray */
            --light-bg: #e1e1e1; /* softcol - light gray */
        }
        
        /* Header styling */
        .title-header {
            background-color: var(--dark-bg);
            padding: 20px;
            margin: 0 -25%;
            width: 150%;
            position: relative;
            color: white;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .title-content {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-left: 25%;
        }
        
        .name-title {
            font-size: 2.8rem;
            text-transform: uppercase;
            font-weight: 700;
            letter-spacing: 1px;
        }
        
        .resume-title {
            font-size: 2.8rem;
            text-transform: uppercase;
            font-weight: 700;
        }
        
        .separator {
            width: 5px;
            height: 40px;
            background-color: var(--accent-color);
            display: inline-block;
            margin: 0 15px;
        }
        
        .profile-image {
            margin-right: 25%;
            width: 120px;
            height: 120px;
            overflow: hidden;
            border-radius: 5px;
        }
        
        .profile-image img {
            width: 100%;
            height: auto;
        }
        
        /* Meta section styling */
        .meta-section {
            margin-top: -60px;
            padding-top: 80px;
            margin-bottom: 30px;
        }
        
        .meta-item {
            display: flex;
            margin-bottom: 12px;
            align-items: center;
        }
        
        .meta-label {
            width: 100px;
            display: flex;
            align-items: center;
        }
        
        .arrow {
            width: 0;
            height: 0;
            border-top: 8px solid transparent;
            border-bottom: 8px solid transparent;
            border-right: 14px solid var(--dark-bg);
            margin-right: 10px;
        }
        
        .meta-label span {
            color: var(--accent-color);
            font-weight: bold;
        }
        
        /* Section styling */
        .cv-section {
            margin-bottom: 30px;
        }
        
        .section-header {
            background-color: var(--accent-color);
            padding: 10px 15px;
            color: white;
            font-weight: bold;
            font-size: 1.2rem;
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }
        
        .section-header .arrows {
            display: flex;
            margin-right: 10px;
        }
        
        .section-header .arrow-left {
            width: 0;
            height: 0;
            border-top: 8px solid transparent;
            border-bottom: 8px solid transparent;
            border-right: 14px solid var(--dark-bg);
            margin-right: 3px;
        }
        
        /* Event styling (for education and work) */
        .cv-entry {
            margin-bottom: 20px;
        }
        
        .entry-header {
            display: flex;
            flex-wrap: wrap;
        }
        
        .entry-date {
            width: 120px;
            color: var(--dark-bg);
            font-weight: bold;
        }
        
        .entry-title {
            font-weight: bold;
            flex: 1;
        }
        
        .entry-org {
            width: 200px;
            text-align: right;
            color: var(--accent-color);
        }
        
        .entry-divider {
            height: 1px;
            background-color: var(--light-bg);
            margin: 8px 0;
        }
        
        .entry-content {
            display: flex;
            flex-direction: column;
            margin-left: 120px;
        }
        
        .entry-point {
            display: flex;
            align-items: flex-start;
            margin-bottom: 5px;
        }
        
        .entry-point .arrow-left {
            min-width: 14px;
            height: 16px;
            margin-right: 10px;
            margin-top: 5px;
            position: relative;
        }
        
        .entry-point .arrow-left::before {
            content: "";
            position: absolute;
            width: 0;
            height: 0;
            border-top: 8px solid transparent;
            border-bottom: 8px solid transparent;
            border-right: 14px solid var(--dark-bg);
        }
        
        /* Publications styling */
        .pub-entry {
            display: flex;
            margin-bottom: 15px;
        }
        
        .pub-date {
            width: 120px;
            color: var(--dark-bg);
            font-weight: bold;
        }
        
        .pub-text {
            flex: 1;
        }
        
        /* Footer styling */
        .footer {
            background-color: var(--dark-bg);
            color: white;
            text-align: center;
            padding: 10px;
            margin: 0 -25%;
            width: 150%;
        }
        
        .footer a {
            color: white;
            text-decoration: none;
        }
        
        /* Links styling */
        a {
            color: var(--accent-color);
            text-decoration: none;
        }
        
        a:hover {
            text-decoration: underline;
        }
        
        /* Responsive design */
        @media (max-width: 768px) {
            .title-header {
                flex-direction: column;
                margin: 0 -10%;
                width: 120%;
            }
            
            .title-content {
                margin-left: 0;
                flex-direction: column;
                text-align: center;
                gap: 5px;
            }
            
            .separator {
                height: 5px;
                width: 100px;
                margin: 10px 0;
            }
            
            .profile-image {
                margin-right: 0;
                margin-top: 20px;
            }
            
            .meta-section {
                margin-top: 20px;
                padding-top: 0;
            }
            
            .entry-header {
                flex-direction: column;
            }
            
            .entry-org {
                width: 100%;
                text-align: left;
                margin-top: 5px;
            }
            
            .entry-content {
                margin-left: 0;
            }
            
            .footer {
                margin: 0 -10%;
                width: 120%;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Title Header -->
        <header class="title-header">
            <div class="title-content">
                <h1 class="name-title">Şükrü Atsızelti</h1>
                <span class="separator"></span>
                <h1 class="resume-title">Resume</h1>
            </div>
            <div class="profile-image">
                <img src="assets/images/profile.jpg" alt="Profile Photo">
            </div>
        </header>

        <!-- Meta Section -->
        <section class="meta-section">
            <div class="meta-item">
                <div class="meta-label">
                    <div class="arrow"></div>
                    <span>Status:</span>
                </div>
                <p>Ph.D. Candidate in Sociology, Koç University</p>
            </div>
            <div class="meta-item">
                <div class="meta-label">
                    <div class="arrow"></div>
                    <span>Research:</span>
                </div>
                <p>Computational Social Science, Public Opinion, Migration, Social Movements</p>
            </div>
            <div class="meta-item">
                <div class="meta-label">
                    <div class="arrow"></div>
                    <span>Languages:</span>
                </div>
                <p>English, Arabic, Turkish</p>
            </div>
            <div class="meta-item">
                <div class="meta-label">
                    <div class="arrow"></div>
                    <span>Contact:</span>
                </div>
                <p><a href="mailto:satsizelti22@ku.edu.tr">satsizelti22@ku.edu.tr</a></p>
            </div>
        </section>

        <!-- Education Section -->
        <section class="cv-section" id="education">
            <div class="section-header">
                <div class="arrows">
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                </div>
                Education
            </div>
            
            <div class="cv-entry">
                <div class="entry-header">
                    <span class="entry-date">2022-Present</span>
                    <span class="entry-title">Sociology, Ph.D.</span>
                    <span class="entry-org">Koç University</span>
                </div>
                <div class="entry-divider"></div>
                <div class="entry-content">
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Pursuing doctoral studies in Sociology with focus on computational methods</p>
                    </div>
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Research in computational social science, public opinion and social movements</p>
                    </div>
                </div>
            </div>
            
            <div class="cv-entry">
                <div class="entry-header">
                    <span class="entry-date">2017-2021</span>
                    <span class="entry-title">Migration Studies, M.A.</span>
                    <span class="entry-org">Istanbul University</span>
                </div>
                <div class="entry-divider"></div>
                <div class="entry-content">
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Master's thesis: "The use of big data in migration management"</p>
                    </div>
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Investigated computational methods in migration research</p>
                    </div>
                </div>
            </div>
            
            <div class="cv-entry">
                <div class="entry-header">
                    <span class="entry-date">2013-2017</span>
                    <span class="entry-title">Psychology, B.A.</span>
                    <span class="entry-org">Fatih Sultan Mehmet Waqf University</span>
                </div>
                <div class="entry-divider"></div>
                <div class="entry-content">
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Studied psychology with interest in social psychology and refugee experience</p>
                    </div>
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Developed foundation in statistics and survey research</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Work Experience Section -->
        <section class="cv-section" id="experience">
            <div class="section-header">
                <div class="arrows">
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                </div>
                Work Experience
            </div>
            
            <div class="cv-entry">
                <div class="entry-header">
                    <span class="entry-date">2022-Present</span>
                    <span class="entry-title">Researcher</span>
                    <span class="entry-org">Politus Analytics</span>
                </div>
                <div class="entry-divider"></div>
                <div class="entry-content">
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Conduct advanced computational social science research</p>
                    </div>
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Apply computational methods to understand public opinion and customer journey</p>
                    </div>
                </div>
            </div>
            
            <div class="cv-entry">
                <div class="entry-header">
                    <span class="entry-date">2018-2019</span>
                    <span class="entry-title">Psychologist</span>
                    <span class="entry-org">World Academy of Local Government and Democracy</span>
                </div>
                <div class="entry-divider"></div>
                <div class="entry-content">
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Provided psycho-social support services</p>
                    </div>
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Applied psychology principles to support community development initiatives</p>
                    </div>
                </div>
            </div>
            
            <div class="cv-entry">
                <div class="entry-header">
                    <span class="entry-date">2017-2019</span>
                    <span class="entry-title">Coordinator</span>
                    <span class="entry-org">Press and Publication Association</span>
                </div>
                <div class="entry-divider"></div>
                <div class="entry-content">
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Managed press and publication projects</p>
                    </div>
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Coordinated member relations, bookfairs and workshops</p>
                    </div>
                </div>
            </div>
            
            <div class="cv-entry">
                <div class="entry-header">
                    <span class="entry-date">2014-2022</span>
                    <span class="entry-title">Freelance Translator</span>
                    <span class="entry-org">Various Clients</span>
                </div>
                <div class="entry-divider"></div>
                <div class="entry-content">
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Provided professional translation services with 10 academic translations</p>
                    </div>
                    <div class="entry-point">
                        <div class="arrow-left"></div>
                        <p>Specialized in academic and technical translations between Turkish and English</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Publications Section -->
        <section class="cv-section" id="publications">
            <div class="section-header">
                <div class="arrows">
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                </div>
                Publications
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2025</span>
                <p class="pub-text">Yörük, E., Atsızelti, Ş., Kına, M.F., Duruşan, F., Gürerk, O., Yardı, M.C., Hürriyetoğlu, A., Mutlu, O., Etgü, T., Koyuncu, M. and Topçu, I. (2025), A Computational Analysis Of Ideological Positions, Emotional Stance, And Support For Presidential Candidates In Turkey. The Developing Economies. <a href="https://doi.org/10.1111/deve.12424">https://doi.org/10.1111/deve.12424</a></p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Kına, M. F., Atsızelti, Ş., Yörük, E., Hürriyetoğlu, A., Yardı, M. C., Duruşan, F., Gürerk, O., Etgü, T., Nişancı, Z., Turbic, G. B., & Akbulut, Y. (2024). Validating digital traces with survey data: The use case of religiosity. In 16th ACM Web Science Conference (WebSci Companion '24), May 21–24, 2024, Stuttgart, Germany. ACM, New York, NY, USA, 4 pages. <a href="https://doi.org/10.1145/3630744.3660242">https://doi.org/10.1145/3630744.3660242</a></p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Barkhordar, E., & Atsızelti, Ş. (2024). Assessing the predictive power of social media data-fed large language models on voter behavior. In 16th ACM Web Science Conference (WebSci Companion '24), May 21–24, 2024, Stuttgart, Germany. ACM, New York, NY, USA, 3 pages. <a href="https://doi.org/10.1145/3630744.3659831">https://doi.org/10.1145/3630744.3659831</a></p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2023</span>
                <p class="pub-text">Atsızelti, Ş. (2023). Göçmenler ve Büyük Veri. In Adıgüzel, Y. (ed), Türkiye'nin Yeni Göçmenleri: Suriyeliler (pp. 219-235). Palet Yayınları</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2022</span>
                <p class="pub-text">Weinstein, N., Wolf, L., Legault L., Atsızelti, Ş., Karyofylli, A. & Legate, N. (2022). Will Outgroup Members Satisfy My Need for Autonomy? The Role of Need Expectations in Outgroup Attitudes. Journal of Social and Political Psychology.</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2021</span>
                <p class="pub-text">Atsızelti, Ş. (2021). The use of big data in migration management. [Master's thesis, Istanbul University]</p>
            </div>
        </section>

        <!-- Summer Schools Section -->
        <section class="cv-section" id="summer-schools">
            <div class="section-header">
                <div class="arrows">
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                </div>
                Summer Schools, Exchanges, Workshops, Conferences and Poster Presentations
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2025</span>
                <p class="pub-text">Total Error Framework for LLM-based Survey Simulations, SsaLM: Social Science and Language Models Workshop, Weizenbaum Institut, Germany</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2025</span>
                <p class="pub-text">Erasmus+ Exchange, Department of Sociology, Egyptology and Anthropology, The American University in Cairo, Egypt</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Büyük Dil Modelleri ile Tarihsel Kamuoyu Simülasyonu: Türkçe ve İngilizce Veriler Üzerine Karşılaştırmalı Bir Analiz, III. Ulusal Siyaset Bilimi Kongresi, Yeditepe Üniversitesi, Türkiye</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Atsizelti, Ş., Hürriyetoğlu, A. Cultural Repertoires and Symbolic Boundaries in Arabic Tweets within the Turkish, Poster presentation at Conference on Natural Language Processing KONVENS 2024/4th Workshop on Computational Linguistics for the Political and Social Sciences, University of Vienna, Austria</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">AI in History – Challenges, Opportunities, and Questions Workshop, University of Heidelberg, Germany</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Wealth Data Science Summer/Winter School 2024, Constructor University, Germany</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Hürriyetoğlu, A., Yörük, E., Duruşan, F., Topçu, I., Kına, M. F., Yardı, M. C. Gürerk, O., Etgü, T., Atsızelti, A. How to Use AI to Obtain Representative Public Opinion from X, poster presentation at 10th International Conference on Computational Social Science, Philadelphia, USA</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Atsızelti, Ş., Duruşan F., Yardı, M.C., Delen, M, Gürerk, O., Kına F., Tan, Ş., Hürriyetoğlu, A., Yörük E. Fine-Tuning Pre-Trained Models by LLM-Generated Annotations, Generative AI as a method of social sciences, Emerging Technologies Research Lab Monash University, Australia & Imagining Sustainable Digital Futures, Aalto University, Finland</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Kına, M. F., Atsızelti, Ş., Yörük, E., Hürriyetoğlu, A., Yardı, M. C., Duruşan, F., Gürerk, O., Etgü, T., Nişancı, Z., Turbic, G. B., & Akbulut, Y. Validating Digital Traces with Survey Data: The Use Case of Religiosity, 16.ACM Web Science Conference 2024, University of Stuttgart, Germany</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Arab Users' Stances Toward Turkey within Turkish Twittersphere, Turkey Computational Social Sciences Conference 2024, Koç University, Türkiye</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Kına, F., Atsızelti, Ş. Linking Surveys and Social Media Data: Shaping the Future of Public Opinion Research with the Politus Project, Web Data Opp Workshop, University Pompeu Fabra, Spain</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2023</span>
                <p class="pub-text">Mimicking Surveys within Turkish Context using ChatGPT, Turkey Computational Social Sciences Conference, Koç University, Türkiye</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2023</span>
                <p class="pub-text">Social ComQuant Summer School: Recent Advances in Computational Social Sciences Methods, ISI, Italy</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2023</span>
                <p class="pub-text">Computational Social Science Summer School on Democratic Debate, Constructor University, Germany</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2023</span>
                <p class="pub-text">5th Interdisciplinary Summerschool on Privacy, Radboud University, Netherlands</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2023</span>
                <p class="pub-text">Social ComQuant Exchange Program, Gesis, Germany</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2022</span>
                <p class="pub-text">Social ComQuant Summer School: Text mining and Natural Language Processing for Computational Social Sciences, Koç University, Türkiye</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2021</span>
                <p class="pub-text">Göç Yönetimi Çalışmalarında Büyük Veri Kaynaklarının Kullanımı, III. Göç Çalışmaları Lisansüstü Öğrenci Konferansı, Bilgi University, Türkiye</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2019</span>
                <p class="pub-text">8. Yılında Türkiye'de Suriyeliler Atölyesi, İstanbul University, Türkiye</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2019</span>
                <p class="pub-text">Analytics & Data Science Summer School, Essex University, United Kingdom</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2016</span>
                <p class="pub-text">Erasmus+ Internship, School of Psychology, Cardiff University, United Kingdom</p>
            </div>
        </section>

        <!-- Organized Workshops Section -->
        <section class="cv-section" id="organized-workshops">
            <div class="section-header">
                <div class="arrows">
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                </div>
                Organized Workshops
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Kına, M. F., Atsızelti, Ş., Gürerk, O., Yörük, E., Hürriyetoğlu, A. 16th ACM Web Science Conference WebSci'24, Linking Surveys and Social Media Data: Advancing Public Opinion Research (LASER) Workshop, University of Stuttgart, Germany</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2019</span>
                <p class="pub-text">Türkiye'de Uluslararası Göç ve Hak Savunuculuğu, Müştereklerimiz Atölyeleri (International Migration and Rights Advocacy in Turkey, Our Commons Workshops)</p>
            </div>
        </section>

        <!-- Invited Talks Section -->
        <section class="cv-section" id="talks">
            <div class="section-header">
                <div class="arrows">
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                    <div class="arrow-left"></div>
                </div>
                Invited Talks and Presentations
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2024</span>
                <p class="pub-text">Büyük Dil Modellerinin Sosyal Bilimlerde Kullanımı, Dijital Beşeri Bilimler Uygulama ve Araştırma Merkezi, Marmara University, Türkiye</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2023</span>
                <p class="pub-text">The Integration of Large Language Models in Text Annotation and Social Science Research, CSS Seminar Series, Center for Computational Social Sciences, Koç University, Türkiye</p>
            </div>
            
            <div class="pub-entry">
                <span class="pub-date">2023</span>
                <p class="pub-text">Matching Survey Data with Social Media Data (with Dr. Fuat Kına), SICSS-Istanbul</p>
            </div>
        </section>

        <!-- Footer -->
        <footer class="footer">
            <p>Email: <a href="mailto:satsizelti22@ku.edu.tr">satsizelti22@ku.edu.tr</a></p>
        </footer>
    </div>
</body>
</html>
