<!DOCTYPE html>
<html lang="tr" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Doruk Çelik | Data Science & Machine Learning Showcase</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .glass-card {
            background: rgba(15, 23, 42, 0.75);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }
        .glass-card:hover {
            border-color: rgba(99, 102, 241, 0.4);
            box-shadow: 0 0 25px rgba(99, 102, 241, 0.15);
        }
        .bg-grid-pattern {
            background-image: radial-gradient(rgba(99, 102, 241, 0.15) 1px, transparent 1px);
            background-size: 24px 24px;
        }
    </style>
</head>
<body class="bg-slate-950 text-slate-100 font-sans antialiased bg-grid-pattern selection:bg-indigo-500 selection:text-white">

    <!-- Navigation Bar -->
    <nav class="fixed top-0 w-full z-50 glass-card border-b border-slate-800/80 px-6 py-4">
        <div class="max-w-6xl mx-auto flex justify-between items-center">
            <a href="#" class="text-lg font-bold tracking-wider text-white flex items-center gap-2">
                <span class="text-indigo-400 font-mono">&lt;D/Ç&gt;</span> Doruk Çelik
            </a>
            <div class="hidden md:flex items-center gap-6 text-sm font-medium text-slate-300">
                <a href="#about" class="hover:text-indigo-400 transition">Hakkımda</a>
                <a href="#simulator" class="hover:text-indigo-400 transition">Live ML Demosu</a>
                <a href="#projects" class="hover:text-indigo-400 transition">Projeler</a>
                <a href="#skills" class="hover:text-indigo-400 transition">Yetenekler</a>
                <a href="#timeline" class="hover:text-indigo-400 transition">Yolculuk</a>
            </div>
            <a href="https://github.com/cdoruk248-cmyk" target="_blank" class="px-4 py-2 bg-indigo-600 hover:bg-indigo-500 text-white rounded-lg text-xs font-semibold tracking-wide transition shadow-lg shadow-indigo-600/30">
                GitHub Profil
            </a>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="max-w-6xl mx-auto px-6 pt-32 pb-20">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
            <div class="lg:col-span-7">
                <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-indigo-500/10 border border-indigo-500/20 text-indigo-400 text-xs font-mono mb-6">
                    <span class="w-2 h-2 rounded-full bg-indigo-400 animate-ping"></span>
                    İstatistik & MIS | Machine Learning Practitioner
                </div>
                <h1 class="text-4xl sm:text-6xl font-extrabold tracking-tight text-white mb-6 leading-tight">
                    Veriden Anlam, <br>
                    <span class="bg-gradient-to-r from-indigo-400 via-cyan-400 to-emerald-400 bg-clip-text text-transparent">Modelden Gelecek</span> Üretiyorum.
                </h1>
                <p class="text-slate-400 text-lg leading-relaxed mb-8">
                    Dokuz Eylül Üniversitesi İstatistik ve Anadolu Üniversitesi YBS öğrencisiyim. Karmaşık veri setlerini analiz ediyor, makine öğrenmesi algoritmalarıyla kestirimsel modeller kuruyor ve uçtan uca veri çözümleri geliştiriyorum.
                </p>
                <div class="flex flex-wrap gap-4">
                    <a href="#simulator" class="px-6 py-3 bg-indigo-600 hover:bg-indigo-500 text-white font-medium rounded-xl transition flex items-center gap-2 shadow-lg shadow-indigo-600/25">
                        <i class="fas fa-microchip"></i> Live ML Demosunu Dene
                    </a>
                    <a href="https://medium.com/@cdoruk248" target="_blank" class="px-6 py-3 bg-slate-900 hover:bg-slate-800 text-slate-200 border border-slate-800 font-medium rounded-xl transition flex items-center gap-2">
                        <i class="fab fa-medium"></i> Medium Makalelerim
                    </a>
                </div>
            </div>

            <!-- Stats & Quick Card -->
            <div class="lg:col-span-5 grid grid-cols-2 gap-4">
                <div class="glass-card p-6 rounded-2xl">
                    <div class="text-indigo-400 text-3xl font-extrabold font-mono mb-1">%93.4</div>
                    <div class="text-xs text-slate-400 font-medium uppercase tracking-wider">En Yüksek ROC-AUC</div>
                    <div class="text-slate-500 text-xs mt-2">HR Attrition Modeli</div>
                </div>
                <div class="glass-card p-6 rounded-2xl">
                    <div class="text-cyan-400 text-3xl font-extrabold font-mono mb-1">2+</div>
                    <div class="text-xs text-slate-400 font-medium uppercase tracking-wider">Akademik Disiplin</div>
                    <div class="text-slate-500 text-xs mt-2">İstatistik & YBS</div>
                </div>
                <div class="glass-card p-6 rounded-2xl">
                    <div class="text-rose-400 text-3xl font-extrabold font-mono mb-1">5+</div>
                    <div class="text-xs text-slate-400 font-medium uppercase tracking-wider">Uçtan Uca Proje</div>
                    <div class="text-slate-500 text-xs mt-2">ML, EDA & Time Series</div>
                </div>
                <div class="glass-card p-6 rounded-2xl">
                    <div class="text-purple-400 text-3xl font-extrabold font-mono mb-1">TOG</div>
                    <div class="text-xs text-slate-400 font-medium uppercase tracking-wider">Genel Koordinatör</div>
                    <div class="text-slate-500 text-xs mt-2">Topluluk Liderliği</div>
                </div>
            </div>
        </div>
    </header>

    <!-- LIVE INTERACTIVE MULTI-MODEL SIMULATOR SECTION -->
    <section id="simulator" class="max-w-6xl mx-auto px-6 py-16">
        <div class="glass-card p-8 sm:p-10 rounded-3xl border border-indigo-500/30 relative overflow-hidden">
            <div class="absolute -right-20 -top-20 w-64 h-64 bg-indigo-500/10 rounded-full blur-3xl pointer-events-none"></div>
            
            <div class="flex flex-col md:flex-row md:items-center justify-between mb-8 gap-4">
                <div>
                    <span class="text-xs font-mono text-indigo-400 tracking-wider uppercase font-semibold">İnteraktif Deneyim</span>
                    <h2 class="text-2xl sm:text-3xl font-bold text-white mt-1">📊 Canlı Makine Öğrenmesi Simülatörü</h2>
                    <p class="text-slate-400 text-sm mt-1">
                        Eğitilen modellerin karar mekanizmalarını tarayıcı üzerinde canlı deneyimleyin.
                    </p>
                </div>

                <!-- Model Switcher Tabs -->
                <div class="flex bg-slate-900/80 p-1.5 rounded-2xl border border-slate-800 gap-1 self-start md:self-auto">
                    <button id="hrTabBtn" onclick="switchSimTab('hr')" class="px-4 py-2 rounded-xl bg-indigo-600 text-white font-medium text-xs transition">
                        🏢 İK Ayrılma Riski
                    </button>
                    <button id="telcoTabBtn" onclick="switchSimTab('telco')" class="px-4 py-2 rounded-xl bg-slate-900 text-slate-400 hover:text-white font-medium text-xs transition">
                        📞 Telco Müşteri Terki
                    </button>
                </div>
            </div>

            <!-- HR SIMULATOR CONTAINER -->
            <div id="hrSimContainer" class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <!-- Controls -->
                <div class="lg:col-span-7 space-y-6">
                    <div>
                        <div class="flex justify-between text-sm font-medium text-slate-300 mb-2">
                            <span>İş Tatmini (Job Satisfaction)</span>
                            <span id="satVal" class="text-indigo-400 font-mono">3 / 4</span>
                        </div>
                        <input type="range" id="satSlider" min="1" max="4" value="3" class="w-full h-2 bg-slate-800 rounded-lg appearance-none cursor-pointer accent-indigo-500">
                    </div>

                    <div>
                        <div class="flex justify-between text-sm font-medium text-slate-300 mb-2">
                            <span>İş - Yaşam Dengesi (Work-Life Balance)</span>
                            <span id="wlbVal" class="text-indigo-400 font-mono">2 / 4</span>
                        </div>
                        <input type="range" id="wlbSlider" min="1" max="4" value="2" class="w-full h-2 bg-slate-800 rounded-lg appearance-none cursor-pointer accent-indigo-500">
                    </div>

                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <label class="block text-sm font-medium text-slate-300 mb-2">Fazla Mesai Var mı?</label>
                            <select id="otSelect" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-2.5 text-sm text-slate-200 focus:outline-none focus:border-indigo-500">
                                <option value="yes">Evet (Düzenli OverTime)</option>
                                <option value="no" selected>Hayır</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-slate-300 mb-2">Şirketteki Yıl</label>
                            <input type="number" id="yearsInput" value="2" min="0" max="20" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-4 py-2.5 text-sm text-slate-200 focus:outline-none focus:border-indigo-500 font-mono">
                        </div>
                    </div>
                </div>

                <!-- Result Box -->
                <div class="lg:col-span-5 bg-slate-900/90 border border-slate-800 p-6 rounded-2xl text-center flex flex-col justify-center items-center">
                    <div class="text-xs uppercase tracking-widest text-slate-400 mb-2">Tahmini Ayrılma Riski</div>
                    <div id="riskScore" class="text-5xl font-black font-mono text-emerald-400 my-2">%18.5</div>
                    <div id="riskBadge" class="inline-block px-3 py-1 rounded-full text-xs font-semibold bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 mb-4">Düşük Risk</div>
                    <p id="riskDesc" class="text-xs text-slate-400 leading-relaxed">
                        Çalışanın iş-yaşam dengesi makul seviyede. Ayrılma olasılığı düşük görünmektedir.
                    </p>
                </div>
            </div>

            <!-- TELCO CHURN SIMULATOR CONTAINER -->
            <div id="telcoSimContainer" class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center hidden">
                <!-- Controls -->
                <div class="lg:col-span-7 space-y-4">
                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <div class="flex justify-between text-xs font-medium text-slate-300 mb-1">
                                <span>Müşteri Kalma Süresi (Ay)</span>
                                <span id="telcoTenureVal" class="text-indigo-400 font-mono">12 Ay</span>
                            </div>
                            <input type="range" id="telcoTenureSlider" min="1" max="72" value="12" class="w-full h-2 bg-slate-800 rounded-lg appearance-none cursor-pointer accent-indigo-500">
                        </div>
                        <div>
                            <label class="block text-xs font-medium text-slate-300 mb-1">Sözleşme Tipi (Kritik!)</label>
                            <select id="telcoContractSelect" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-3 py-1.5 text-xs text-slate-200 focus:outline-none focus:border-indigo-500">
                                <option value="Month-to-month" selected>Month-to-month</option>
                                <option value="One year">One year</option>
                                <option value="Two year">Two year</option>
                            </select>
                        </div>
                    </div>

                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <label class="block text-xs font-medium text-slate-300 mb-1">Aylık Ödeme ($)</label>
                            <input type="number" id="telcoMonthlyInput" value="65.00" step="5" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-3 py-1.5 text-xs text-slate-200 focus:outline-none focus:border-indigo-500 font-mono">
                        </div>
                        <div>
                            <label class="block text-xs font-medium text-slate-300 mb-1">İnternet Servisi</label>
                            <select id="telcoInternetSelect" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-3 py-1.5 text-xs text-slate-200 focus:outline-none focus:border-indigo-500">
                                <option value="DSL" selected>DSL</option>
                                <option value="Fiber optic">Fiber optic</option>
                                <option value="No">No</option>
                            </select>
                        </div>
                    </div>

                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <label class="block text-xs font-medium text-slate-300 mb-1">Bakmakla Yükümlü Kişi Var mı?</label>
                            <select id="telcoDependentsSelect" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-3 py-1.5 text-xs text-slate-200 focus:outline-none focus:border-indigo-500">
                                <option value="Yes">Evet</option>
                                <option value="No" selected>Hayır</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-xs font-medium text-slate-300 mb-1">Partner Var mı?</label>
                            <select id="telcoPartnerSelect" class="w-full bg-slate-900 border border-slate-700 rounded-xl px-3 py-1.5 text-xs text-slate-200 focus:outline-none focus:border-indigo-500">
                                <option value="Yes">Evet</option>
                                <option value="No" selected>Hayır</option>
                            </select>
                        </div>
                    </div>
                </div>

                <!-- Result Box -->
                <div class="lg:col-span-5 bg-slate-900/90 border border-slate-800 p-6 rounded-2xl text-center flex flex-col justify-center items-center">
                    <div class="text-xs uppercase tracking-widest text-slate-400 mb-2">Tahmini Churn (Terk) Riski</div>
                    <div id="telcoRiskScore" class="text-5xl font-black font-mono text-amber-400 my-2">%42.8</div>
                    <div id="telcoRiskBadge" class="inline-block px-3 py-1 rounded-full text-xs font-semibold bg-amber-500/10 text-amber-400 border border-amber-500/20 mb-4">Orta Risk</div>
                    <p id="telcoRiskDesc" class="text-xs text-slate-400 leading-relaxed">
                        Aylık sözleşme ve kısa abonelik süresi müşterinin rakip firmaya geçme olasılığını yükseltmektedir.
                    </p>
                </div>
            </div>

        </div>
    </section>

    <!-- PROJECTS SECTION WITH FILTER -->
    <section id="projects" class="max-w-6xl mx-auto px-6 py-16">
        <div class="flex flex-col md:flex-row md:items-end justify-between mb-10 gap-4">
            <div>
                <span class="text-xs font-mono text-indigo-400 tracking-wider uppercase font-semibold">Portfolyo</span>
                <h2 class="text-3xl font-bold text-white mt-1">Öne Çıkan Çalışmalarım</h2>
            </div>
            
            <!-- Filter Buttons -->
            <div class="flex flex-wrap gap-2 text-xs font-medium">
                <button onclick="filterProjects('all')" class="project-filter-btn px-4 py-2 rounded-xl bg-indigo-600 text-white transition" data-filter="all">Tümü</button>
                <button onclick="filterProjects('ml')" class="project-filter-btn px-4 py-2 rounded-xl bg-slate-900 text-slate-400 hover:text-white transition" data-filter="ml">Makine Öğrenmesi</button>
                <button onclick="filterProjects('eda')" class="project-filter-btn px-4 py-2 rounded-xl bg-slate-900 text-slate-400 hover:text-white transition" data-filter="eda">Veri Analizi (EDA)</button>
                <button onclick="filterProjects('llm')" class="project-filter-btn px-4 py-2 rounded-xl bg-slate-900 text-slate-400 hover:text-white transition" data-filter="llm">Yapay Zeka & RAG</button>
            </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            
            <!-- Project Card: COVID-19 Turkey Analytics Hub -->
            <div class="project-card glass-card p-8 rounded-3xl flex flex-col justify-between transition group border border-slate-800 hover:border-rose-500/50" data-category="ml">
                <div>
                    <div class="flex justify-between items-start mb-4">
                        <span class="text-xs font-mono text-rose-400 bg-rose-500/10 px-3 py-1 rounded-full border border-rose-500/20">Time Series & ML / Healthcare</span>
                        <div class="flex gap-3 text-slate-400 text-lg">
                            <a href="https://github.com/cdoruk248-cmyk/covid19-turkey-analytics" target="_blank" rel="noopener noreferrer" class="hover:text-white transition" title="GitHub Repo"><i class="fab fa-github"></i></a>
                            <a href="https://covid19-turkey-analytics-nco9cy2sjfetgsgwevb5wz.streamlit.app/" target="_blank" rel="noopener noreferrer" class="hover:text-rose-400 transition" title="Live Demo"><i class="fas fa-external-link-alt"></i></a>
                        </div>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-3 group-hover:text-rose-400 transition">COVID-19 Turkey Analytics Hub</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        Türkiye'nin pandemi verileriyle uçtan uca zaman serisi analitiği, Mann-Whitney U testiyle tam kapanma etki ölçümü, Isolation Forest anomali tespiti ve XGBoost ile vefat kestirim modeli (R² = 0.98) içeren interaktif Streamlit platformu.
                    </p>
                </div>
                <div>
                    <div class="flex flex-wrap gap-2 text-xs font-mono text-rose-300 mb-6">
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Streamlit</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">XGBoost</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Isolation Forest</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Hypothesis Testing</span>
                    </div>
                    <a href="https://covid19-turkey-analytics-nco9cy2sjfetgsgwevb5wz.streamlit.app/" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 text-sm font-semibold text-rose-400 hover:text-rose-300">
                        Canlı Uygulamayı İncele <i class="fas fa-arrow-right text-xs"></i>
                    </a>
                </div>
            </div>

            <!-- Project Card: Telco Customer Churn Prediction -->
            <div class="project-card glass-card p-8 rounded-3xl flex flex-col justify-between transition group border border-slate-800 hover:border-amber-500/50" data-category="ml">
                <div>
                    <div class="flex justify-between items-start mb-4">
                        <span class="text-xs font-mono text-amber-400 bg-amber-500/10 px-3 py-1 rounded-full border border-amber-500/20">Classification / Telecommunication</span>
                        <div class="flex gap-3 text-slate-400 text-lg">
                            <a href="https://github.com/cdoruk248-cmyk/Telco-Customer-Churn-Prediction" target="_blank" class="hover:text-white transition"><i class="fab fa-github"></i></a>
                        </div>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-3 group-hover:text-amber-400 transition">Telco Customer Churn Prediction</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        Telekomünikasyon müşterilerinin terk etme eğilimlerini XGBoost ve Lojistik Regresyon algoritmalarıyla tahmin eden, Streamlit arayüzü ile canlıya alınmış kestirimsel model projesi.
                    </p>
                </div>
                <div>
                    <div class="flex flex-wrap gap-2 text-xs font-mono text-amber-300 mb-6">
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">XGBoost</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Streamlit</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Churn Analysis</span>
                    </div>
                    <a href="https://github.com/cdoruk248-cmyk/Telco-Customer-Churn-Prediction" target="_blank" class="inline-flex items-center gap-2 text-sm font-semibold text-amber-400 hover:text-amber-300">
                        Repoyu İncele <i class="fas fa-arrow-right text-xs"></i>
                    </a>
                </div>
            </div>

            <!-- Project Card 1 -->
            <div class="project-card glass-card p-8 rounded-3xl flex flex-col justify-between transition group" data-category="ml">
                <div>
                    <div class="flex justify-between items-start mb-4">
                        <span class="text-xs font-mono text-indigo-400 bg-indigo-500/10 px-3 py-1 rounded-full border border-indigo-500/20">Machine Learning / HR</span>
                        <div class="flex gap-3 text-slate-400 text-lg">
                            <a href="https://github.com/cdoruk248-cmyk/HR-Analytics-Employee-Attrition-Prediction" target="_blank" class="hover:text-white transition"><i class="fab fa-github"></i></a>
                            <a href="https://medium.com/@cdoruk248" target="_blank" class="hover:text-emerald-400 transition"><i class="fab fa-medium"></i></a>
                        </div>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-3 group-hover:text-indigo-400 transition">HR Analytics Attrition Prediction</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        IBM HR veri seti üzerinde SMOTE ile sınıf dengesizliği çözülmüş, Random Forest & Lojistik Regresyon modelleri ile %93.4 ROC-AUC skoru elde edilmiş uçtan uca risk tahmin boru hattı.
                    </p>
                </div>
                <div>
                    <div class="flex flex-wrap gap-2 text-xs font-mono text-indigo-300 mb-6">
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Python</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">SMOTE</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Random Forest</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Feature Importances</span>
                    </div>
                    <a href="https://github.com/cdoruk248-cmyk/HR-Analytics-Employee-Attrition-Prediction" target="_blank" class="inline-flex items-center gap-2 text-sm font-semibold text-indigo-400 hover:text-indigo-300">
                        Repoyu İncele <i class="fas fa-arrow-right text-xs"></i>
                    </a>
                </div>
            </div>

            <!-- Project Card 2 -->
            <div class="project-card glass-card p-8 rounded-3xl flex flex-col justify-between transition group" data-category="ml">
                <div>
                    <div class="flex justify-between items-start mb-4">
                        <span class="text-xs font-mono text-cyan-400 bg-cyan-500/10 px-3 py-1 rounded-full border border-cyan-500/20">Classification / Healthcare</span>
                        <div class="flex gap-3 text-slate-400 text-lg">
                            <a href="https://github.com/cdoruk248-cmyk/hastalik-riski-siniflandirma-knn-svm" target="_blank" class="hover:text-white transition"><i class="fab fa-github"></i></a>
                            <a href="https://medium.com/@cdoruk248" target="_blank" class="hover:text-emerald-400 transition"><i class="fab fa-medium"></i></a>
                        </div>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-3 group-hover:text-cyan-400 transition">Hastalık Riski Sınıflandırması (KNN vs SVM)</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        Biyometrik parametrelerden hastalık riskini kestiren model karşılaştırması. SVM (RBF Kernel) %94.49 ROC-AUC ve yüksek Recall oranıyla klinik teşhiste en güvenilir model seçilmiştir.
                    </p>
                </div>
                <div>
                    <div class="flex flex-wrap gap-2 text-xs font-mono text-cyan-300 mb-6">
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">KNN</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">SVM</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">StandardScaler</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">GridSearchCV</span>
                    </div>
                    <a href="https://github.com/cdoruk248-cmyk/hastalik-riski-siniflandirma-knn-svm" target="_blank" class="inline-flex items-center gap-2 text-sm font-semibold text-cyan-400 hover:text-cyan-300">
                        Repoyu İncele <i class="fas fa-arrow-right text-xs"></i>
                    </a>
                </div>
            </div>

            <!-- Project Card 3 -->
            <div class="project-card glass-card p-8 rounded-3xl flex flex-col justify-between transition group" data-category="eda">
                <div>
                    <div class="flex justify-between items-start mb-4">
                        <span class="text-xs font-mono text-emerald-400 bg-emerald-500/10 px-3 py-1 rounded-full border border-emerald-500/20">E-Commerce / Business EDA</span>
                        <div class="flex gap-3 text-slate-400 text-lg">
                            <a href="https://github.com/cdoruk248-cmyk/veri-bilimi-final-odevi" target="_blank" class="hover:text-white transition"><i class="fab fa-github"></i></a>
                        </div>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-3 group-hover:text-emerald-400 transition">E-Ticaret Veri Analitiği & İş Mimarisi</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        Müşteri segmentasyonu, sepet ortalaması (AOV), coğrafi büyüme potansiyelleri ve kategori ciro dalgalanmalarının görselleştirildiği detaylı keşifçi veri analizi.
                    </p>
                </div>
                <div>
                    <div class="flex flex-wrap gap-2 text-xs font-mono text-emerald-300 mb-6">
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Pandas</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Seaborn</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Data Viz</span>
                    </div>
                    <a href="https://github.com/cdoruk248-cmyk/veri-bilimi-final-odevi" target="_blank" class="inline-flex items-center gap-2 text-sm font-semibold text-emerald-400 hover:text-emerald-300">
                        Repoyu İncele <i class="fas fa-arrow-right text-xs"></i>
                    </a>
                </div>
            </div>

            <!-- Project Card 4 -->
            <div class="project-card glass-card p-8 rounded-3xl flex flex-col justify-between transition group" data-category="llm">
                <div>
                    <div class="flex justify-between items-start mb-4">
                        <span class="text-xs font-mono text-purple-400 bg-purple-500/10 px-3 py-1 rounded-full border border-purple-500/20">GenAI / Local LLM</span>
                        <div class="flex gap-3 text-slate-400 text-lg">
                            <a href="https://github.com/cdoruk248-cmyk/linkedin-bot" target="_blank" class="hover:text-white transition"><i class="fab fa-github"></i></a>
                        </div>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-3 group-hover:text-purple-400 transition">LinkedIn Profil Analiz Botu (Local LLM)</h3>
                    <p class="text-slate-400 text-sm leading-relaxed mb-6">
                        Tamamen yerel cihazda çalışan Ollama & Qwen 2.5 mimarisiyle LinkedIn profillerini hedef pozisyona göre analiz edip İK tavsiyeleri üreten Streamlit uygulaması.
                    </p>
                </div>
                <div>
                    <div class="flex flex-wrap gap-2 text-xs font-mono text-purple-300 mb-6">
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Streamlit</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Ollama</span>
                        <span class="bg-slate-900 border border-slate-800 px-3 py-1 rounded-lg">Qwen 2.5</span>
                    </div>
                    <a href="https://github.com/cdoruk248-cmyk/linkedin-bot" target="_blank" class="inline-flex items-center gap-2 text-sm font-semibold text-purple-400 hover:text-purple-300">
                        Repoyu İncele <i class="fas fa-arrow-right text-xs"></i>
                    </a>
                </div>
            </div>

        </div>
    </section>

    <!-- SKILLS RADAR CHART SECTION -->
    <section id="skills" class="max-w-6xl mx-auto px-6 py-16">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
            <div class="lg:col-span-5">
                <span class="text-xs font-mono text-indigo-400 tracking-wider uppercase font-semibold">Yetkinlik Mimarisi</span>
                <h2 class="text-3xl font-bold text-white mt-1 mb-4">Teori ve Uygulamanın Kesişimi</h2>
                <p class="text-slate-400 text-sm leading-relaxed mb-6">
                    İstatistiksel modelleme temellerini Yönetim Bilişim Sistemleri'nin iş bakış açısıyla harmanlıyorum.
                </p>
                
                <div class="space-y-4 text-sm">
                    <div class="flex items-center gap-3">
                        <i class="fas fa-check-circle text-indigo-400"></i>
                        <span class="text-slate-300">Python, SQL & R ile Gelişmiş Veri Manipülasyonu</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <i class="fas fa-check-circle text-indigo-400"></i>
                        <span class="text-slate-300">Makine Öğrenmesi (Scikit-Learn, Hyperparameter Tuning)</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <i class="fas fa-check-circle text-indigo-400"></i>
                        <span class="text-slate-300">İstatistiksel Hipotez Testleri ve Olasılık Modelleme</span>
                    </div>
                    <div class="flex items-center gap-3">
                        <i class="fas fa-check-circle text-indigo-400"></i>
                        <span class="text-slate-300">Yerel LLM Entegrasyonları & RAG Mimarileri</span>
                    </div>
                </div>
            </div>

            <!-- Chart -->
            <div class="lg:col-span-7 glass-card p-6 rounded-3xl">
                <canvas id="skillsChart" class="w-full max-h-80"></canvas>
            </div>
        </div>
    </section>

    <!-- TIMELINE / JOURNEY SECTION -->
    <section id="timeline" class="max-w-6xl mx-auto px-6 py-16">
        <div class="text-center max-w-2xl mx-auto mb-12">
            <span class="text-xs font-mono text-indigo-400 tracking-wider uppercase font-semibold">Gelişim Süreci</span>
            <h2 class="text-3xl font-bold text-white mt-1">Akademik & Liderlik Yolculuğu</h2>
        </div>

        <div class="max-w-3xl mx-auto relative border-l-2 border-slate-800 pl-8 space-y-10">
            
            <!-- Timeline Item 1 -->
            <div class="relative group">
                <div class="absolute -left-[41px] top-0 w-5 h-5 rounded-full bg-indigo-600 border-4 border-slate-950 group-hover:scale-125 transition"></div>
                <span class="text-xs font-mono text-indigo-400">2026 - Halen</span>
                <h3 class="text-lg font-bold text-white mt-1">Genel Koordinatör @ DEÜ Toplum Gönüllüleri Topluluğu</h3>
                <p class="text-slate-400 text-sm mt-2 leading-relaxed">
                    Öğrenci topluluğunda genel yönetim, kaynak geliştirme ve sosyal sorumluluk projelerinin uçtan uca organizasyon liderliği.
                </p>
            </div>

            <!-- Timeline Item 2 -->
            <div class="relative group">
                <div class="absolute -left-[41px] top-0 w-5 h-5 rounded-full bg-cyan-500 border-4 border-slate-950 group-hover:scale-125 transition"></div>
                <span class="text-xs font-mono text-cyan-400">2025 - 2026</span>
                <h3 class="text-lg font-bold text-white mt-1">Türkiye Yapay Zeka Akademisi & HSD Bootcamp</h3>
                <p class="text-slate-400 text-sm mt-2 leading-relaxed">
                    Veri Bilimi ve Makine Öğrenmesi alanında bitirme projeleri, SMOTE, sınıflandırma modelleri ve teknik Medium yayınlarının hazırlanması.
                </p>
            </div>

            <!-- Timeline Item 3 -->
            <div class="relative group">
                <div class="absolute -left-[41px] top-0 w-5 h-5 rounded-full bg-emerald-500 border-4 border-slate-950 group-hover:scale-125 transition"></div>
                <span class="text-xs font-mono text-emerald-400">Lisans Eğitimi</span>
                <h3 class="text-lg font-bold text-white mt-1">Dokuz Eylül Üniv. (İstatistik) & Anadolu Üniv. (YBS)</h3>
                <p class="text-slate-400 text-sm mt-2 leading-relaxed">
                    Matematiksel İstatistik, Regresyon Analizi, Yöneylem Araştırması ve Yönetim Bilişim Sistemleri eğitimi.
                </p>
            </div>

        </div>
    </section>

    <!-- FOOTER -->
    <footer class="glass-card border-t border-slate-800/80 py-12 mt-20">
        <div class="max-w-6xl mx-auto px-6 text-center">
            <h3 class="text-2xl font-bold text-white mb-2">Birlikte Veri Odaklı Projeler Geliştirelim</h3>
            <p class="text-slate-400 text-sm mb-6 max-w-md mx-auto">
                Sorularınız, proje iş birlikleri veya veri bilimi sohbetleri için doğrudan ulaşabilirsiniz.
            </p>
            
            <div class="flex justify-center gap-6 text-xl mb-8">
                <a href="https://github.com/cdoruk248-cmyk" target="_blank" class="text-slate-400 hover:text-white transition"><i class="fab fa-github"></i></a>
                <a href="https://www.linkedin.com/in/dorukcelik" target="_blank" class="text-slate-400 hover:text-blue-400 transition"><i class="fab fa-linkedin"></i></a>
                <a href="https://medium.com/@cdoruk248" target="_blank" class="text-slate-400 hover:text-emerald-400 transition"><i class="fab fa-medium"></i></a>
            </div>

            <div class="text-xs text-slate-500 font-mono">
                © 2026 Doruk Çelik. Built with HTML, Tailwind CSS & Chart.js.
            </div>
        </div>
    </footer>

    <!-- INTERACTIVE JAVASCRIPT LOGIC -->
    <script>
        // Tab Switcher Function
        function switchSimTab(tab) {
            const hrContainer = document.getElementById('hrSimContainer');
            const telcoContainer = document.getElementById('telcoSimContainer');
            const hrBtn = document.getElementById('hrTabBtn');
            const telcoBtn = document.getElementById('telcoTabBtn');

            if (tab === 'hr') {
                hrContainer.classList.remove('hidden');
                telcoContainer.classList.add('hidden');
                hrBtn.className = "px-4 py-2 rounded-xl bg-indigo-600 text-white font-medium text-xs transition";
                telcoBtn.className = "px-4 py-2 rounded-xl bg-slate-900 text-slate-400 hover:text-white font-medium text-xs transition";
            } else {
                hrContainer.classList.add('hidden');
                telcoContainer.classList.remove('hidden');
                telcoBtn.className = "px-4 py-2 rounded-xl bg-indigo-600 text-white font-medium text-xs transition";
                hrBtn.className = "px-4 py-2 rounded-xl bg-slate-900 text-slate-400 hover:text-white font-medium text-xs transition";
                updateTelcoSimulator();
            }
        }

        // 1. HR Simulator Calculation
        function updateSimulator() {
            const sat = parseInt(document.getElementById('satSlider').value);
            const wlb = parseInt(document.getElementById('wlbSlider').value);
            const ot = document.getElementById('otSelect').value;
            const years = parseInt(document.getElementById('yearsInput').value) || 0;

            document.getElementById('satVal').innerText = sat + " / 4";
            document.getElementById('wlbVal').innerText = wlb + " / 4";

            let baseRisk = 30;
            baseRisk -= (sat * 6);
            baseRisk -= (wlb * 5);
            if (ot === 'yes') baseRisk += 32;
            if (years <= 2) baseRisk += 14;

            baseRisk = Math.max(4, Math.min(94, baseRisk));

            const riskEl = document.getElementById('riskScore');
            const badgeEl = document.getElementById('riskBadge');
            const descEl = document.getElementById('riskDesc');

            riskEl.innerText = "%" + baseRisk.toFixed(1);

            if (baseRisk > 50) {
                riskEl.className = "text-5xl font-black font-mono text-rose-500 my-2";
                badgeEl.className = "inline-block px-3 py-1 rounded-full text-xs font-semibold bg-rose-500/10 text-rose-400 border border-rose-500/20 mb-4";
                badgeEl.innerText = "Yüksek Risk";
                descEl.innerText = "Düşük tatmin ve fazla mesai yükü çalışanın ayrılma olasılığını kritik seviyeye çıkarmaktadır.";
            } else if (baseRisk > 25) {
                riskEl.className = "text-5xl font-black font-mono text-amber-400 my-2";
                badgeEl.className = "inline-block px-3 py-1 rounded-full text-xs font-semibold bg-amber-500/10 text-amber-400 border border-amber-500/20 mb-4";
                badgeEl.innerText = "Orta Risk";
                descEl.innerText = "Çalışan stabil görünmekle birlikte izlenmesi ve iş yükünün dengelenmesi önerilir.";
            } else {
                riskEl.className = "text-5xl font-black font-mono text-emerald-400 my-2";
                badgeEl.className = "inline-block px-3 py-1 rounded-full text-xs font-semibold bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 mb-4";
                badgeEl.innerText = "Düşük Risk";
                descEl.innerText = "Çalışanın tutundurma faktörleri yüksek, istifa riski oldukça düşüktür.";
            }
        }

        // 2. Telco Churn Simulator Calculation
        function updateTelcoSimulator() {
            const tenure = parseInt(document.getElementById('telcoTenureSlider').value) || 1;
            const contract = document.getElementById('telcoContractSelect').value;
            const monthly = parseFloat(document.getElementById('telcoMonthlyInput').value) || 65;
            const internet = document.getElementById('telcoInternetSelect').value;

            document.getElementById('telcoTenureVal').innerText = tenure + " Ay";

            let baseRisk = 25;
            if (contract === 'Month-to-month') baseRisk += 28;
            if (contract === 'Two year') baseRisk -= 22;
            if (internet === 'Fiber optic') baseRisk += 14;
            if (tenure <= 12) baseRisk += 16;
            if (monthly > 70) baseRisk += 10;

            baseRisk = Math.max(3, Math.min(96, baseRisk));

            const riskEl = document.getElementById('telcoRiskScore');
            const badgeEl = document.getElementById('telcoRiskBadge');
            const descEl = document.getElementById('telcoRiskDesc');

            riskEl.innerText = "%" + baseRisk.toFixed(1);

            if (baseRisk > 50) {
                riskEl.className = "text-5xl font-black font-mono text-rose-500 my-2";
                badgeEl.className = "inline-block px-3 py-1 rounded-full text-xs font-semibold bg-rose-500/10 text-rose-400 border border-rose-500/20 mb-4";
                badgeEl.innerText = "Yüksek Churn Riski";
                descEl.innerText = "Aylık sözleşme yapısı ve yüksek tarife ücreti müşterinin abonelik iptali riskini ciddi seviyede artırıyor.";
            } else if (baseRisk > 25) {
                riskEl.className = "text-5xl font-black font-mono text-amber-400 my-2";
                badgeEl.className = "inline-block px-3 py-1 rounded-full text-xs font-semibold bg-amber-500/10 text-amber-400 border border-amber-500/20 mb-4";
                badgeEl.innerText = "Orta Churn Riski";
                descEl.innerText = "Müşteri tutundurma kampanyaları ve uzun süreli sözleşme indirimleri önerilebilir.";
            } else {
                riskEl.className = "text-5xl font-black font-mono text-emerald-400 my-2";
                badgeEl.className = "inline-block px-3 py-1 rounded-full text-xs font-semibold bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 mb-4";
                badgeEl.innerText = "Düşük Churn Riski";
                descEl.innerText = "Müşterinin bağlılığı yüksek, uzun vadeli abonelik yapısı sebebiyle terk etme olasılığı düşüktür.";
            }
        }

        // Event Listeners for HR
        document.getElementById('satSlider').addEventListener('input', updateSimulator);
        document.getElementById('wlbSlider').addEventListener('input', updateSimulator);
        document.getElementById('otSelect').addEventListener('change', updateSimulator);
        document.getElementById('yearsInput').addEventListener('input', updateSimulator);

        // Event Listeners for Telco
        document.getElementById('telcoTenureSlider').addEventListener('input', updateTelcoSimulator);
        document.getElementById('telcoContractSelect').addEventListener('change', updateTelcoSimulator);
        document.getElementById('telcoMonthlyInput').addEventListener('input', updateTelcoSimulator);
        document.getElementById('telcoInternetSelect').addEventListener('change', updateTelcoSimulator);
        document.getElementById('telcoDependentsSelect').addEventListener('change', updateTelcoSimulator);
        document.getElementById('telcoPartnerSelect').addEventListener('change', updateTelcoSimulator);

        // 3. Project Filter Logic
        function filterProjects(cat) {
            const cards = document.querySelectorAll('.project-card');
            const btns = document.querySelectorAll('.project-filter-btn');

            btns.forEach(btn => {
                if (btn.getAttribute('data-filter') === cat) {
                    btn.className = "project-filter-btn px-4 py-2 rounded-xl bg-indigo-600 text-white transition";
                } else {
                    btn.className = "project-filter-btn px-4 py-2 rounded-xl bg-slate-900 text-slate-400 hover:text-white transition";
                }
            });

            cards.forEach(card => {
                if (cat === 'all' || card.getAttribute('data-category') === cat) {
                    card.style.display = 'flex';
                } else {
                    card.style.display = 'none';
                }
            });
        }

        // 4. Chart.js Skills Radar
        window.addEventListener('DOMContentLoaded', () => {
            updateSimulator();
            
            const ctx = document.getElementById('skillsChart').getContext('2d');
            new Chart(ctx, {
                type: 'radar',
                data: {
                    labels: ['Matematiksel İstatistik', 'Makine Öğrenmesi', 'Veri Analizi (EDA)', 'Python & Kütüphaneler', 'SQL & Veri Tabanı', 'LLM & RAG'],
                    datasets: [{
                        label: 'Yetenek Yetkinlik Oranı (%)',
                        data: [90, 88, 92, 95, 80, 75],
                        backgroundColor: 'rgba(99, 102, 241, 0.25)',
                        borderColor: 'rgba(99, 102, 241, 1)',
                        pointBackgroundColor: '#38bdf8',
                        pointBorderColor: '#fff',
                        pointHoverBackgroundColor: '#fff',
                        pointHoverBorderColor: '#38bdf8'
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: {
                        r: {
                            angleLines: { color: 'rgba(255, 255, 255, 0.1)' },
                            grid: { color: 'rgba(255, 255, 255, 0.1)' },
                            pointLabels: { color: '#94a3b8', font: { size: 11 } },
                            ticks: { display: false, max: 100 }
                        }
                    },
                    plugins: {
                        legend: { display: false }
                    }
                }
            });
        });
    </script>
</body>
</html>
