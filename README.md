<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DentalSpace Pro - AI-Enhanced Tandartspraktijk Inrichting Specialist</title>
    <meta name="description" content="DentalSpace Pro helpt tandartsen met slimme praktijkinrichting. AI-ondersteuning, expert advies en exclusieve deals via onze partners DentalMa en IsSolid.">
    <meta name="keywords" content="tandartspraktijk inrichting, dentalma, issolid, solid surface, praktijkrealisatie, AI chatbot">
    <link rel="icon" href="data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><text y='.9em' font-size='90'>🦷</text></svg>">
    
    <!-- Open Graph voor social media -->
    <meta property="og:title" content="DentalSpace Pro - AI-Enhanced Praktijkinrichting">
    <meta property="og:description" content="Slimme adviezen voor tandartspraktijk inrichting met AI-ondersteuning">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://dentalspacepro.nl">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            overflow-x: hidden;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            color: white;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000"><defs><radialGradient id="a" cx="50%" cy="50%"><stop offset="0%" stop-color="%23ffffff" stop-opacity="0.1"/><stop offset="100%" stop-color="%23ffffff" stop-opacity="0"/></radialGradient></defs><circle cx="200" cy="200" r="100" fill="url(%23a)"/><circle cx="800" cy="300" r="150" fill="url(%23a)"/><circle cx="600" cy="800" r="120" fill="url(%23a)"/></svg>') no-repeat center center;
            background-size: cover;
            opacity: 0.3;
        }

        .hero-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
            z-index: 2;
            position: relative;
        }

        .hero-text h1 {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 1rem;
            background: linear-gradient(135deg, #ffffff, #e0e6ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-text p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .ai-badge {
            background: linear-gradient(45deg, #ff6b6b, #ee5a24);
            color: white;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 1rem;
            display: inline-block;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { opacity: 1; }
            50% { opacity: 0.7; }
            100% { opacity: 1; }
        }

        .cta-buttons {
            display: flex;
            gap: 20px;
            margin-bottom: 2rem;
        }

        .btn-primary {
            background: linear-gradient(135deg, #e74c3c, #c0392b);
            color: white;
            padding: 15px 30px;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(231, 76, 60, 0.3);
        }

        .btn-secondary {
            background: transparent;
            color: white;
            padding: 15px 30px;
            border: 2px solid white;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
        }

        .btn-secondary:hover {
            background: white;
            color: #667eea;
        }

        .hero-stats {
            display: flex;
            gap: 30px;
            margin-top: 2rem;
        }

        .stat {
            text-align: center;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: 700;
            display: block;
        }

        .stat-label {
            font-size: 0.9rem;
            opacity: 0.8;
        }

        /* AI Chatbot Styles */
        .hero-chatbot {
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.1);
            overflow: hidden;
            transform: perspective(1000px) rotateY(-5deg);
            transition: transform 0.3s ease;
        }

        .hero-chatbot:hover {
            transform: perspective(1000px) rotateY(0deg);
        }

        .chatbot-container {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            height: 600px;
            display: flex;
            flex-direction: column;
        }

        .chatbot-header {
            background: linear-gradient(135deg, #4a90e2 0%, #357abd 100%);
            color: white;
            padding: 20px;
            text-align: center;
            position: relative;
        }

        .chatbot-header h3 {
            margin-bottom: 5px;
            font-size: 1.3rem;
        }

        .chatbot-header p {
            opacity: 0.9;
            font-size: 0.9rem;
        }

        .ai-status {
            position: absolute;
            top: 10px;
            right: 15px;
            font-size: 0.8rem;
            background: rgba(255,255,255,0.2);
            padding: 4px 8px;
            border-radius: 10px;
        }

        .setup-panel {
            background: #f8f9fa;
            border-bottom: 2px solid #e9ecef;
            padding: 15px;
            text-align: center;
        }

        .setup-panel.hidden {
            display: none;
        }

        .api-input {
            width: 80%;
            padding: 8px 12px;
            border: 2px solid #ddd;
            border-radius: 20px;
            margin-right: 10px;
            font-size: 0.9rem;
        }

        .setup-btn {
            background: #28a745;
            color: white;
            border: none;
            padding: 8px 16px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 0.9rem;
        }

        .setup-btn:hover {
            background: #218838;
        }

        .chat-messages {
            flex: 1;
            overflow-y: auto;
            padding: 20px;
            display: flex;
            flex-direction: column;
            gap: 15px;
            background: #fafafa;
        }

        .message {
            display: flex;
            align-items: flex-start;
            gap: 10px;
            animation: fadeInUp 0.3s ease-out;
        }

        .message.user {
            flex-direction: row-reverse;
        }

        .message-avatar {
            width: 35px;
            height: 35px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1rem;
            flex-shrink: 0;
        }

        .message.bot .message-avatar {
            background: linear-gradient(135deg, #4a90e2, #357abd);
            color: white;
        }

        .message.user .message-avatar {
            background: #e74c3c;
            color: white;
        }

        .message.ai .message-avatar {
            background: linear-gradient(135deg, #ff6b6b, #ee5a24);
            color: white;
        }

        .message-content {
            background: white;
            padding: 12px 16px;
            border-radius: 18px;
            max-width: 75%;
            word-wrap: break-word;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
            position: relative;
        }

        .message-content a {
            color: #4a90e2;
            text-decoration: none;
            font-weight: 600;
        }

        .message-content a:hover {
            text-decoration: underline;
        }

        .message.user .message-content {
            background: #4a90e2;
            color: white;
        }

        .message.user .message-content a {
            color: #ffffff;
            text-decoration: underline;
        }

        .message.ai .message-content {
            background: linear-gradient(135deg, #ff6b6b, #ee5a24);
            color: white;
        }

        .message-source {
            font-size: 0.7rem;
            opacity: 0.7;
            margin-top: 5px;
            text-align: right;
        }

        .ai-thinking {
            background: rgba(255, 107, 107, 0.1);
            border-left: 4px solid #ff6b6b;
            color: #333;
            font-style: italic;
        }

        .chat-input-container {
            padding: 15px 20px;
            border-top: 1px solid #eee;
            display: flex;
            gap: 10px;
            background: white;
        }

        .chat-input {
            flex: 1;
            padding: 12px 16px;
            border: 2px solid #e0e0e0;
            border-radius: 25px;
            outline: none;
            font-size: 0.9rem;
            transition: border-color 0.3s ease;
        }

        .chat-input:focus {
            border-color: #4a90e2;
        }

        .send-button {
            background: linear-gradient(45deg, #e74c3c, #c0392b);
            color: white;
            border: none;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        .send-button:hover {
            transform: scale(1.05);
        }

        .send-button:disabled {
            background: #ccc;
            cursor: not-allowed;
            transform: none;
        }

        .quick-suggestions {
            padding: 10px 15px;
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            background: #f8f9fa;
        }

        .suggestion-btn {
            background: white;
            border: 1px solid #ddd;
            border-radius: 15px;
            padding: 6px 12px;
            cursor: pointer;
            font-size: 0.8rem;
            transition: all 0.3s ease;
        }

        .suggestion-btn:hover {
            background: #4a90e2;
            color: white;
            border-color: #4a90e2;
        }

        .suggestion-btn.ai-suggestion {
            background: linear-gradient(45deg, #ff6b6b, #ee5a24);
            color: white;
            border: none;
        }

        .typing-indicator {
            display: none;
            padding: 8px 16px;
            background: white;
            border-radius: 18px;
            max-width: 70px;
        }

        .typing-dots {
            display: flex;
            gap: 4px;
        }

        .typing-dots span {
            width: 6px;
            height: 6px;
            border-radius: 50%;
            background: #4a90e2;
            animation: typingBounce 1.4s ease-in-out infinite both;
        }

        .typing-dots span:nth-child(1) { animation-delay: -0.32s; }
        .typing-dots span:nth-child(2) { animation-delay: -0.16s; }

        @keyframes typingBounce {
            0%, 80%, 100% { 
                transform: scale(0);
            } 40% { 
                transform: scale(1);
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Instructions Panel */
        .instructions-panel {
            background: #e8f4fd;
            border: 2px solid #4a90e2;
            border-radius: 10px;
            padding: 20px;
            margin: 20px;
            display: block;
        }

        .instructions-panel.hidden {
            display: none;
        }

        .instructions-panel h3 {
            color: #2c5aa0;
            margin-bottom: 15px;
        }

        .instructions-panel ol {
            color: #2c5aa0;
            line-height: 1.8;
        }

        .instructions-panel li {
            margin-bottom: 8px;
        }

        .instructions-panel code {
            background: #fff;
            padding: 2px 6px;
            border-radius: 4px;
            font-family: monospace;
            color: #e74c3c;
        }

        /* Services Section */
        .services {
            padding: 100px 0;
            background: #f8f9fa;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-title h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .section-title p {
            font-size: 1.2rem;
            color: #666;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: white;
            padding: 40px 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 50px rgba(0,0,0,0.1);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 20px;
            display: block;
        }

        .service-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            color: #333;
        }

        .service-card p {
            color: #666;
            line-height: 1.6;
        }

        /* Partners Section */
        .partners {
            padding: 100px 0;
            background: white;
        }

        .partners-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 40px;
            max-width: 900px;
            margin: 0 auto;
        }

        .partner-card {
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
        }

        .partner-card:hover {
            transform: translateY(-5px);
        }

        .partner-header {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }

        .partner-logo {
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, #667eea, #764ba2);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.5rem;
            font-weight: bold;
            margin-right: 15px;
        }

        .partner-card h3 {
            font-size: 1.5rem;
            color: #333;
        }

        .partner-features {
            list-style: none;
            margin: 20px 0;
        }

        .partner-features li {
            padding: 8px 0;
            color: #666;
            position: relative;
            padding-left: 25px;
        }

        .partner-features li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #28a745;
            font-weight: bold;
        }

        /* CTA Section */
        .cta-section {
            padding: 100px 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            text-align: center;
        }

        .cta-content h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        .cta-content p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            opacity: 0.9;
        }

        /* Mobile Responsive */
        @media (max-width: 768px) {
            .hero-content {
                grid-template-columns: 1fr;
                gap: 40px;
                text-align: center;
            }

            .hero-text h1 {
                font-size: 2.5rem;
            }

            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }

            .hero-stats {
                justify-content: center;
            }

            .chatbot-container {
                height: 500px;
            }

            .api-input {
                width: 70%;
                margin-bottom: 10px;
            }

            .section-title h2 {
                font-size: 2rem;
            }

            .partner-header {
                flex-direction: column;
                text-align: center;
            }

            .partner-logo {
                margin-right: 0;
                margin-bottom: 10px;
            }
        }

        /* Cookie Notice */
        .cookie-notice {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background: #333;
            color: white;
            padding: 15px;
            text-align: center;
            z-index: 1000;
            display: none;
        }

        .cookie-notice.show {
            display: block;
        }

        .cookie-notice button {
            background: #4a90e2;
            color: white;
            border: none;
            padding: 8px 16px;
            border-radius: 5px;
            margin-left: 10px;
            cursor: pointer;
        }

        /* Footer */
        .footer {
            background: #333;
            color: white;
            padding: 40px 0;
            text-align: center;
        }

        .footer p {
            margin-bottom: 10px;
        }

        .footer a {
            color: #4a90e2;
            text-decoration: none;
        }

        .footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <!-- Hero Section with AI-Enhanced Chatbot -->
    <section class="hero">
        <div class="hero-content">
            <div class="hero-text">
                <div class="ai-badge">🧠 Powered by AI + Expert Knowledge</div>
                <h1>DentalSpace Pro</h1>
                <p>Nu met AI-ondersteuning! Krijg slimme adviezen over praktijkinrichting, gecombineerd met onze specialistische kennis.</p>
                
                <div class="cta-buttons">
                    <a href="#chat" class="btn-primary" onclick="scrollToChat(); return false;">🧠 Probeer AI Chat</a>
                    <a href="#instructions" class="btn-secondary" onclick="showInstructions(); return false;">⚙️ Setup Guide</a>
                </div>

                <div class="hero-stats">
                    <div class="stat">
                        <span class="stat-number">AI+</span>
                        <span class="stat-label">Smart Responses</span>
                    </div>
                    <div class="stat">
                        <span class="stat-number">24/7</span>
                        <span class="stat-label">Beschikbaar</span>
                    </div>
                    <div class="stat">
                        <span class="stat-number">∞</span>
                        <span class="stat-label">Zelflerend</span>
                    </div>
                </div>
            </div>

            <div class="hero-chatbot" id="chat">
                <!-- Setup Instructions Panel -->
                <div class="instructions-panel" id="instructionsPanel">
                    <h3>🚀 AI Setup (5 minuten)</h3>
                    <ol>
                        <li>Ga naar <code>platform.openai.com/api-keys</code></li>
                        <li>Maak een account (gratis $5 credit)</li>
                        <li>Klik "Create new secret key"</li>
                        <li>Kopieer de API key (begint met sk-...)</li>
                        <li>Plak hieronder en klik "Activeer AI"</li>
                    </ol>
                    <p><strong>💰 Kosten:</strong> ~€0.01 per vraag | <strong>🔒 Privacy:</strong> API key blijft lokaal</p>
                </div>

                <div class="chatbot-container">
                    <div class="chatbot-header">
                        <div class="ai-status" id="aiStatus">🔴 AI Uit</div>
                        <h3>🦷 DentalSpace Pro AI Assistent</h3>
                        <p>Specialist kennis + AI intelligentie</p>
                    </div>

                    <!-- API Setup Panel -->
                    <div class="setup-panel" id="setupPanel">
                        <input type="password" id="apiKeyInput" class="api-input" placeholder="Plak je OpenAI API key hier (sk-...)">
                        <button onclick="setupAI()" class="setup-btn">Activeer AI 🧠</button>
                        <div style="margin-top: 8px; font-size: 0.8rem; color: #666;">
                            <span onclick="showInstructions()" style="cursor: pointer; color: #4a90e2;">📖 Setup instructies</span> | 
                            <span onclick="skipAI()" style="cursor: pointer; color: #e74c3c;">⏭️ Skip AI (gebruik basis versie)</span>
                        </div>
                    </div>

                    <div class="chat-messages" id="chatMessages">
                        <div class="message bot">
                            <div class="message-avatar">🤖</div>
                            <div class="message-content">
                                Hallo! Ik ben je DentalSpace Pro adviseur met AI-ondersteuning! 🧠
                                <br><br>
                                <strong>🎯 Nieuw:</strong> Ik kan nu complexe vragen beantwoorden, leren van gesprekken en slimme adviezen geven over praktijkinrichting.
                                <br><br>
                                <strong>🔗 Alle links werken perfect:</strong> Klik op contact links om direct te bellen of emailen!
                                <br><br>
                                <strong>⚙️ Setup:</strong> Activeer AI voor de beste ervaring, of gebruik de basis versie met expert kennis.
                                <div class="message-source">💡 DentalSpace Pro Knowledge Base</div>
                            </div>
                        </div>
                    </div>

                    <div class="quick-suggestions">
                        <div class="suggestion-btn" onclick="sendSuggestion('Wat kost een moderne praktijk met 3 behandelkamers?')">💰 Gedetailleerde Kosten</div>
                        <div class="suggestion-btn ai-suggestion" onclick="sendSuggestion('Geef me 5 tips voor een efficiënte praktijkindeling')">🧠 AI Tips</div>
                        <div class="suggestion-btn" onclick="sendSuggestion('DentalMa contact')">🏗️ DentalMa via Expert</div>
                        <div class="suggestion-btn" onclick="sendSuggestion('IsSolid meubilair info')">💎 IsSolid via Expert</div>
                        <div class="suggestion-btn" onclick="sendSuggestion('persoonlijk contact')">🤝 Expert Contact</div>
                        <div class="suggestion-btn ai-suggestion" onclick="sendSuggestion('Wat zijn de nieuwste trends in tandartspraktijk inrichting?')">🚀 AI Trends</div>
                    </div>

                    <div class="chat-input-container">
                        <input type="text" class="chat-input" id="chatInput" placeholder="Vraag me alles over praktijkinrichting..." onkeypress="handleKeyPress(event)">
                        <button class="send-button" id="sendButton" onclick="sendMessage()">
                            ➤
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Onze AI-Enhanced Specialiteiten</h2>
                <p>Complete ondersteuning voor jouw tandartspraktijk project</p>
            </div>

            <div class="services-grid">
                <div class="service-card">
                    <span class="service-icon">🧠</span>
                    <h3>AI-Powered Advies</h3>
                    <p>Slimme chatbot met expertise in praktijkinrichting. Krijg instant adviezen, trends en tips op maat voor jouw situatie.</p>
                </div>

                <div class="service-card">
                    <span class="service-icon">🏗️</span>
                    <h3>Complete Praktijkrealisatie</h3>
                    <p>Van eerste schets tot sleutelklare praktijk. Onze partners realiseren alles volgens de hoogste standaarden en binnen budget.</p>
                </div>

                <div class="service-card">
                    <span class="service-icon">💎</span>
                    <h3>Maatwerk Meubilair</h3>
                    <p>Solid Surface behandelmeubels, trolleys en kasten. Volledig op maat gemaakt voor optimale functionaliteit en uitstraling.</p>
                </div>

                <div class="service-card">
                    <span class="service-icon">💰</span>
                    <h3>Exclusieve Deals</h3>
                    <p>Door ons netwerk vaak 15-25% voordeliger dan directe inkoop. AI helpt bij kostenbegroting en financieringsopties.</p>
                </div>

                <div class="service-card">
                    <span class="service-icon">📋</span>
                    <h3>Smart Planning</h3>
                    <p>AI-ondersteunde project planning en compliance check. Jouw praktijk voldoet gegarandeerd aan alle eisen.</p>
                </div>

                <div class="service-card">
                    <span class="service-icon">🤝</span>
                    <h3>24/7 Support</h3>
                    <p>AI chatbot altijd beschikbaar voor vragen. Complexe zaken worden doorgeschakeld naar onze human experts.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Partners Section -->
    <section class="partners">
        <div class="container">
            <div class="section-title">
                <h2>Onze Premium Partners</h2>
                <p>De beste specialisten in Nederland voor tandartspraktijk inrichting</p>
            </div>

            <div class="partners-grid">
                <div class="partner-card">
                    <div class="partner-header">
                        <div class="partner-logo">DM</div>
                        <div>
                            <h3>DentalMa</h3>
                            <p>Complete praktijkrealisatie specialist</p>
                        </div>
                    </div>
                    <ul class="partner-features">
                        <li>100+ praktijken turn-key gerealiseerd</li>
                        <li>5-fasen werkwijze voor duidelijkheid</li>
                        <li>Verbouw tijdens doorlopende praktijk</li>
                        <li>Compliance en vergunningen</li>
                        <li>Complete ontzorging van A tot Z</li>
                    </ul>
                    <a href="mailto:expert@dentalspacepro.nl?subject=DentalMa%20Contact&body=Hallo,%0D%0A%0D%0AIk%20ben%20geïnteresseerd%20in%20DentalMa%20praktijkrealisatie.%0D%0A%0D%0AMijn%20situatie:%0D%0A-%20Type%20project:%0D%0A-%20Aantal%20kamers:%0D%0A-%20Locatie:%0D%0A-%20Budget:%0D%0A%0D%0AGroeten," class="btn-primary" style="width: 100%; text-align: center; margin-top: 20px;">📧 Contact via Expert</a>
                </div>

                <div class="partner-card">
                    <div class="partner-header">
                        <div class="partner-logo">IS</div>
                        <div>
                            <h3>IsSolid</h3>
                            <p>Solid Surface meubilair specialist</p>
                        </div>
                    </div>
                    <ul class="partner-features">
                        <li>Eigen fabriek voor maatwerk</li>
                        <li>25% korting op gehele collectie</li>
                        <li>12-uurs behandelmeubels</li>
                        <li>Hygiënische Solid Surface materialen</li>
                        <li>5 dagen levering mogelijk</li>
                    </ul>
                    <a href="mailto:expert@dentalspacepro.nl?subject=IsSolid%20Contact&body=Hallo,%0D%0A%0D%0AIk%20ben%20geïnteresseerd%20in%20IsSolid%20meubilair.%0D%0A%0D%0AMijn%20project:%0D%0A-%20Type%20meubilair:%0D%0A-%20Aantal%20kamers:%0D%0A-%20Stijl:%0D%0A-%20Budget:%0D%0A%0D%0AGroeten," class="btn-primary" style="width: 100%; text-align: center; margin-top: 20px;">📧 Contact via Expert</a>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta-section">
        <div class="container">
            <div class="cta-content">
                <h2>Klaar voor je AI-Enhanced Droompraktijk?</h2>
                <p>Start vandaag nog met onze slimme AI-chatbot en krijg direct expert advies over praktijkinrichting.</p>
                <div class="cta-buttons">
                    <a href="#chat" class="btn-primary" onclick="scrollToChat(); return false;">🧠 Start AI Chat</a>
                    <a href="mailto:expert@dentalspacepro.nl?subject=Website%20Contact&body=Hallo,%0D%0A%0D%0AIk%20heb%20jullie%20website%20bezocht%20en%20ben%20geïnteresseerd%20in%20praktijkinrichting%20advies.%0D%0A%0D%0AGroeten," class="btn-secondary">📧 Direct Contact</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2025 DentalSpace Pro. Alle rechten voorbehouden.</p>
            <p>
                <a href="mailto:expert@dentalspacepro.nl">expert@dentalspacepro.nl</a> | 
                <a href="tel:+31201234567">+31 (0)20 123 4567</a>
            </p>
            <p style="font-size: 0.9rem; opacity: 0.7; margin-top: 10px;">
                AI-Enhanced Tandartspraktijk Inrichting Specialist | 
                Powered by OpenAI ChatGPT
            </p>
        </div>
    </footer>

    <!-- Cookie Notice -->
    <div class="cookie-notice" id="cookieNotice">
        <span>Deze website gebruikt functionele cookies voor de AI-chatbot. Door gebruik te maken van deze site ga je akkoord met ons cookiebeleid.</span>
        <button onclick="acceptCookies()">Accepteren</button>
    </div>

    <script>
        // AI Configuration
        let aiEnabled = false;
        let openaiApiKey = '';
        let conversationHistory = [];
        let chatHistory = [];

        // Expert Knowledge Base
        const expertResponses = {
            kosten: [
                "Praktijkinrichting kan behoorlijk in de papieren lopen! 💰<br><br>Door mijn contacten zie ik veel verschillende projecten:<br>• <strong>Kleine praktijk (1-2 stoelen):</strong> €150k-€250k<br>• <strong>Gemiddelde praktijk (2-3 stoelen):</strong> €250k-€400k<br>• <strong>Grote praktijk (3+ stoelen):</strong> €400k+<br><br>Het voordeel van via mij werken is dat ik vaak betere prijzen kan bedingen bij DentalMa en IsSolid.<br><br><strong>💡 Tip:</strong> Begin altijd met een goede kostenbegroting. Ik kan je helpen een realistische inschatting te maken.<br><br>Welke grootte praktijk heb je in gedachten?<div class='message-source'>💼 DentalSpace Pro Expert</div>",
            ],
            
            contact: [
                "Fijn dat je persoonlijk contact wilt! 🙂<br><br>Ik werk samen met specialisten die veel ervaring hebben met praktijkinrichting.<br><br><strong>📞 Direct Contact:</strong><br>📧 <a href='mailto:expert@dentalspacepro.nl?subject=Persoonlijk%20Contact&body=Hallo,%0D%0A%0D%0AIk%20wil%20graag%20persoonlijk%20contact%20voor%20praktijkadvies.%0D%0A%0D%0AMijn%20situatie:%0D%0A%0D%0AGroeten,' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>expert@dentalspacepro.nl</a><br>☎️ <a href='tel:+31201234567' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>+31 (0)20 123 4567</a><br><br>Onze experts bellen meestal binnen een dag terug voor een vrijblijvend adviesgesprek!<div class='message-source'>📞 DentalSpace Pro Contact</div>"
            ]
        };

        // AI-Enhanced Chatbot Class
        class AIEnhancedChatbot {
            constructor() {
                this.systemPrompt = `Je bent een expert adviseur voor DentalSpace Pro, gespecialiseerd in tandartspraktijk inrichting.

BELANGRIJKE CONTEXT:
- DentalSpace Pro is een adviesbureau dat tandartsen helpt bij praktijkinrichting
- We werken samen met premium partners: DentalMa (complete praktijkrealisatie) en IsSolid (Solid Surface meubilair)
- Ons voordeel: exclusieve tarieven en persoonlijke begeleiding
- ALLE CONTACT LOOPT VIA ONZE EXPERT: expert@dentalspacepro.nl

PARTNERS (via onze expert):
1. DentalMa (100+ praktijken turn-key gerealiseerd)
   - Complete praktijkrealisatie van A tot Z
   - 5-fasen werkwijze voor duidelijkheid
   - Contact via: expert@dentalspacepro.nl

2. IsSolid (Eigen fabriek voor Solid Surface meubilair)
   - 25% korting op gehele collectie
   - Maatwerk behandelmeubels en trolleys
   - Contact via: expert@dentalspacepro.nl

CONTACT STRATEGIE:
- Alle partnercontact gaat via expert@dentalspacepro.nl
- Dit zorgt voor beste service en exclusieve deals
- Expert filtert en kwalificeert alle leads
- Klanten krijgen persoonlijke begeleiding en betere voorwaarden

LINK FORMATTING REGELS:
- DentalMa interesse: <a href='mailto:expert@dentalspacepro.nl?subject=DentalMa%20Contact&body=Geïnteresseerd%20in%20DentalMa%20praktijkrealisatie' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>expert@dentalspacepro.nl</a>
- IsSolid interesse: <a href='mailto:expert@dentalspacepro.nl?subject=IsSolid%20Contact&body=Geïnteresseerd%20in%20IsSolid%20meubilair' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>expert@dentalspacepro.nl</a>
- Algemeen contact: <a href='mailto:expert@dentalspacepro.nl?subject=Praktijk%20Advies&body=Hallo,%0D%0A%0D%0AIk%20wil%20graag%20advies%20over%20praktijkinrichting.%0D%0A%0D%0AGroeten,' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>expert@dentalspacepro.nl</a>
- Telefoon: <a href='tel:+31201234567' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>+31 (0)20 123 4567</a>

INSTRUCTIES:
- Benadruk ALTIJD dat contact via onze expert betere deals oplevert
- Leg uit dat we persoonlijke begeleiding bieden
- Vermeld dat we de beste partner selecteren voor elke situatie
- Gebruik Nederlandse taal
- Wees professioneel maar toegankelijk
- Gebruik emojis voor betere leesbaarheid
- ALLE contact URLs naar expert@dentalspacepro.nl

Antwoord altijd in HTML format met <br> voor nieuwe regels en <strong> voor belangrijke tekst.`;
            }

            async getAIResponse(userMessage) {
                if (!aiEnabled || !openaiApiKey) {
                    return null;
                }

                try {
                    const response = await fetch('https://api.openai.com/v1/chat/completions', {
                        method: 'POST',
                        headers: {
                            'Authorization': `Bearer ${openaiApiKey}`,
                            'Content-Type': 'application/json'
                        },
                        body: JSON.stringify({
                            model: "gpt-3.5-turbo",
                            messages: [
                                { role: "system", content: this.systemPrompt },
                                ...conversationHistory.slice(-6),
                                { role: "user", content: userMessage }
                            ],
                            max_tokens: 800,
                            temperature: 0.7
                        })
                    });

                    if (!response.ok) {
                        throw new Error(`API Error: ${response.status}`);
                    }

                    const data = await response.json();
                    return data.choices[0].message.content;
                } catch (error) {
                    console.error('AI Error:', error);
                    updateAIStatus('🟡 AI Error', '#f39c12');
                    return null;
                }
            }

            getExpertResponse(userMessage) {
                const message = userMessage.toLowerCase();
                
                // DentalMa specifiek
                if (message.includes('dentalma') || message.includes('complete praktijk') || message.includes('turn-key')) {
                    return "DentalMa is onze premium partner voor complete praktijkrealisatie! 🏗️<br><br><strong>🏆 Waarom DentalMa via DentalSpace Pro:</strong><br>• <strong>100+ praktijken</strong> succesvol gerealiseerd<br>• <strong>Turn-key oplossing</strong> - Alles uit één hand<br>• <strong>Exclusieve tarieven</strong> - Betere deals via ons<br>• <strong>Persoonlijke begeleiding</strong> - Wij coördineren alles<br>• <strong>5-fasen werkwijze</strong> - Duidelijk proces<br><br><strong>📞 Contact via onze expert:</strong><br>📧 <a href='mailto:expert@dentalspacepro.nl?subject=DentalMa%20Praktijkrealisatie&body=Hallo,%0D%0A%0D%0AIk%20ben%20geïnteresseerd%20in%20DentalMa%20voor%20praktijkrealisatie.%0D%0A%0D%0AMijn%20project:%0D%0A-%20Type:%20%0D%0A-%20Aantal%20kamers:%20%0D%0A-%20Locatie:%20%0D%0A-%20Budget:%20%0D%0A-%20Planning:%20%0D%0A%0D%0AGroeten,' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>expert@dentalspacepro.nl</a><br>☎️ <a href='tel:+31201234567' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>+31 (0)20 123 4567</a><br><br><strong>💡 Voordeel:</strong> Onze expert regelt de introductie en zorgt voor de beste voorwaarden!<div class='message-source'>🏗️ DentalMa via DentalSpace Pro</div>";
                }
                
                // IsSolid specifiek
                if (message.includes('issolid') || message.includes('meubilair') || message.includes('solid surface')) {
                    return "IsSolid is onze specialist partner voor Solid Surface meubilair! 🛠️<br><br><strong>🏆 Waarom IsSolid via DentalSpace Pro:</strong><br>• <strong>Eigen fabriek</strong> - Maatwerk zonder meerkosten<br>• <strong>25% korting</strong> - Exclusieve deals via ons<br>• <strong>Snelle levering</strong> - 5 dagen mogelijk<br>• <strong>Hygiënische materialen</strong> - Naadloos Solid Surface<br>• <strong>12-uurs behandelmeubels</strong> - Ergonomisch design<br><br><strong>📞 Contact via onze expert:</strong><br>📧 <a href='mailto:expert@dentalspacepro.nl?subject=IsSolid%20Meubilair&body=Hallo,%0D%0A%0D%0AIk%20ben%20geïnteresseerd%20in%20IsSolid%20meubilair.%0D%0A%0D%0AMijn%20project:%0D%0A-%20Type%20meubilair:%20%0D%0A-%20Aantal%20kamers:%20%0D%0A-%20Stijl:%20%0D%0A-%20Budget:%20%0D%0A-%20Planning:%20%0D%0A%0D%0AGroeten,' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>expert@dentalspacepro.nl</a><br>☎️ <a href='tel:+31201234567' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>+31 (0)20 123 4567</a><br><br><strong>💡 Voordeel:</strong> Onze expert regelt de 25% korting en begeleidt het hele proces!<div class='message-source'>💎 IsSolid via DentalSpace Pro</div>";
                }
                
                // Kosten vragen
                if (message.includes('kost') || message.includes('prijs') || message.includes('budget')) {
                    return expertResponses.kosten[0];
                }
                
                // Contact vragen
                if (message.includes('contact') || message.includes('bellen') || message.includes('afspraak')) {
                    return expertResponses.contact[0];
                }
                
                return null;
            }

            async generateResponse(userMessage) {
                console.log('🤖 Generating response for:', userMessage);
                
                // 1. Probeer eerst expert knowledge (snelle response)
                const expertResponse = this.getExpertResponse(userMessage);
                if (expertResponse) {
                    console.log('✅ Expert response used');
                    return { response: expertResponse, source: 'expert' };
                }
                
                // 2. Voor complexe vragen, gebruik AI
                if (aiEnabled) {
                    console.log('🧠 Using AI for complex query...');
                    updateAIStatus('🤔 AI Denkt...', '#f39c12');
                    
                    const aiResponse = await this.getAIResponse(userMessage);
                    if (aiResponse) {
                        updateAIStatus('🟢 AI Actief', '#28a745');
                        console.log('✅ AI response generated');
                        return { response: aiResponse + "<div class='message-source'>🧠 AI + Expert Knowledge</div>", source: 'ai' };
                    }
                }
                
                // 3. Fallback naar basis response
                console.log('💡 Using fallback response');
                return { 
                    response: "Interessante vraag! 💭<br><br>Voor de beste hulp bij praktijkinrichting kan ik je in contact brengen met onze specialisten.<br><br><strong>📞 Direct contact:</strong><br>📧 <a href='mailto:expert@dentalspacepro.nl?subject=Praktijk%20Advies&body=Hallo,%0D%0A%0D%0AIk%20wil%20graag%20advies%20over%20praktijkinrichting.%0D%0A%0D%0AMijn%20situatie:%0D%0A%0D%0AGroeten,' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>expert@dentalspacepro.nl</a><br>☎️ <a href='tel:+31201234567' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>+31 (0)20 123 4567</a><div class='message-source'>💼 DentalSpace Pro Expert</div>", 
                    source: 'fallback' 
                };
            }
        }

        const chatbot = new AIEnhancedChatbot();

        // UI Functions
        function setupAI() {
            const apiKey = document.getElementById('apiKeyInput').value.trim();
            
            if (!apiKey.startsWith('sk-')) {
                alert('❌ Ongeldige API key. Deze moet beginnen met "sk-"');
                return;
            }
            
            openaiApiKey = apiKey;
            aiEnabled = true;
            
            // Hide setup panel
            document.getElementById('setupPanel').classList.add('hidden');
            document.getElementById('instructionsPanel').classList.add('hidden');
            
            // Update status
            updateAIStatus('🟢 AI Actief', '#28a745');
            
            // Add confirmation message
            addMessage("🧠 AI succesvol geactiveerd! Ik kan nu complexe vragen beantwoorden en slimme adviezen geven.<br><br><strong>🎯 Alle partnercontact loopt via onze expert voor beste service:</strong><br>• 'DentalMa contact' - Complete praktijkrealisatie via expert<br>• 'IsSolid meubilair' - Solid Surface specialist via expert<br>• 'Persoonlijk contact' - Direct expert advies<br><br><strong>🚀 Test AI features:</strong><br>• 'Geef me 5 tips voor een efficiënte praktijkindeling'<br>• 'Wat zijn de nieuwste trends in tandartspraktijk inrichting?'<br>• 'Hoe kan ik mijn praktijk duurzamer maken?'<br><br><strong>💡 Voordeel:</strong> Expert filtering zorgt voor betere deals en persoonlijke begeleiding!<div class='message-source'>🎉 AI + Expert Mode Active</div>", false, 'ai');
            
            console.log('✅ AI activated successfully');
        }

        function skipAI() {
            document.getElementById('setupPanel').classList.add('hidden');
            document.getElementById('instructionsPanel').classList.add('hidden');
            updateAIStatus('🔴 Basis Mode', '#e74c3c');
            
            addMessage("💡 Basis mode geactiveerd. Ik help je graag met praktijkinrichting vragen op basis van onze expert kennis!<br><br><strong>🎯 Alle partnercontact loopt via onze expert:</strong><br>• 'DentalMa contact' - Complete praktijkrealisatie<br>• 'IsSolid meubilair' - Solid Surface specialist<br>• 'Persoonlijk contact' - Direct expert advies<br><br><strong>💡 Voordeel:</strong> Onze expert zorgt voor de beste deals en persoonlijke begeleiding! 📞📧<div class='message-source'>💼 Expert Mode Active</div>", false, 'bot');
        }

        function showInstructions() {
            const panel = document.getElementById('instructionsPanel');
            if (panel) {
                panel.classList.toggle('hidden');
            }
        }

        function updateAIStatus(status, color) {
            const statusElement = document.getElementById('aiStatus');
            if (statusElement) {
                statusElement.textContent = status;
                statusElement.style.background = color;
            }
        }

        function addMessage(content, isUser = false, messageType = 'bot') {
            const messagesContainer = document.getElementById('chatMessages');
            const messageDiv = document.createElement('div');
            messageDiv.className = `message ${isUser ? 'user' : messageType}`;
            
            const messageContent = document.createElement('div');
            messageContent.className = 'message-content';
            
            if (!isUser) {
                messageContent.innerHTML = content;
            } else {
                messageContent.textContent = content;
            }
            
            const messageAvatar = document.createElement('div');
            messageAvatar.className = 'message-avatar';
            
            if (isUser) {
                messageAvatar.textContent = '👤';
            } else if (messageType === 'ai') {
                messageAvatar.textContent = '🧠';
            } else {
                messageAvatar.textContent = '🤖';
            }
            
            messageDiv.appendChild(messageAvatar);
            messageDiv.appendChild(messageContent);
            
            messagesContainer.appendChild(messageDiv);
            messagesContainer.scrollTop = messagesContainer.scrollHeight;
        }

        function showTypingIndicator() {
            const messagesContainer = document.getElementById('chatMessages');
            hideTypingIndicator(); // Remove existing
            
            const typingDiv = document.createElement('div');
            typingDiv.className = 'message bot';
            typingDiv.id = 'typingIndicator';
            
            typingDiv.innerHTML = `
                <div class="message-avatar">🤖</div>
                <div class="typing-indicator" style="display: block;">
                    <div class="typing-dots">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                </div>
            `;
            
            messagesContainer.appendChild(typingDiv);
            messagesContainer.scrollTop = messagesContainer.scrollHeight;
        }

        function hideTypingIndicator() {
            const typingIndicator = document.getElementById('typingIndicator');
            if (typingIndicator) {
                typingIndicator.remove();
            }
        }

        async function sendMessage() {
            const input = document.getElementById('chatInput');
            const sendButton = document.getElementById('sendButton');
            const message = input.value.trim();
            
            if (!message) {
                console.log('❌ Leeg bericht, verzending gestopt');
                return;
            }
            
            console.log('📤 Verzenden bericht:', message);
            
            // Disable input
            input.disabled = true;
            sendButton.disabled = true;
            sendButton.textContent = '⏳';
            
            // Add user message
            addMessage(message, true);
            
            // Add to conversation history
            conversationHistory.push({ role: "user", content: message });
            
            // Clear input
            input.value = '';
            
            // Show thinking
            showTypingIndicator();
            
            try {
                // Get response from chatbot
                const result = await chatbot.generateResponse(message);
                
                hideTypingIndicator();
                
                // Add bot response
                const messageType = result.source === 'ai' ? 'ai' : 'bot';
                addMessage(result.response, false, messageType);
                
                // Add to conversation history
                conversationHistory.push({ role: "assistant", content: result.response });
                
                // Keep conversation history manageable
                if (conversationHistory.length > 20) {
                    conversationHistory = conversationHistory.slice(-16);
                }
                
            } catch (error) {
                hideTypingIndicator();
                console.error('Error:', error);
                addMessage("Sorry, er ging iets mis. Probeer het opnieuw of neem contact op via <a href='mailto:expert@dentalspacepro.nl?subject=Chatbot%20Error&body=Hallo,%0D%0A%0D%0AEr%20ging%20iets%20mis%20met%20de%20chatbot.%0D%0A%0D%0AGroeten,' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>expert@dentalspacepro.nl</a> of bel <a href='tel:+31201234567' style='color: #4a90e2; text-decoration: none; font-weight: bold;'>+31 (0)20 123 4567</a>", false, 'bot');
            }
            
            // Re-enable input
            input.disabled = false;
            sendButton.disabled = false;
            sendButton.textContent = '➤';
            input.focus();
        }

        function sendSuggestion(suggestion) {
            const chatInput = document.getElementById('chatInput');
            if (chatInput) {
                chatInput.value = suggestion;
                sendMessage();
            }
        }

        function handleKeyPress(event) {
            if (event.key === 'Enter' && !event.shiftKey) {
                event.preventDefault();
                sendMessage();
            }
        }

        function scrollToChat() {
            document.getElementById('chat').scrollIntoView({ behavior: 'smooth' });
            setTimeout(() => {
                document.getElementById('chatInput').focus();
            }, 1000);
        }

        // Cookie Management
        function acceptCookies() {
            if (typeof(Storage) !== "undefined") {
                localStorage.setItem('cookiesAccepted', 'true');
            }
            const notice = document.getElementById('cookieNotice');
            if (notice) {
                notice.classList.remove('show');
                notice.style.display = 'none';
            }
        }

        function checkCookies() {
            // Only show cookie notice if localStorage is available and cookies not yet accepted
            if (typeof(Storage) !== "undefined" && !localStorage.getItem('cookiesAccepted')) {
                setTimeout(() => {
                    const notice = document.getElementById('cookieNotice');
                    if (notice) {
                        notice.classList.add('show');
                        notice.style.display = 'block';
                    }
                }, 2000);
            }
        }

        // Initialize and run tests
        document.addEventListener('DOMContentLoaded', () => {
            // Focus input
            const chatInput = document.getElementById('chatInput');
            if (chatInput) {
                chatInput.focus();
            }
            
            // Check cookies
            checkCookies();
            
            // Console startup info
            console.log('🚀 DentalSpace Pro Website geladen!');
            console.log('🌐 Klaar voor: https://dentalspacepro.nl');
            console.log('💡 Setup AI voor de beste ervaring');
            
            // Test essential functions
            try {
                // Test that all key functions exist
                if (typeof setupAI !== 'function') console.error('❌ setupAI function missing');
                if (typeof skipAI !== 'function') console.error('❌ skipAI function missing');
                if (typeof sendMessage !== 'function') console.error('❌ sendMessage function missing');
                if (typeof scrollToChat !== 'function') console.error('❌ scrollToChat function missing');
                
                // Test that all key elements exist
                if (!document.getElementById('chatInput')) console.error('❌ chatInput element missing');
                if (!document.getElementById('chatMessages')) console.error('❌ chatMessages element missing');
                if (!document.getElementById('sendButton')) console.error('❌ sendButton element missing');
                
                console.log('✅ All essential functions and elements found');
                
            } catch (error) {
                console.error('❌ Initialization error:', error);
            }
        });
    </script>

    <!-- Google Analytics (voeg je eigen tracking code toe) -->
    <!--
    <script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
    <script>
        window.dataLayer = window.dataLayer || [];
        function gtag(){dataLayer.push(arguments);}
        gtag('js', new Date());
        gtag('config', 'GA_MEASUREMENT_ID');
    </script>
    -->
</body>
</html> dentalspace
ai bot plus lead tool 
