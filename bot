<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Earn Master Pro</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700&family=Raleway:wght@400;600;700&display=swap');

* { box-sizing: border-box; margin: 0; padding: 0; font-family: 'Raleway', sans-serif; }

body {
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
    background-size: 400% 400%;
    animation: gradientBG 15s ease infinite;
    color: #fff;
    padding: 20px;
    position: relative;
}

@keyframes gradientBG {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}

/* IP Display at top right */
.ip-badge {
    position: absolute;
    top: 15px;
    right: 15px;
    background: rgba(0, 0, 0, 0.7);
    backdrop-filter: blur(5px);
    padding: 6px 12px;
    border-radius: 8px;
    font-size: 12px;
    color: #00ffcc;
    border: 1px solid rgba(0, 255, 204, 0.3);
    z-index: 10;
}

.container {
    background: rgba(18, 18, 24, 0.9);
    backdrop-filter: blur(10px);
    padding: 25px;
    border-radius: 24px;
    width: 100%;
    max-width: 400px;
    box-shadow: 0 15px 35px rgba(0, 0, 0, 0.6);
    text-align: center;
    border: 1px solid rgba(255, 255, 255, 0.1);
}

h1 {
    font-family: 'Orbitron', sans-serif;
    font-size: 24px;
    color: #00ffcc;
    margin-bottom: 10px;
    letter-spacing: 1px;
}

/* Welcome Page Specific Styles */
#welcome-screen h2 {
    font-size: 20px;
    color: #fff;
    margin-bottom: 8px;
}
#welcome-screen p {
    font-size: 13px;
    color: #b3b3b3;
    margin-bottom: 15px;
}

/* Welcome Screen Headline Notice */
.welcome-notice {
    display: block;
    padding: 10px 12px;
    border-radius: 10px;
    font-weight: 600;
    font-size: 13px;
    color: #111;
    background: linear-gradient(90deg, #ff5f6d, #ffc371);
    margin-bottom: 15px;
    box-shadow: 0 4px 15px rgba(255, 95, 109, 0.3);
    line-height: 1.5;
    text-align: center;
}

#welcome-screen input {
    width: 100%;
    padding: 12px;
    margin-bottom: 12px;
    border-radius: 10px;
    border: 1px solid rgba(255,255,255,0.1);
    background: #111;
    color: #fff;
    font-size: 15px;
    text-align: center;
}
#welcome-screen button {
    width: 100%;
    padding: 12px;
    border: none;
    border-radius: 12px;
    font-size: 15px;
    font-weight: bold;
    cursor: pointer;
    color: #111;
    background: linear-gradient(45deg, #1FA2FF, #12D8FA, #A6FFCB);
    transition: 0.3s;
}

/* Main Dashboard Screens */
#main-screen {
    display: none;
}

.user-greeting {
    font-size: 14px;
    color: #00ffcc;
    margin-bottom: 10px;
    font-weight: 600;
}

/* Notice Banner */
.notice-banner {
    display: block;
    padding: 8px 12px;
    border-radius: 10px;
    font-weight: 600;
    font-size: 12px;
    color: #111;
    background: linear-gradient(90deg, #ff5f6d, #ffc371);
    margin-bottom: 15px;
    box-shadow: 0 4px 15px rgba(255, 95, 109, 0.3);
    line-height: 1.4;
}

/* Stats */
.stats {
    display: flex;
    flex-direction: column;
    gap: 8px;
    background: rgba(255, 255, 255, 0.05);
    padding: 12px;
    border-radius: 14px;
    margin-bottom: 15px;
}
.stat-row {
    display: flex;
    justify-content: space-around;
}
.stats p {
    font-size: 13px;
    color: #b3b3b3;
}
.stats span {
    display: block;
    font-size: 16px;
    font-weight: 700;
    color: #00ffcc;
    margin-top: 2px;
}

/* Progress Circle */
.progress-circle {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    background: conic-gradient(#00ffcc 0%, rgba(0,255,204,0.1) 100%);
    margin: 10px auto;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    font-size: 15px;
    color: #00ffcc;
    box-shadow: inset 0 0 10px rgba(0,255,204,0.2);
}

/* Buttons */
.buttons {
    display: flex;
    flex-direction: column;
    gap: 8px;
    margin-top: 10px;
}
.buttons button {
    width: 100%;
    padding: 11px;
    border: none;
    border-radius: 12px;
    font-size: 14px;
    font-weight: 600;
    cursor: pointer;
    color: #fff;
    background: linear-gradient(45deg, #ff512f, #dd2476);
    transition: 0.3s;
    box-shadow: 0 4px 15px rgba(221, 36, 118, 0.3);
}
.buttons button:hover:not(:disabled) {
    transform: translateY(-2px);
    opacity: 0.95;
}
.buttons button:disabled {
    background: #444;
    cursor: not-allowed;
    box-shadow: none;
    opacity: 0.6;
}

.buttons .secondary-btn {
    background: linear-gradient(45deg, #2b5876, #4e4376);
    box-shadow: 0 4px 15px rgba(43, 88, 118, 0.3);
}

/* Withdraw Section */
.withdraw-section {
    margin-top: 12px;
    display: none;
    background: rgba(25, 25, 35, 0.95);
    padding: 15px;
    border-radius: 14px;
    border: 1px solid rgba(255,255,255,0.08);
    text-align: left;
}
.withdraw-section h3 {
    font-size: 15px;
    margin-bottom: 8px;
    color: #00ffcc;
    text-align: center;
}
.withdraw-section button {
    width: 100%;
    padding: 11px;
    margin-top: 6px;
    font-weight: bold;
    font-size: 14px;
    border: none;
    border-radius: 8px;
    background: linear-gradient(45deg, #1FA2FF, #12D8FA, #A6FFCB);
    color: #111;
    cursor: pointer;
    transition: 0.3s;
}
#withdraw-status {
    margin-top: 6px;
    font-size: 12px;
    text-align: center;
    font-weight: 600;
}
</style>
</head>
<body>

<!-- IP Display -->
<div class="ip-badge">IP: <span id="user-ip">Detecting...</span></div>

<div class="container">
    
    <!-- WELCOME / LOGIN SCREEN -->
    <div id="welcome-screen">
        <h1>Earn Master</h1>
        <div class="welcome-notice">৫০ পয়েন্ট অর্জনের পর অবশ্যই বট থেকে বের হয়ে থ্রি ডট অপশনে ক্লিক করে ক্লিয়ার হিস্ট্রি ডাটা (history data) করতে হবে। না হলে, পেমেন্ট পাবেন না</div>
        <p>Enter your username to start earning</p>
        <input type="text" id="username-input" placeholder="Enter Your Username" autocomplete="off">
        <button onclick="handleLogin()">Start Earning</button>
    </div>

    <!-- MAIN DASHBOARD SCREEN -->
    <div id="main-screen">
        <h1>Earn Master</h1>
        <div class="user-greeting">Welcome, <span id="display-username">User</span>!</div>
        <div class="notice-banner">50 ads dekhar por ip change must. nahole payment paben na</div>

        <div class="stats">
            <div class="stat-row">
                <div>
                    <p>Watched Ads</p>
                    <span id="watched-ads">0</span>
                </div>
                <div>
                    <p>Earned Points</p>
                    <span id="earned-points">0.00</span>
                </div>
            </div>
            <div class="stat-row">
                <div>
                    <p>Daily Target</p>
                    <span>3500</span>
                </div>
                <div>
                    <p>Remaining</p>
                    <span id="remaining-points">3500.00</span>
                </div>
            </div>
        </div>

        <div class="progress-circle" id="progress-circle"><span id="ads-progress">0%</span></div>

        <div class="buttons">
            <button id="watch-ad-btn" disabled>Loading Ad SDK...</button>
            <button id="auto-ad-btn" class="secondary-btn" onclick="startAutoAds()">Start Auto Ads</button>
            <button id="stop-auto-btn" class="secondary-btn" onclick="stopAutoAds()" disabled>Stop Auto Ads</button>
            <button onclick="toggleWithdraw()">Withdraw Earnings</button>
        </div>

        <div class="withdraw-section" id="withdraw-section">
            <h3>Request Payout</h3>
            <p style="font-size: 13px; color: #ccc; text-align: center; margin-bottom: 8px;">Min Withdrawal: 3500 Points</p>
            <button onclick="withdrawPoints()">Submit Withdrawal Request</button>
            <p id="withdraw-status"></p>
        </div>
    </div>

</div>

<!-- New Monetag SDK (Zone: 11057205) -->
<script src='//libtl.com/sdk.js' data-zone='11057205' data-sdk='show_11057205'></script>

<script>
const WEB_APP_URL = "https://script.google.com/macros/s/AKfycbziSU1TtLBpHQYKGTsruOj9h6LWq9y5pMEiRoXtmlrPbhFAwRLCXN7zQa3i7vH1oWMhrw/exec";

let currentUsername = localStorage.getItem('earnMasterUsername') || '';
let earnedPoints = 0;
let watchedAdsCount = parseInt(localStorage.getItem('watchedAdsCount')) || 0;
let autoAdInterval = null;
let monetagLoaded = false;
let currentIP = "Unknown";
const dailyTarget = 3500;

// IP Detection
function getClientIP() {
    fetch('https://api.ipify.org?format=json')
        .then(res => res.json())
        .then(data => {
            currentIP = data.ip;
            document.getElementById('user-ip').textContent = currentIP;
        })
        .catch(() => {
            fetch('https://ipapi.co/json/')
                .then(res => res.json())
                .then(data => {
                    currentIP = data.ip || 'Dynamic';
                    document.getElementById('user-ip').textContent = currentIP;
                })
                .catch(() => {
                    document.getElementById('user-ip').textContent = 'Dynamic IP';
                });
        });
}
getClientIP();

// Check Login Status on Load & Fetch Points from Google Sheet
window.addEventListener('DOMContentLoaded', () => {
    if(currentUsername){
        document.getElementById('welcome-screen').style.display = 'none';
        document.getElementById('main-screen').style.display = 'block';
        document.getElementById('display-username').textContent = currentUsername;
        fetchUserPoints(currentUsername);
    }
});

// Handle Login
function handleLogin(){
    const username = document.getElementById('username-input').value.trim();
    if(!username){
        alert('Please enter a valid username!');
        return;
    }
    currentUsername = username;
    localStorage.setItem('earnMasterUsername', username);
    
    document.getElementById('welcome-screen').style.display = 'none';
    document.getElementById('main-screen').style.display = 'block';
    document.getElementById('display-username').textContent = username;
    fetchUserPoints(username);
}

// Fetch Points from Google Sheet API
function fetchUserPoints(username) {
    fetch(`${WEB_APP_URL}?username=${encodeURIComponent(username)}`)
        .then(res => res.json())
        .then(data => {
            if(data.status === "success"){
                earnedPoints = data.totalPoints;
                updateStatsUI();
            }
        })
        .catch(err => console.error("Error fetching points:", err));
}

function updateStatsUI(){
    document.getElementById('watched-ads').textContent = watchedAdsCount;
    document.getElementById('earned-points').textContent = earnedPoints.toFixed(2);
    
    let remaining = Math.max(0, dailyTarget - earnedPoints);
    document.getElementById('remaining-points').textContent = remaining.toFixed(2);
    
    updateProgressCircle();
}

// SDK Checker Loop (Updated for show_11057205)
function checkSDK(){
    if(typeof window.show_11057205 === 'function'){
        monetagLoaded = true;
        const watchBtn = document.getElementById('watch-ad-btn');
        watchBtn.disabled = false;
        watchBtn.textContent = 'Watch Ad (+1 Pt)';
    } else {
        setTimeout(checkSDK, 500);
    }
}
window.addEventListener('DOMContentLoaded', checkSDK);

function updateProgressCircle(){
    let cycleAds = earnedPoints % 50;
    if(earnedPoints > 0 && cycleAds === 0) cycleAds = 50;
    let percent = (cycleAds / 50) * 100;
    
    document.getElementById('ads-progress').textContent = Math.round(percent) + '%';
    document.getElementById('progress-circle').style.background = `conic-gradient(#00ffcc ${percent}%, rgba(0,255,204,0.1) ${percent}%)`;
}

// Watch Ad Handler (1 Ad = 1 Point sent to Google Sheet)
document.getElementById('watch-ad-btn').addEventListener('click', ()=>{
    if(!monetagLoaded){ 
        alert('Ad network is still loading. Please wait a moment.'); 
        return; 
    }
    
    // Trigger the new Monetag SDK function
    show_11057205().then(()=>{
        watchedAdsCount++;
        localStorage.setItem('watchedAdsCount', watchedAdsCount);

        // Send point update to Google Sheet API
        fetch(WEB_APP_URL, {
            method: "POST",
            body: JSON.stringify({
                username: currentUsername,
                points: 1,
                ip: currentIP
            })
        })
        .then(res => res.json())
        .then(data => {
            if(data.status === "success"){
                earnedPoints = data.totalPoints;
                updateStatsUI();
                
                // Every 50 points, enforce close app rule
                if(earnedPoints > 0 && earnedPoints % 50 === 0){
                    stopAutoAds();
                    alert("৫০ পয়েন্ট অর্জিত হয়েছে! এখন অবশ্যই বট থেকে বের হয়ে থ্রি ডট অপশনে ক্লিক করে ক্লিয়ার হিস্ট্রি ডাটা (history data) করুন, তারপর অ্যাপ রিওপেন করে কাজ করুন।");
                }
            }
        })
        .catch(err => {
            console.error("Failed to sync points:", err);
            alert("Point sync failed, check your internet connection.");
        });

    }).catch(e=>{ 
        console.error(e); 
    });
});

// Auto Ads Control
function startAutoAds(){
    if(!monetagLoaded){ alert('Ad network not ready.'); return; }
    
    autoAdInterval = setInterval(()=>{ 
        document.getElementById('watch-ad-btn').click(); 
    }, 6000); 
    
    document.getElementById('auto-ad-btn').disabled = true;
    document.getElementById('stop-auto-btn').disabled = false;
}

function stopAutoAds(){
    if(autoAdInterval) clearInterval(autoAdInterval);
    document.getElementById('auto-ad-btn').disabled = false;
    document.getElementById('stop-auto-btn').disabled = true;
}

// Withdraw Section Toggle & Logic (Min 3500)
function toggleWithdraw(){ 
    const section = document.getElementById('withdraw-section');
    section.style.display = section.style.display === 'block' ? 'none' : 'block'; 
}

function withdrawPoints(){
    const statusEl = document.getElementById('withdraw-status');
    
    if(earnedPoints < 3500){ 
        statusEl.style.color = '#ff4d4d';
        statusEl.textContent = "Minimum 3500 points required to withdraw!"; 
        return; 
    }
    
    statusEl.style.color = '#00ffcc';
    statusEl.textContent = "Withdrawal request submitted successfully! Admin will check.";
}
</script>

</body>
</html>
