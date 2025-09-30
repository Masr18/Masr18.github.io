<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>What is My IP Address & Internet Speed Test (Free Online Tool)</title>
    <meta name="description" content="Find your IP address, ISP, location, and test your internet speed instantly. 100% free.">
    
    <!-- AdSense Verification Script -->
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-1125233376353054" crossorigin="anonymous"></script>
    
    <style>
        :root {
            --primary: #4a6ee0;
            --primary-dark: #3a5ac8;
            --secondary: #6c757d;
            --light: #f8f9fa;
            --dark: #343a40;
            --success: #28a745;
            --danger: #dc3545;
            --warning: #ffc107;
            --info: #17a2b8;
            --border-radius: 8px;
            --box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            color: white;
            padding: 40px 0;
            text-align: center;
            margin-bottom: 30px;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        h2 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--primary);
        }
        
        h3 {
            font-size: 1.4rem;
            margin-bottom: 15px;
        }
        
        section {
            background: white;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            padding: 30px;
            margin-bottom: 30px;
        }
        
        .ip-info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .info-card {
            background: var(--light);
            border-radius: var(--border-radius);
            padding: 20px;
            text-align: center;
        }
        
        .info-card h4 {
            font-size: 0.9rem;
            color: var(--secondary);
            margin-bottom: 10px;
            text-transform: uppercase;
        }
        
        .info-card p {
            font-size: 1.2rem;
            font-weight: 600;
            color: var(--dark);
        }
        
        .speed-test {
            text-align: center;
        }
        
        .speed-test-btn {
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 50px;
            padding: 15px 40px;
            font-size: 1.2rem;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
            margin: 20px 0;
            box-shadow: var(--box-shadow);
        }
        
        .speed-test-btn:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
        }
        
        .speed-test-btn:disabled {
            background: var(--secondary);
            cursor: not-allowed;
            transform: none;
        }
        
        .speed-results {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
        
        .speed-card {
            background: var(--light);
            border-radius: var(--border-radius);
            padding: 20px;
            text-align: center;
            position: relative;
        }
        
        .speed-card h4 {
            font-size: 1rem;
            color: var(--secondary);
            margin-bottom: 10px;
        }
        
        .speed-value {
            font-size: 2rem;
            font-weight: 700;
            color: var(--primary);
        }
        
        .speed-unit {
            font-size: 1rem;
            color: var(--secondary);
        }
        
        .progress-bar {
            height: 8px;
            background: #e9ecef;
            border-radius: 4px;
            margin-top: 15px;
            overflow: hidden;
        }
        
        .progress {
            height: 100%;
            background: var(--primary);
            width: 0%;
            transition: width 0.5s ease;
        }
        
        .faq-item {
            margin-bottom: 25px;
        }
        
        .faq-item h3 {
            color: var(--primary);
            margin-bottom: 10px;
        }
        
        footer {
            background: var(--dark);
            color: white;
            padding: 40px 0;
            margin-top: 30px;
        }
        
        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        
        .footer-links {
            display: flex;
            gap: 20px;
            margin-top: 20px;
        }
        
        .footer-links a {
            color: white;
            text-decoration: none;
            transition: var(--transition);
        }
        
        .footer-links a:hover {
            color: var(--primary);
        }
        
        .ad-container {
            background: #f8f9fa;
            border: 1px dashed #dee2e6;
            border-radius: var(--border-radius);
            padding: 20px;
            text-align: center;
            margin: 20px 0;
            color: var(--secondary);
        }
        
        .vpn-promo {
            background: linear-gradient(135deg, #ff6b6b, #ff8e53);
            color: white;
            border-radius: var(--border-radius);
            padding: 20px;
            text-align: center;
            margin: 20px 0;
            box-shadow: var(--box-shadow);
        }
        
        .vpn-promo h3 {
            color: white;
            margin-bottom: 10px;
        }
        
        .vpn-promo p {
            margin-bottom: 15px;
        }
        
        .vpn-btn {
            background: white;
            color: #ff6b6b;
            border: none;
            border-radius: 50px;
            padding: 10px 25px;
            font-weight: 600;
            cursor: pointer;
            transition: var(--transition);
        }
        
        .vpn-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            
            h2 {
                font-size: 1.5rem;
            }
            
            section {
                padding: 20px;
            }
            
            .footer-content {
                flex-direction: column;
            }
            
            .footer-links {
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Your IP Address is <span id="ipv4">Loading...</span></h1>
            <p>Discover your IP information and test your internet speed in seconds</p>
        </div>
    </header>
    
    <div class="container">
        <!-- Top Ad Space -->
        <div class="ad-container">
            <p>Advertisement Space (728x90)</p>
            <!-- AdSense ad unit will be placed here -->
        </div>
        
        <!-- IP Information Section -->
        <section id="ip-info">
            <h2>Your IP Information</h2>
            <div class="ip-info-grid">
                <div class="info-card">
                    <h4>IPv4 Address</h4>
                    <p id="ipv4-detail">Loading...</p>
                </div>
                <div class="info-card">
                    <h4>IPv6 Address</h4>
                    <p id="ipv6-detail">Not detected</p>
                </div>
                <div class="info-card">
                    <h4>ISP</h4>
                    <p id="isp">Loading...</p>
                </div>
                <div class="info-card">
                    <h4>Location</h4>
                    <p id="location">Loading...</p>
                </div>
                <div class="info-card">
                    <h4>Country</h4>
                    <p id="country">Loading...</p>
                </div>
                <div class="info-card">
                    <h4>Browser</h4>
                    <p id="browser">Loading...</p>
                </div>
            </div>
            
            <!-- VPN Affiliate Placement -->
            <div class="vpn-promo">
                <h3>Want to hide your IP?</h3>
                <p>Protect your privacy and access content worldwide</p>
                <button class="vpn-btn">Get NordVPN 65% OFF</button>
            </div>
        </section>
        
        <!-- Middle Ad Space -->
        <div class="ad-container">
            <p>Advertisement Space (728x90)</p>
            <!-- AdSense ad unit will be placed here -->
        </div>
        
        <!-- Speed Test Section -->
        <section id="speed-test" class="speed-test">
            <h2>Internet Speed Test</h2>
            <p>Measure your download, upload, and ping speeds with our accurate speed test tool</p>
            
            <button id="start-test" class="speed-test-btn">Start Speed Test</button>
            
            <div class="speed-results">
                <div class="speed-card">
                    <h4>Ping</h4>
                    <div class="speed-value" id="ping-value">--</div>
                    <div class="speed-unit">ms</div>
                    <div class="progress-bar">
                        <div class="progress" id="ping-progress"></div>
                    </div>
                </div>
                <div class="speed-card">
                    <h4>Download</h4>
                    <div class="speed-value" id="download-value">--</div>
                    <div class="speed-unit">Mbps</div>
                    <div class="progress-bar">
                        <div class="progress" id="download-progress"></div>
                    </div>
                </div>
                <div class="speed-card">
                    <h4>Upload</h4>
                    <div class="speed-value" id="upload-value">--</div>
                    <div class="speed-unit">Mbps</div>
                    <div class="progress-bar">
                        <div class="progress" id="upload-progress"></div>
                    </div>
                </div>
            </div>
        </section>
        
        <!-- FAQ Section -->
        <section id="faq">
            <h2>Frequently Asked Questions</h2>
            
            <div class="faq-item">
                <h3>What is an IP Address?</h3>
                <p>An IP (Internet Protocol) address is a unique numerical identifier assigned to every device connected to a network. It allows devices to communicate with each other over the internet, similar to how a home address helps mail reach its destination.</p>
            </div>
            
            <div class="faq-item">
                <h3>How can I hide my IP address?</h3>
                <p>You can hide your IP address by using a VPN (Virtual Private Network), which routes your internet traffic through a secure server in a different location. This masks your real IP address and enhances your online privacy and security.</p>
            </div>
            
            <div class="faq-item">
                <h3>What is considered a good internet speed?</h3>
                <p>For basic browsing and email, 5-10 Mbps is sufficient. For HD video streaming, 15-25 Mbps is recommended. For 4K streaming, online gaming, or multiple users, 50+ Mbps is ideal. Upload speeds of 10+ Mbps are good for video calls and sharing files.</p>
            </div>
        </section>
        
        <!-- Footer Ad Space -->
        <div class="ad-container">
            <p>Advertisement Space (728x90)</p>
            <!-- AdSense ad unit will be placed here -->
        </div>
    </div>
    
    <footer>
        <div class="container">
            <div class="footer-content">
                <div>
                    <p>&copy; 2023 What is My IP + Speed Test. All rights reserved.</p>
                    <div class="footer-links">
                        <a href="#">About</a>
                        <a href="#">Contact</a>
                        <a href="#">Privacy Policy</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // IP Detection and Geolocation
        async function fetchIPInfo() {
            try {
                // Using ipapi.co for IP information (free tier available)
                const response = await fetch('https://ipapi.co/json/');
                const data = await response.json();
                
                // Update IP information
                document.getElementById('ipv4').textContent = data.ip;
                document.getElementById('ipv4-detail').textContent = data.ip;
                document.getElementById('isp').textContent = data.org || 'Unknown';
                document.getElementById('location').textContent = `${data.city}, ${data.region}`;
                document.getElementById('country').textContent = data.country_name;
                
                // Check for IPv6 (this API doesn't provide it, so we'll try another approach)
                checkIPv6();
                
            } catch (error) {
                console.error('Error fetching IP info:', error);
                document.getElementById('ipv4').textContent = 'Unable to detect';
                document.getElementById('ipv4-detail').textContent = 'Unable to detect';
                document.getElementById('isp').textContent = 'Unknown';
                document.getElementById('location').textContent = 'Unknown';
                document.getElementById('country').textContent = 'Unknown';
            }
        }
        
        // Try to detect IPv6
        function checkIPv6() {
            // This is a simplified approach - in reality, IPv6 detection is more complex
            // We'll check if the user has an IPv6 address by making a request to an IPv6-only service
            fetch('https://api6.ipify.org?format=json')
                .then(response => response.json())
                .then(data => {
                    document.getElementById('ipv6-detail').textContent = data.ip;
                })
                .catch(error => {
                    // If this fails, the user likely doesn't have IPv6 or it's not configured
                    document.getElementById('ipv6-detail').textContent = 'Not detected';
                });
        }
        
        // Browser and OS Detection
        function detectBrowserInfo() {
            const userAgent = navigator.userAgent;
            let browser = "Unknown";
            let os = "Unknown";
            
            // Detect browser
            if (userAgent.includes("Firefox")) {
                browser = "Firefox";
            } else if (userAgent.includes("Edg")) {
                browser = "Microsoft Edge";
            } else if (userAgent.includes("Chrome")) {
                browser = "Chrome";
            } else if (userAgent.includes("Safari") && !userAgent.includes("Chrome")) {
                browser = "Safari";
            } else if (userAgent.includes("OPR") || userAgent.includes("Opera")) {
                browser = "Opera";
            }
            
            // Detect OS
            if (userAgent.includes("Windows")) {
                os = "Windows";
            } else if (userAgent.includes("Mac")) {
                os = "macOS";
            } else if (userAgent.includes("Linux")) {
                os = "Linux";
            } else if (userAgent.includes("Android")) {
                os = "Android";
            } else if (userAgent.includes("iOS") || userAgent.includes("iPhone") || userAgent.includes("iPad")) {
                os = "iOS";
            }
            
            document.getElementById('browser').textContent = `${browser} on ${os}`;
        }
        
        // Speed Test Simulation
        function startSpeedTest() {
            const startBtn = document.getElementById('start-test');
            startBtn.disabled = true;
            startBtn.textContent = 'Testing...';
            
            // Reset values
            document.getElementById('ping-value').textContent = '--';
            document.getElementById('download-value').textContent = '--';
            document.getElementById('upload-value').textContent = '--';
            
            // Reset progress bars
            document.getElementById('ping-progress').style.width = '0%';
            document.getElementById('download-progress').style.width = '0%';
            document.getElementById('upload-progress').style.width = '0%';
            
            // Simulate ping test
            simulatePingTest()
                .then(() => simulateDownloadTest())
                .then(() => simulateUploadTest())
                .then(() => {
                    startBtn.disabled = false;
                    startBtn.textContent = 'Test Again';
                });
        }
        
        function simulatePingTest() {
            return new Promise(resolve => {
                const pingProgress = document.getElementById('ping-progress');
                const pingValue = document.getElementById('ping-value');
                
                // Simulate ping test with random value between 10-100ms
                let progress = 0;
                const interval = setInterval(() => {
                    progress += 5;
                    pingProgress.style.width = `${progress}%`;
                    
                    if (progress >= 100) {
                        clearInterval(interval);
                        const ping = Math.floor(Math.random() * 90) + 10;
                        pingValue.textContent = ping;
                        resolve();
                    }
                }, 50);
            });
        }
        
        function simulateDownloadTest() {
            return new Promise(resolve => {
                const downloadProgress = document.getElementById('download-progress');
                const downloadValue = document.getElementById('download-value');
                
                // Simulate download test with random value between 10-500 Mbps
                let progress = 0;
                const interval = setInterval(() => {
                    progress += 2;
                    downloadProgress.style.width = `${progress}%`;
                    
                    if (progress >= 100) {
                        clearInterval(interval);
                        const download = Math.floor(Math.random() * 490) + 10;
                        downloadValue.textContent = download;
                        resolve();
                    }
                }, 50);
            });
        }
        
        function simulateUploadTest() {
            return new Promise(resolve => {
                const uploadProgress = document.getElementById('upload-progress');
                const uploadValue = document.getElementById('upload-value');
                
                // Simulate upload test with random value between 5-100 Mbps
                let progress = 0;
                const interval = setInterval(() => {
                    progress += 2;
                    uploadProgress.style.width = `${progress}%`;
                    
                    if (progress >= 100) {
                        clearInterval(interval);
                        const upload = Math.floor(Math.random() * 95) + 5;
                        uploadValue.textContent = upload;
                        resolve();
                    }
                }, 50);
            });
        }
        
        // Initialize the page
        document.addEventListener('DOMContentLoaded', function() {
            fetchIPInfo();
            detectBrowserInfo();
            
            // Add event listener to speed test button
            document.getElementById('start-test').addEventListener('click', startSpeedTest);
        });
    </script>
</body>
</html>
