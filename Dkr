```html
<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Class 8 WBBSE Physical Science (35 Marks) — Final Exam Portal</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Noto+Sans+Devanagari:wght@400;500;600;700;800&display=swap" rel="stylesheet" />
  <style>
    :root {
      --dusk-blue: #4B6584;
      --dusk-dark: #0B1120;
      --dusk-card: #131D31;
      --dusk-surface: #1B2842;
      --accent-gold: #F59E0B;
      --accent-cyan: #38BDF8;
      --accent-emerald: #10B981;
    }
    * {
      box-sizing: border-box;
    }
    body {
      font-family: 'Inter', 'Noto Sans Devanagari', sans-serif;
      background: radial-gradient(circle at 15% 10%, #1E2E4A 0%, #0B1120 55%, #070B14 100%);
      color: #F1F5F9;
      min-height: 100vh;
      overflow-x: hidden;
    }
    .dusk-card {
      background: linear-gradient(145deg, rgba(27, 40, 66, 0.92), rgba(15, 23, 42, 0.96));
      border: 1px solid rgba(75, 101, 132, 0.48);
      box-shadow: 0 10px 28px -8px rgba(0, 0, 0, 0.55);
    }
    .dusk-panel {
      background: rgba(11, 17, 32, 0.85);
      border: 1px solid rgba(75, 101, 132, 0.4);
    }
    .dusk-pill {
      background: linear-gradient(135deg, #4B6584, #334760);
      border: 1px solid rgba(148, 163, 184, 0.35);
    }
    .no-scrollbar::-webkit-scrollbar {
      display: none;
    }
    .no-scrollbar {
      -ms-overflow-style: none;
      scrollbar-width: none;
    }
    @keyframes pulseMic {
      0%, 100% { transform: scale(1); box-shadow: 0 0 0 0 rgba(239, 68, 68, 0.7); }
      50% { transform: scale(1.04); box-shadow: 0 0 0 8px rgba(239, 68, 68, 0); }
    }
    .mic-recording {
      animation: pulseMic 1.2s infinite;
      background: #DC2626 !important;
      color: #FFFFFF !important;
      border-color: #FCA5A5 !important;
    }
  </style>
</head>
<body class="antialiased selection:bg-cyan-500 selection:text-slate-950">

  <!-- Toast Notification Box (No alert/confirm used anywhere) -->
  <div id="toast-box" class="fixed bottom-4 right-4 z-50 hidden max-w-sm px-4 py-3 rounded-2xl border text-xs sm:text-sm font-bold shadow-2xl transition-all duration-200"></div>

  <!-- ===================================================================== -->
  <!-- MANDATORY STARTUP LOGIN & PASSWORD GATE MODAL (OPENS ON APP LOAD)     -->
  <!-- ===================================================================== -->
  <div id="authGateModal" class="fixed inset-0 z-50 bg-slate-950/95 backdrop-blur-md flex items-center justify-center p-3 sm:p-5 overflow-y-auto">
    <div class="dusk-card w-full max-w-lg rounded-3xl p-5 sm:p-7 space-y-4 border-2 border-cyan-400/60 shadow-2xl my-auto">
      <!-- Top Permanently Locked Credits inside Login Gate -->
      <div class="p-3.5 rounded-2xl bg-slate-950/90 border border-amber-400/50 space-y-1.5 text-xs">
        <div class="flex flex-wrap items-center justify-between gap-1">
          <span class="text-slate-400 font-semibold">🔒 Web Created by:</span>
          <span class="text-amber-300 font-extrabold">Dipak Kumar Rajak (दीपक कुमार राजक)</span>
        </div>
        <div class="flex flex-wrap items-center justify-between gap-1">
          <span class="text-slate-400 font-semibold">🔒 स्कूल (School):</span>
          <span class="text-cyan-300 font-bold">D.A.V. Higher Secondary School, Asansol</span>
        </div>
        <div class="flex flex-wrap items-center justify-between gap-1">
          <span class="text-slate-400 font-semibold">🔒 विषय शिक्षक (Sir):</span>
          <span class="text-emerald-300 font-extrabold">Sri Pankaj Kumar (श्री पंकज कुमार)</span>
        </div>
      </div>

      <!-- Heading -->
      <div class="text-center space-y-1">
        <span class="px-3 py-1 rounded-full text-[11px] font-extrabold bg-cyan-500/20 text-cyan-300 border border-cyan-400/40">
          🔐 STUDENT LOGIN & LEVEL SAVE VAULT (35 MARKS EXAM)
        </span>
        <h2 class="text-lg sm:text-2xl font-extrabold text-white pt-1">
          अपना नाम, सेक्शन, रोल नं. और पासवर्ड डालें
        </h2>
        <p class="text-xs text-slate-300">
          नया पासवर्ड बनाएँ या पुराना पासवर्ड डालें — आपके सभी <strong>17 लेवल, 35-अंक अभ्यास और मॉक टेस्ट</strong> सुरक्षित सेव रहेंगे!
        </p>
      </div>

      <!-- Saved Accounts Quick-Select Chips -->
      <div id="saved-accounts-box" class="hidden p-3 rounded-2xl bg-slate-950/80 border border-slate-700 space-y-2">
        <div class="text-[11px] font-extrabold text-cyan-300">⚡ इस डिवाइस पर सेव किए गए छात्र (1-टैप में चुनें):</div>
        <div id="saved-accounts-chips" class="flex flex-wrap gap-1.5"></div>
      </div>

      <!-- Inline Auth Error / Status Alert -->
      <div id="auth-error-box" class="hidden p-3 rounded-xl bg-rose-950/90 border border-rose-400 text-xs font-bold text-rose-200 space-y-2">
        <div id="auth-error-text"></div>
        <button
          type="button"
          onclick="resetForgottenPassword()"
          class="px-3 py-1 rounded-lg bg-amber-400 text-slate-950 text-[11px] font-extrabold"
        >
          🔄 इस रोल नंबर का नया पासवर्ड सेट करें (Reset Password)
        </button>
      </div>

      <!-- Login / Register Form -->
      <div class="space-y-3">
        <div>
          <label class="block text-xs font-extrabold text-slate-200 mb-1">1. छात्र का नाम (Student Name) *</label>
          <input
            id="auth-student-name"
            type="text"
            placeholder="जैसे: Dipak Kumar Rajak"
            class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-600 text-white text-sm font-bold focus:outline-none focus:border-cyan-400"
          />
        </div>

        <div class="grid grid-cols-2 gap-3">
          <div>
            <label class="block text-xs font-extrabold text-slate-200 mb-1">2. सेक्शन (Section A / B / C) *</label>
            <select
              id="auth-student-sec"
              onchange="checkExistingAccountHint()"
              class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-600 text-white text-sm font-bold focus:outline-none focus:border-cyan-400"
            >
              <option value="A">Section A</option>
              <option value="B">Section B</option>
              <option value="C">Section C</option>
            </select>
          </div>
          <div>
            <label class="block text-xs font-extrabold text-slate-200 mb-1">3. रोल नंबर (Roll No.) *</label>
            <input
              id="auth-student-roll"
              type="text"
              placeholder="जैसे: 01"
              oninput="checkExistingAccountHint()"
              class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-600 text-white text-sm font-bold focus:outline-none focus:border-cyan-400"
            />
          </div>
        </div>

        <div>
          <div class="flex items-center justify-between mb-1">
            <label class="block text-xs font-extrabold text-amber-300">4. पासवर्ड (Password — लेवल सेव रखने के लिए) *</label>
            <span id="auth-account-mode-badge" class="text-[11px] font-extrabold text-emerald-300">✨ नया खाता / लॉगिन</span>
          </div>
          <div class="relative flex items-center">
            <input
              id="auth-student-pass"
              type="password"
              placeholder="अपना पासवर्ड लिखें (कम से कम 3 अक्षर/अंक)..."
              onkeydown="if(event.key==='Enter') handleAuthGateSubmit();"
              class="w-full pl-3.5 pr-12 py-2.5 rounded-xl bg-slate-950 border border-amber-400/60 text-white text-sm font-bold focus:outline-none focus:border-amber-400"
            />
            <button
              type="button"
              onclick="togglePasswordVisibility('auth-student-pass', 'auth-pass-eye')"
              id="auth-pass-eye"
              class="absolute right-2.5 px-2 py-1 rounded-lg bg-slate-800 hover:bg-slate-700 text-xs font-bold text-slate-200"
              title="पासवर्ड देखें/छुपाएँ"
            >
              👁️
            </button>
          </div>
          <p id="auth-pass-helper" class="text-[11px] text-slate-400 mt-1">
            💡 पहली बार लॉगिन करने पर यही आपका पासवर्ड बन जाएगा। अगली बार यही पासवर्ड डालने पर सारे सेव्ड लेवल खुलेंगे।
          </p>
        </div>
      </div>

      <button
        type="button"
        onclick="handleAuthGateSubmit()"
        class="w-full py-3.5 rounded-2xl bg-gradient-to-r from-cyan-400 via-emerald-400 to-amber-400 hover:opacity-95 text-slate-950 font-extrabold text-sm shadow-xl transition"
      >
        🚀 लॉगिन करें एवं मेरे सभी लेवल खोलें (Unlock & Save Levels)
      </button>
    </div>
  </div>

  <!-- Change Password / Edit Student Profile Modal (When Already Logged In) -->
  <div id="profile-modal" class="fixed inset-0 z-50 hidden bg-slate-950/80 backdrop-blur-sm flex items-center justify-center p-4">
    <div class="dusk-card w-full max-w-md rounded-2xl p-5 sm:p-6 space-y-4 border-2 border-cyan-400/50">
      <div class="flex items-center justify-between border-b border-slate-700/70 pb-3">
        <div>
          <span class="px-2.5 py-0.5 rounded-full text-[10px] font-extrabold bg-cyan-500/20 text-cyan-300 border border-cyan-400/40">
            🔑 ACCOUNT & PASSWORD SETTINGS
          </span>
          <h3 class="text-base sm:text-lg font-extrabold text-white mt-1">छात्र प्रोफ़ाइल एवं पासवर्ड अपडेट</h3>
        </div>
        <button onclick="closeProfileModal()" class="w-8 h-8 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-300 font-bold text-sm">✕</button>
      </div>

      <!-- Locked Permanent Information -->
      <div class="p-3 rounded-xl bg-slate-950/90 border border-amber-400/40 space-y-1.5 text-xs">
        <div class="flex items-center justify-between">
          <span class="text-slate-400 font-semibold">🔒 Web Created by:</span>
          <span class="text-amber-300 font-extrabold">Dipak Kumar Rajak (दीपक कुमार राजक)</span>
        </div>
        <div class="flex items-center justify-between">
          <span class="text-slate-400 font-semibold">🔒 स्कूल (School):</span>
          <span class="text-cyan-300 font-bold">D.A.V. Higher Secondary School, Asansol</span>
        </div>
        <div class="flex items-center justify-between">
          <span class="text-slate-400 font-semibold">🔒 विषय शिक्षक (Sir):</span>
          <span class="text-emerald-300 font-extrabold">Sri Pankaj Kumar (श्री पंकज कुमार)</span>
        </div>
      </div>

      <!-- Editable Student Fields -->
      <div class="space-y-3">
        <div>
          <label class="block text-xs font-bold text-slate-300 mb-1">आपका नाम (Student Name):</label>
          <input id="input-student-name" type="text" placeholder="जैसे: Dipak Kumar Rajak" class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-600 text-white text-sm font-bold focus:outline-none focus:border-cyan-400" />
        </div>
        <div class="grid grid-cols-2 gap-3">
          <div>
            <label class="block text-xs font-bold text-slate-300 mb-1">सेक्शन (Section A / B / C):</label>
            <select id="input-student-sec" class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-600 text-white text-sm font-bold focus:outline-none focus:border-cyan-400">
              <option value="A">Section A</option>
              <option value="B">Section B</option>
              <option value="C">Section C</option>
            </select>
          </div>
          <div>
            <label class="block text-xs font-bold text-slate-300 mb-1">रोल नंबर (Roll No.):</label>
            <input id="input-student-roll" type="text" placeholder="01" class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-600 text-white text-sm font-bold focus:outline-none focus:border-cyan-400" />
          </div>
        </div>
        <div>
          <label class="block text-xs font-bold text-amber-300 mb-1">आपका पासवर्ड (Password):</label>
          <div class="relative flex items-center">
            <input id="input-student-pass" type="password" placeholder="नया पासवर्ड..." class="w-full pl-3.5 pr-12 py-2.5 rounded-xl bg-slate-950 border border-amber-400/60 text-white text-sm font-bold focus:outline-none focus:border-amber-400" />
            <button type="button" onclick="togglePasswordVisibility('input-student-pass', 'modal-pass-eye')" id="modal-pass-eye" class="absolute right-2.5 px-2 py-1 rounded-lg bg-slate-800 text-xs font-bold text-slate-200">👁️</button>
          </div>
        </div>
      </div>

      <div class="flex flex-wrap items-center justify-between gap-2 pt-2">
        <button onclick="closeProfileModal(); logoutAndOpenAuthGate();" class="px-3.5 py-2 rounded-xl bg-rose-600 hover:bg-rose-500 text-white text-xs font-extrabold">
          🚪 लॉगआउट / दूसरा छात्र
        </button>
        <div class="flex items-center gap-2">
          <button onclick="closeProfileModal()" class="px-3.5 py-2 rounded-xl bg-slate-800 hover:bg-slate-700 text-slate-300 text-xs font-bold">रद्द करें</button>
          <button onclick="saveStudentProfile()" class="px-4 py-2 rounded-xl bg-cyan-400 hover:bg-cyan-300 text-slate-950 text-xs font-extrabold shadow-lg">💾 सेव करें</button>
        </div>
      </div>
    </div>
  </div>

  <!-- Top Branding & Profile Header -->
  <header class="max-w-6xl mx-auto px-3 sm:px-5 pt-3 pb-2">
    <div class="dusk-card rounded-2xl p-3.5 sm:p-4 border border-[#4B6584]/60 space-y-2.5">
      <!-- Top Locked Credits Ribbon -->
      <div class="flex flex-wrap items-center justify-between gap-2 pb-2.5 border-b border-slate-700/60 text-[11px] sm:text-xs">
        <div class="flex flex-wrap items-center gap-1.5 sm:gap-2">
          <span class="px-2.5 py-1 rounded-full bg-amber-400 text-slate-950 font-extrabold shadow-sm">
            ✨ Web Created by: Dipak Kumar Rajak
          </span>
          <span class="px-2.5 py-1 rounded-full bg-[#1B2842] text-cyan-300 border border-cyan-400/30 font-bold">
            🏫 D.A.V. Higher Secondary School, Asansol
          </span>
          <span class="px-2.5 py-1 rounded-full bg-emerald-950/90 text-emerald-300 border border-emerald-400/40 font-extrabold">
            👨‍🏫 Sir: Sri Pankaj Kumar (श्री पंकज कुमार)
          </span>
        </div>
        <div class="flex items-center gap-1.5">
          <span id="autosave-status-badge" class="px-2.5 py-1 rounded-full bg-emerald-500/20 text-emerald-300 border border-emerald-400/40 font-extrabold">
            💾 सभी लेवल सेव्ड (Auto-Saved)
          </span>
          <span class="px-2.5 py-1 rounded-full bg-rose-950/90 text-rose-200 border border-rose-400/40 font-extrabold">
            📅 Exam: 4 Dec 2026 (35 Marks)
          </span>
        </div>
      </div>

      <!-- Compact Student Bar -->
      <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-2.5">
        <div>
          <h1 class="text-base sm:text-xl font-extrabold text-white tracking-tight flex flex-wrap items-center gap-2">
            <span>Class 8 WBBSE परिवेश और विज्ञान (Physical Science)</span>
            <span class="text-xs px-2 py-0.5 rounded-lg bg-cyan-500/20 text-cyan-300 border border-cyan-400/40 font-bold">10+7+12+6 = 35 अंक</span>
          </h1>
          <p id="student-greeting-line" class="text-xs text-slate-300 mt-0.5">
            👋 छात्र: <strong class="text-amber-300">Dipak Kumar Rajak</strong> • <span class="text-cyan-300 font-bold">Class 8 (Section A • Roll #01)</span> • मार्गदर्शन: <strong class="text-emerald-300">श्री पंकज कुमार सर</strong>
          </p>
        </div>

        <div class="flex flex-wrap items-center gap-1.5 shrink-0">
          <button onclick="openProfileModal()" class="px-3 py-1.5 rounded-xl bg-cyan-400 hover:bg-cyan-300 text-slate-950 text-xs font-extrabold transition shadow-sm">
            🔑 पासवर्ड / प्रोफ़ाइल
          </button>
          <button onclick="logoutAndOpenAuthGate()" class="px-3 py-1.5 rounded-xl bg-slate-800 hover:bg-rose-600 text-slate-200 hover:text-white border border-slate-600 text-xs font-extrabold transition shadow-sm">
            🚪 लॉगआउट / छात्र बदलें
          </button>
          <button onclick="switchTab('quizroom')" class="px-3 py-1.5 rounded-xl bg-amber-400 hover:bg-amber-300 text-slate-950 text-xs font-extrabold transition shadow-sm">
            ⚔️ Quiz Room
          </button>
        </div>
      </div>

      <!-- Live 35-Mark Scoreboard & Level Progress Bar -->
      <div class="grid grid-cols-3 sm:grid-cols-6 gap-1.5 pt-1 text-center">
        <div class="px-2 py-1.5 rounded-xl bg-slate-950/90 border border-cyan-400/30">
          <div class="text-[10px] text-slate-400 font-bold">MCQ (10)</div>
          <div id="hdr-score-mcq" class="text-xs sm:text-sm font-extrabold text-cyan-300">0 / 10</div>
        </div>
        <div class="px-2 py-1.5 rounded-xl bg-slate-950/90 border border-amber-400/30">
          <div class="text-[10px] text-slate-400 font-bold">रिक्त स्थान (7)</div>
          <div id="hdr-score-fill" class="text-xs sm:text-sm font-extrabold text-amber-300">0 / 7</div>
        </div>
        <div class="px-2 py-1.5 rounded-xl bg-slate-950/90 border border-emerald-400/30">
          <div class="text-[10px] text-slate-400 font-bold">लघु उत्तरीय (12)</div>
          <div id="hdr-score-short" class="text-xs sm:text-sm font-extrabold text-emerald-300">0 / 12</div>
        </div>
        <div class="px-2 py-1.5 rounded-xl bg-slate-950/90 border border-purple-400/30">
          <div class="text-[10px] text-slate-400 font-bold">दीर्घ उत्तरीय (6)</div>
          <div id="hdr-score-long" class="text-xs sm:text-sm font-extrabold text-purple-300">0 / 6</div>
        </div>
        <div class="px-2 py-1.5 rounded-xl bg-amber-400/15 border border-amber-400/60">
          <div class="text-[10px] text-amber-200 font-bold">कुल अंक (35)</div>
          <div id="hdr-score-total" class="text-xs sm:text-sm font-extrabold text-amber-300">0 / 35</div>
        </div>
        <div class="px-2 py-1.5 rounded-xl bg-emerald-400/15 border border-emerald-400/60">
          <div class="text-[10px] text-emerald-200 font-bold">लेवल पूरे (17)</div>
          <div id="hdr-score-levels" class="text-xs sm:text-sm font-extrabold text-emerald-300">1 / 17</div>
        </div>
      </div>
    </div>
  </header>

  <!-- Slim Sticky 8-Tab Navigation Bar -->
  <nav class="sticky top-0 z-40 bg-[#0B1120]/95 backdrop-blur-md border-y border-[#4B6584]/50 shadow-lg">
    <div class="max-w-6xl mx-auto px-2 sm:px-5 py-1.5 flex items-center justify-between gap-2">
      <!-- Scrollable 8 Tabs -->
      <div class="flex items-center gap-1.5 overflow-x-auto no-scrollbar py-0.5">
        <button id="tab-btn-roadmap" onclick="switchTab('roadmap')" class="tab-btn shrink-0 px-3 py-1.5 rounded-xl text-xs font-extrabold transition">
          1. 🗺️ 99% रोडमैप & लेवल टीचर
        </button>
        <button id="tab-btn-mock" onclick="switchTab('mock')" class="tab-btn shrink-0 px-3 py-1.5 rounded-xl text-xs font-extrabold transition">
          2. ⏱️ 35-Mark Mock Test
        </button>
        <button id="tab-btn-obj" onclick="switchTab('obj')" class="tab-btn shrink-0 px-3 py-1.5 rounded-xl text-xs font-extrabold transition">
          3. ✅ 10 MCQ & 7 रिक्त स्थान (17)
        </button>
        <button id="tab-btn-subj" onclick="switchTab('subj')" class="tab-btn shrink-0 px-3 py-1.5 rounded-xl text-xs font-extrabold transition">
          4. ✍️ लघु (12) & दीर्घ (6) + 🎤 Voice
        </button>
        <button id="tab-btn-formulas" onclick="switchTab('formulas')" class="tab-btn shrink-0 px-3 py-1.5 rounded-xl text-xs font-extrabold transition">
          5. 📌 फॉर्मूला & 7 मिस्टेक-फिक्सर
        </button>
        <but
