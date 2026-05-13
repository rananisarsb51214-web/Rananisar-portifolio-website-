o# Rana Nisar - Portfolio Website

Welcome to my portfolio website! This is the digital home of Rana Nisar, showcasing my expertise in digital marketing, web development, and content creation.

## About

I'm a passionate technology enthusiast and digital creator dedicated to helping businesses grow their online presence. This portfolio website demonstrates my skills and services.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean and professional design with smooth animations
- **Easy Navigation**: Intuitive navigation with smooth scrolling
- **Service Showcase**: Detailed information about digital marketing, web development, and content creation services
- **Skills Display**: Comprehensive list of technical and creative skills
- **Contact Information**: Easy ways to get in touch

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Responsive Web Design

## How to Use<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nisar AI Studio | Autonomous Empire v7.0</title>

<script src="https://cdn.tailwindcss.com"></script>
<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;900&family=Inter:wght@300;600&display=swap" rel="stylesheet">

<style>
    :root {
        --neon-gold: #fbbf24;
        --glass-bg: rgba(17, 24, 39, 0.7);
    }
    body {
        background: #030712;
        color: #f3f4f6;
        font-family: 'Inter', sans-serif;
        overflow-x: hidden;
    }
    .orbitron { font-family: 'Orbitron', sans-serif; }

    /* Glassmorphism Effect */
    .glass {
        background: var(--glass-bg);
        backdrop-filter: blur(12px);
        border: 1px solid rgba(255, 255, 255, 0.1);
        box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
    }

    /* SLIDESHOW ANIMATION */
    .slide {
        position: absolute;
        inset: 0;
        opacity: 0;
        transition: opacity 1.5s ease-in-out, transform 10s ease-in-out;
        transform: scale(1.1);
    }
    .slide.active {
        opacity: 1;
        transform: scale(1);
    }

    /* Revenue Ticker Animation */
    @keyframes ticker {
        0% { transform: translateX(100%); }
        100% { transform: translateX(-100%); }
    }
    .ticker-content {
        display: inline-block;
        white-space: nowrap;
        animation: ticker 30s linear infinite;
    }
    
    .whale-glow {
        animation: gold-pulse 2s infinite;
    }
    @keyframes gold-pulse {
        0% { box-shadow: 0 0 0 0 rgba(251, 191, 36, 0.4); }
        70% { box-shadow: 0 0 0 20px rgba(251, 191, 36, 0); }
        100% { box-shadow: 0 0 0 0 rgba(251, 191, 36, 0); }
    }
</style>
</head>
<body>

<div class="fixed inset-0 -z-10 overflow-hidden">
    <div class="slide active bg-[url('https://images.unsplash.com/photo-1512453979798-5ea266f8880c?auto=format&fit=crop&q=80&w=1920')] bg-cover bg-center"></div>
    <div class="slide bg-[url('https://images.unsplash.com/photo-1513635269975-59663e0ac1ad?auto=format&fit=crop&q=80&w=1920')] bg-cover bg-center"></div>
    <div class="slide bg-[url('https://images.unsplash.com/photo-1497366216548-37526070297c?auto=format&fit=crop&q=80&w=1920')] bg-cover bg-center"></div>
    <div class="absolute inset-0 bg-black/70 backdrop-blur-[1px]"></div>
</div>

<nav class="flex justify-between items-center p-6 glass sticky top-0 z-50 border-b border-white/5">
    <div class="logo orbitron text-2xl font-black tracking-tighter">
        🚀 <span class="text-yellow-500">NISAR</span> STUDIO <span class="text-[10px] text-gray-500 uppercase tracking-widest">v7.0 Elite</span>
    </div>
    <div class="flex gap-4 items-center">
        <div id="statusBadge" class="bg-green-500/20 text-green-400 border border-green-500/30 px-4 py-1.5 rounded-full text-[10px] font-bold flex items-center gap-2">
            <span class="w-1.5 h-1.5 bg-green-400 rounded-full animate-pulse"></span> EMPIRE LIVE
        </div>
        <button onclick="evolveSystem()" class="bg-gradient-to-r from-yellow-500 to-amber-700 px-6 py-2 rounded-xl font-bold text-black text-xs hover:scale-105 transition shadow-lg shadow-yellow-500/20">✨ MAGIC EVOLVE</button>
    </div>
</nav>

<div class="w-full bg-yellow-500/5 border-y border-yellow-500/10 py-1.5 overflow-hidden">
    <div class="ticker-content text-yellow-500/80 text-[10px] font-bold uppercase tracking-[0.2em]">
        💰 Latest Whale: $50M ROI Dubai South ... Syncing Google Ledger ... +$10.00 Payout Initialized ... AI Agent V7.0 Node Online ... Global Real Estate Engine Active ... Architect Muhammad Nisar God-Mode Engaged ...
    </div>
</div>

<main class="max-w-7xl mx-auto p-8">
    
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        
        <div id="revCard" class="glass p-8 rounded-3xl border-l-4 border-yellow-500 relative overflow-hidden group">
            <h3 class="text-gray-400 text-xs font-bold uppercase mb-2 tracking-widest">Net Revenue (Live)</h3>
            <p class="text-5xl font-black orbitron text-yellow-500">$<span id="rev">0.00</span></p>
            <button onclick="startRevenue()" class="mt-4 text-[10px] text-yellow-500/50 group-hover:text-yellow-500 transition-colors uppercase font-bold">Initialize Revenue Stream</button>
        </div>

        <div class="glass p-8 rounded-3xl md:col-span-2 relative">
            <h3 class="orbitron text-lg font-bold mb-4 flex items-center gap-2">🤖 AI Agent Brain</h3>
            <div class="flex gap-2">
                <input id="prompt" class="bg-white/5 border border-white/10 w-full p-4 rounded-2xl focus:border-yellow-500 outline-none text-sm transition-all" placeholder="Enter High-Value Command (e.g., Analyze Dubai ROI)...">
                <button onclick="runAI()" class="bg-yellow-500 text-black px-8 rounded-2xl font-black hover:bg-white transition flex items-center gap-2">EXECUTE</button>
            </div>
            <div id="aiOut" class="mt-4 p-4 bg-black/40 rounded-xl text-xs text-gray-400 min-h-[70px] italic leading-relaxed">Awaiting Architect's Command...</div>
        </div>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
        <div class="glass p-6 rounded-2xl border border-white/5 hover:border-blue-500/30 transition">
            <h4 class="text-xs font-bold mb-3 text-blue-400 uppercase tracking-widest">⚙️ API Builder</h4>
            <input id="apiName" class="bg-white/5 p-2.5 rounded-lg text-[10px] w-full mb-2 outline-none border border-white/5 focus:border-blue-500/50" placeholder="Endpoint Name">
            <button onclick="createAPI()" class="w-full text-[10px] bg-blue-600/10 text-blue-400 py-2.5 rounded-lg font-bold hover:bg-blue-600/20">CREATE NODE</button>
            <pre id="apiOut" class="text-[9px] mt-3 text-blue-300 font-mono"></pre>
        </div>

        <div class="glass p-6 rounded-2xl border border-white/5 hover:border-purple-500/30 transition">
            <h4 class="text-xs font-bold mb-3 text-purple-400 uppercase tracking-widest">🔗 Affiliate Engine</h4>
            <input id="url" class="bg-white/5 p-2.5 rounded-lg text-[10px] w-full mb-2 outline-none border border-white/5 focus:border-purple-500/50" placeholder="Product URL">
            <button onclick="genAffiliate()" class="w-full text-[10px] bg-purple-600/10 text-purple-400 py-2.5 rounded-lg font-bold hover:bg-purple-600/20">GENERATE LINK</button>
            <div id="affOut" class="text-[9px] mt-3 break-all text-purple-300 font-mono"></div>
        </div>

        <div class="glass p-6 rounded-2xl border border-white/5 hover:border-emerald-500/30 transition">
            <h4 class="text-xs font-bold mb-3 text-emerald-400 uppercase tracking-widest">🧩 Template Gen</h4>
            <input id="tplName" class="bg-white/5 p-2.5 rounded-lg text-[10px] w-full mb-2 outline-none border border-white/5 focus:border-emerald-500/50" placeholder="Module Name">
            <button onclick="generateTemplate()" class="w-full text-[10px] bg-emerald-600/10 text-emerald-400 py-2.5 rounded-lg font-bold hover:bg-emerald-600/20">INJECT CODE</button>
            <div id="tplOut" class="text-[9px] mt-3 text-emerald-300 font-mono"></div>
        </div>

        <div class="glass p-6 rounded-2xl border border-white/5 hover:border-gray-400/30 transition">
            <h4 class="text-xs font-bold mb-3 text-gray-400 uppercase tracking-widest">🧠 Memory Vault</h4>
            <input id="mem" class="bg-white/5 p-2.5 rounded-lg text-[10px] w-full mb-2 outline-none border border-white/5 focus:border-gray-400/50" placeholder="Save Data String">
            <div class="flex gap-2">
                <button onclick="saveMemory()" class="w-1/2 text-[10px] bg-white/5 py-2.5 rounded-lg font-bold hover:bg-white/10">SAVE</button>
                <button onclick="loadMemory()" class="w-1/2 text-[10px] bg-white/5 py-2.5 rounded-lg font-bold hover:bg-white/10">LOAD</button>
            </div>
            <div id="memOut" class="text-[9px] mt-3 text-gray-500 font-mono"></div>
        </div>
    </div>
</main>

<script>
/* ================= SLIDESHOW LOGIC ================= */
let currentSlide = 0;
const slides = document.querySelectorAll('.slide');

function nextSlide() {
    slides[currentSlide].classList.remove('active');
    currentSlide = (currentSlide + 1) % slides.length;
    slides[currentSlide].classList.add('active');
}
setInterval(nextSlide, 7000);

/* ================= SYSTEM STATE ================= */
const state = {
    revenue: parseFloat(localStorage.getItem("revenue")) || 0.00,
    memory: JSON.parse(localStorage.getItem("memory") || "[]"),
    evolution: 1
};
document.getElementById("rev").innerText = state.revenue.toFixed(2);

function updateUI() {
    document.getElementById("rev").innerText = state.revenue.toFixed(2);
    localStorage.setItem("revenue", state.revenue);
}

/* ================= AI AGENT ================= */
function runAI(){
    const p = document.getElementById("prompt").value;
    const out = document.getElementById("aiOut");
    out.innerHTML = "<span class='animate-pulse text-yellow-500'>🧠 NexusBrain Analyzing Node Path...</span>";
    
    setTimeout(() => {
        if(p.toLowerCase().includes("dubai") || p.toLowerCase().includes("roi")) {
            out.innerHTML = "✅ <span class='text-yellow-500 font-bold uppercase'>Whale Detected:</span> Lead score 98/100. High ROI detected in Dubai South. WhatsApp Alert Triggered. Entry synced to Google Sheets Ledger.";
            state.revenue += 10.00;
            document.getElementById("revCard").classList.add("whale-glow");
            setTimeout(()=>document.getElementById("revCard").classList.remove("whale-glow"), 3000);
            updateUI();
        } else {
            out.innerText = "🤖 Agent Result: Task execution for [" + p + "] successful. Persistence node updated. Memory secured in the Vault.";
        }
    }, 1500);
}

function startRevenue(){
    setInterval(()=>{
        state.revenue += 0.05;
        updateUI();
    }, 3000);
    alert("💸 Revenue Stream Initialized! $5-per-exec tracking live.");
}

function createAPI(){
    const name = document.getElementById("apiName").value;
    document.getElementById("apiOut").innerText = JSON.stringify({endpoint: "/api/"+name, status:"active", version: "7.0"}, null, 2);
}

function genAffiliate(){
    const url = document.getElementById("url").value;
    document.getElementById("affOut").innerText = url + "?ref=nisar_empire_v7";
}

function generateTemplate() {
    const name = document.getElementById("tplName").value;
    document.getElementById("tplOut").innerText = "Generating <" + name + "> module... Injection Successful.";
}

function saveMemory(){
    const val = document.getElementById("mem").value;
    if(!val) return;
    state.memory.push(val);
    localStorage.setItem("memory", JSON.stringify(state.memory));
    document.getElementById("memOut").innerText = "✔ Vault Updated";
}

function loadMemory(){
    document.getElementById("memOut").innerText = state.memory.slice(-2).join(" | ") || "Vault Empty";
}

function evolveSystem(){
    state.evolution++;
    document.getElementById("statusBadge").innerText = "GOD MODE ACTIVE";
    document.getElementById("statusBadge").className = "bg-yellow-500/20 text-yellow-400 border border-yellow-500/40 px-4 py-1.5 rounded-full text-[10px] font-bold";
    alert("⚡ System Evolution Successful. Level " + state.evolution + " Reached. Architect Muhammad Nisar access elevated.");
}
</script>
</body>https://mn-studio-v2.netlify.app/real-estate-ai
</html>

https://github.com/rananisarsb51214-web/Google-cloud-consol-.githttps://github.com/rana51214https://discord.gg/q3NRtPV4u
Simply open `index.html` in your web browser to view the portfolio website.

For deployment to GitHub Pages:
1. Go to your repository settings
2. Navigate to Pages section
3. Select the branch to deploy from
4. Your site will be published at `https://[username].github.io/[repository-name]/`

## Contacthttps://claude.ai/public/artifacts/81b6caee-a9bf-46d4-bb47-fa4e2209dfea

- **nisarsn@gmail.ccom
- **Phone**: 03408060167
- **Location**: Available for Remote Projects

## License

This project is licensed under the terms specified in the LICENSE file.

---

© 2025 Rana Nisar. All rights reserved.
