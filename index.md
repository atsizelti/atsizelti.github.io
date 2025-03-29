<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Şükrü Atsızelti | Ph.D. Candidate in Sociology</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Helvetica Neue', Arial, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: #333;
            max-width: 900px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Colors */
        :root {
            --orange: #ff9600;
            --dark-gray: #6e6e6e;
            --light-gray: #f0f0f0;
        }
        
        /* Header */
        .header {
            background-color: var(--dark-gray);
            color: white;
            padding: 30px;
            margin-bottom: 30px;
            text-align: center;
        }
        
        .name-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .name {
            font-size: 32px;
            font-weight: bold;
            text-transform: uppercase;
            margin-bottom: 20px;
        }
        
        .photo {
            width: 120px;
            height: 120px;
            border: 3px solid var(--orange);
            border-radius: 4px;
            overflow: hidden;
        }
        
        .photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        /* Meta info section */
        .meta-info {
            display: flex;
            flex-wrap: wrap;
            gap: 15px 40px;
            background-color: var(--light-gray);
            padding: 20px;
            margin-bottom: 30px;
        }
        
        .meta-item {
            flex-basis: calc(50% - 20px);
        }
        
        .meta-label {
            color: var(--orange);
            font-weight: bold;
            margin-right: 5px;
        }
        
        /* Section styles */
        .section {
            margin-bottom: 30px;
        }
        
        .section-title {
            background-color: var(--orange);
            color: white;
            padding: 8px 15px;
            font-size: 18px;
            font-weight: bold;
            margin-bottom: 15px;
            position: relative;
        }
        
        .section-title:before {
            content: "▶▶▶";
            margin-right: 10px;
            font-size: 14px;
            color: var(--dark-gray);
        }
        
        /* Entry styles */
        .entry {
            display: flex;
            margin-bottom: 20px;
        }
        
        .date {
            width: 120px;
            color: var(--dark-gray);
            font-weight: bold;
            flex-shrink: 0;
        }
        
        .content {
            flex-grow: 1;
        }
        
        .position {
            font-weight: bold;
        }
        
        .organization {
            color: var(--orange);
            font-weight: bold;
        }
        
        .description {
            margin-top: 5px;
        }
        
        .description ul {
            list-style: none;
            margin-left: 5px;
        }
        
        .description li {
            position: relative;
            padding-left: 15px;
            margin-bottom: 5px;
        }
        
        .description li:before {
            content: "▶";
            position: absolute;
            left: 0;
            color: var(--dark-gray);
            font-size: 10px;
        }
        
        /* Footer */
        .footer {
            background-color: var(--dark-gray);
            color: white;
            padding: 15px;
            text-align: center;
            margin-top: 30px;
        }
        
        .footer a {
            color: white;
            text-decoration: none;
        }
        
        /* Links */
        a {
            color: var(--orange);
            text-decoration: none;
        }
        
        a:hover {
            text-decoration: underline;
        }
        
        /* Mobile adjustments */
        @media (max-width: 768px) {
            .header {
                flex-direction: column;
                gap: 20px;
            }
            
            .meta-item {
                flex-basis: 100%;
            }
            
            .entry {
                flex-direction: column;
            }
            
            .date {
                margin-bottom: 5px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="name-container">
            <h1 class="name">Şükrü Atsızelti</h1>
            <div class="photo">
                <img src="assets/images/profile.jpg" alt="Profile Photo">
            </div>
        </div>
    </header>

    <!-- Meta Information -->
    <section class="meta-info">
        <div class="meta-item">
            <span class="meta-label">Status:</span>
            <span>Ph.D. Candidate in Sociology, Koç University</span>
        </div>
        <div class="meta-item">
            <span class="meta-label">Research:</span>
            <span>Computational Social Science, Public Opinion, Migration, Social Movements</span>
        </div>
        <div class="meta-item">
            <span class="meta-label">Languages:</span>
            <span>English, Arabic, Turkish</span>
        </div>
        <div class="meta-item">
            <span class="meta-label">Contact:</span>
            <a href="mailto:satsizelti22@ku.edu.tr">satsizelti22@ku.edu.tr</a>
        </div>
    </section>

    <!-- Education Section -->
    <section class="section">
        <h2 class="section-title">Education</h2>
        
        <div class="entry">
            <div class="date">2022-Present</div>
            <div class="content">
                <div>
                    <span class="position">Sociology, Ph.D.</span> - 
                    <span class="organization">Koç University</span>
                </div>
                <div class="description">
                    <ul>
                        <li>Pursuing doctoral studies in Sociology with focus on computational methods</li>
                        <li>Research in computational social science, public opinion and social movements</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2017-2021</div>
            <div class="content">
                <div>
                    <span class="position">Migration Studies, M.A.</span> - 
                    <span class="organization">Istanbul University</span>
                </div>
                <div class="description">
                    <ul>
                        <li>Master's thesis: "The use of big data in migration management"</li>
                        <li>Investigated computational methods in migration research</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2013-2017</div>
            <div class="content">
                <div>
                    <span class="position">Psychology, B.A.</span> - 
                    <span class="organization">Fatih Sultan Mehmet Waqf University</span>
                </div>
                <div class="description">
                    <ul>
                        <li>Studied psychology with interest in social psychology and refugee experience</li>
                        <li>Developed foundation in statistics and survey research</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Work Experience Section -->
    <section class="section">
        <h2 class="section-title">Work Experience</h2>
        
        <div class="entry">
            <div class="date">2022-Present</div>
            <div class="content">
                <div>
                    <span class="position">Researcher</span> - 
                    <span class="organization">Politus Analytics</span>
                </div>
                <div class="description">
                    <ul>
                        <li>Conduct advanced computational social science research</li>
                        <li>Apply computational methods to understand public opinion and customer journey</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2018-2019</div>
            <div class="content">
                <div>
                    <span class="position">Psychologist</span> - 
                    <span class="organization">World Academy of Local Government and Democracy</span>
                </div>
                <div class="description">
                    <ul>
                        <li>Provided psycho-social support services</li>
                        <li>Applied psychology principles to support community development initiatives</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2017-2019</div>
            <div class="content">
                <div>
                    <span class="position">Coordinator</span> - 
                    <span class="organization">Press and Publication Association</span>
                </div>
                <div class="description">
                    <ul>
                        <li>Managed press and publication projects</li>
                        <li>Coordinated member relations, bookfairs and workshops</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2014-2022</div>
            <div class="content">
                <div>
                    <span class="position">Freelance Translator</span> - 
                    <span class="organization">Various Clients</span>
                </div>
                <div class="description">
                    <ul>
                        <li>Provided professional translation services with 10 academic translations</li>
                        <li>Specialized in academic and technical translations between Turkish and English</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Publications Section -->
    <section class="section">
        <h2 class="section-title">Publications</h2>
        
        <div class="entry">
            <div class="date">2025</div>
            <div class="content">
                Yörük, E., Atsızelti, Ş., Kına, M.F., Duruşan, F., Gürerk, O., Yardı, M.C., Hürriyetoğlu, A., Mutlu, O., Etgü, T., Koyuncu, M. and Topçu, I. (2025), A Computational Analysis Of Ideological Positions, Emotional Stance, And Support For Presidential Candidates In Turkey. The Developing Economies. <a href="https://doi.org/10.1111/deve.12424">https://doi.org/10.1111/deve.12424</a>
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Kına, M. F., Atsızelti, Ş., Yörük, E., Hürriyetoğlu, A., Yardı, M. C., Duruşan, F., Gürerk, O., Etgü, T., Nişancı, Z., Turbic, G. B., & Akbulut, Y. (2024). Validating digital traces with survey data: The use case of religiosity. In 16th ACM Web Science Conference (WebSci Companion '24), May 21–24, 2024, Stuttgart, Germany. ACM, New York, NY, USA, 4 pages. <a href="https://doi.org/10.1145/3630744.3660242">https://doi.org/10.1145/3630744.3660242</a>
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Barkhordar, E., & Atsızelti, Ş. (2024). Assessing the predictive power of social media data-fed large language models on voter behavior. In 16th ACM Web Science Conference (WebSci Companion '24), May 21–24, 2024, Stuttgart, Germany. ACM, New York, NY, USA, 3 pages. <a href="https://doi.org/10.1145/3630744.3659831">https://doi.org/10.1145/3630744.3659831</a>
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2023</div>
            <div class="content">
                Atsızelti, Ş. (2023). Göçmenler ve Büyük Veri. In Adıgüzel, Y. (ed), Türkiye'nin Yeni Göçmenleri: Suriyeliler (pp. 219-235). Palet Yayınları
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2022</div>
            <div class="content">
                Weinstein, N., Wolf, L., Legault L., Atsızelti, Ş., Karyofylli, A. & Legate, N. (2022). Will Outgroup Members Satisfy My Need for Autonomy? The Role of Need Expectations in Outgroup Attitudes. Journal of Social and Political Psychology.
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2021</div>
            <div class="content">
                Atsızelti, Ş. (2021). The use of big data in migration management. [Master's thesis, Istanbul University]
            </div>
        </div>
    </section>

    <!-- Summer Schools Section -->
    <section class="section">
        <h2 class="section-title">Summer Schools, Exchanges, Workshops, Conferences and Poster Presentations</h2>
        
        <div class="entry">
            <div class="date">2025</div>
            <div class="content">
                Total Error Framework for LLM-based Survey Simulations, SsaLM: Social Science and Language Models Workshop, Weizenbaum Institut, Germany
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2025</div>
            <div class="content">
                Erasmus+ Exchange, Department of Sociology, Egyptology and Anthropology, The American University in Cairo, Egypt
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Büyük Dil Modelleri ile Tarihsel Kamuoyu Simülasyonu: Türkçe ve İngilizce Veriler Üzerine Karşılaştırmalı Bir Analiz, III. Ulusal Siyaset Bilimi Kongresi, Yeditepe Üniversitesi, Türkiye
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Atsizelti, Ş., Hürriyetoğlu, A. Cultural Repertoires and Symbolic Boundaries in Arabic Tweets within the Turkish, Poster presentation at Conference on Natural Language Processing KONVENS 2024/4th Workshop on Computational Linguistics for the Political and Social Sciences, University of Vienna, Austria
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                AI in History – Challenges, Opportunities, and Questions Workshop, University of Heidelberg, Germany
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Wealth Data Science Summer/Winter School 2024, Constructor University, Germany
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Hürriyetoğlu, A., Yörük, E., Duruşan, F., Topçu, I., Kına, M. F., Yardı, M. C. Gürerk, O., Etgü, T., Atsızelti, A. How to Use AI to Obtain Representative Public Opinion from X, poster presentation at 10th International Conference on Computational Social Science, Philadelphia, USA
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Atsızelti, Ş., Duruşan F., Yardı, M.C., Delen, M, Gürerk, O., Kına F., Tan, Ş., Hürriyetoğlu, A., Yörük E. Fine-Tuning Pre-Trained Models by LLM-Generated Annotations, Generative AI as a method of social sciences, Emerging Technologies Research Lab Monash University, Australia & Imagining Sustainable Digital Futures, Aalto University, Finland
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Kına, M. F., Atsızelti, Ş., Yörük, E., Hürriyetoğlu, A., Yardı, M. C., Duruşan, F., Gürerk, O., Etgü, T., Nişancı, Z., Turbic, G. B., & Akbulut, Y. Validating Digital Traces with Survey Data: The Use Case of Religiosity, 16.ACM Web Science Conference 2024, University of Stuttgart, Germany
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Arab Users' Stances Toward Turkey within Turkish Twittersphere, Turkey Computational Social Sciences Conference 2024, Koç University, Türkiye
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Kına, F., Atsızelti, Ş. Linking Surveys and Social Media Data: Shaping the Future of Public Opinion Research with the Politus Project, Web Data Opp Workshop, University Pompeu Fabra, Spain
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2023</div>
            <div class="content">
                Mimicking Surveys within Turkish Context using ChatGPT, Turkey Computational Social Sciences Conference, Koç University, Türkiye
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2023</div>
            <div class="content">
                Social ComQuant Summer School: Recent Advances in Computational Social Sciences Methods, ISI, Italy
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2023</div>
            <div class="content">
                Computational Social Science Summer School on Democratic Debate, Constructor University, Germany
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2023</div>
            <div class="content">
                5th Interdisciplinary Summerschool on Privacy, Radboud University, Netherlands
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2023</div>
            <div class="content">
                Social ComQuant Exchange Program, Gesis, Germany
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2022</div>
            <div class="content">
                Social ComQuant Summer School: Text mining and Natural Language Processing for Computational Social Sciences, Koç University, Türkiye
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2021</div>
            <div class="content">
                Göç Yönetimi Çalışmalarında Büyük Veri Kaynaklarının Kullanımı, III. Göç Çalışmaları Lisansüstü Öğrenci Konferansı, Bilgi University, Türkiye
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2019</div>
            <div class="content">
                8. Yılında Türkiye'de Suriyeliler Atölyesi, İstanbul University, Türkiye
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2019</div>
            <div class="content">
                Analytics & Data Science Summer School, Essex University, United Kingdom
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2016</div>
            <div class="content">
                Erasmus+ Internship, School of Psychology, Cardiff University, United Kingdom
            </div>
        </div>
    </section>

    <!-- Organized Workshops Section -->
    <section class="section">
        <h2 class="section-title">Organized Workshops</h2>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Kına, M. F., Atsızelti, Ş., Gürerk, O., Yörük, E., Hürriyetoğlu, A. 16th ACM Web Science Conference WebSci'24, Linking Surveys and Social Media Data: Advancing Public Opinion Research (LASER) Workshop, University of Stuttgart, Germany
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2019</div>
            <div class="content">
                Türkiye'de Uluslararası Göç ve Hak Savunuculuğu, Müştereklerimiz Atölyeleri (International Migration and Rights Advocacy in Turkey, Our Commons Workshops)
            </div>
        </div>
    </section>

    <!-- Invited Talks Section -->
    <section class="section">
        <h2 class="section-title">Invited Talks and Presentations</h2>
        
        <div class="entry">
            <div class="date">2024</div>
            <div class="content">
                Büyük Dil Modellerinin Sosyal Bilimlerde Kullanımı, Dijital Beşeri Bilimler Uygulama ve Araştırma Merkezi, Marmara University, Türkiye
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2023</div>
            <div class="content">
                The Integration of Large Language Models in Text Annotation and Social Science Research, CSS Seminar Series, Center for Computational Social Sciences, Koç University, Türkiye
            </div>
        </div>
        
        <div class="entry">
            <div class="date">2023</div>
            <div class="content">
                Matching Survey Data with Social Media Data (with Dr. Fuat Kına), SICSS-Istanbul
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <p>Email: <a href="mailto:satsizelti22@ku.edu.tr">satsizelti22@ku.edu.tr</a></p>
    </footer>
</body>
</html>
