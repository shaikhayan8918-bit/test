<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Executive Fitness Transformation</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);
            min-height: 100vh;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            background: rgba(255, 255, 255, 0.98);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            margin-top: 20px;
            margin-bottom: 20px;
        }
        
        .preheader {
            text-align: center;
            font-size: 14px;
            color: #666;
            margin-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .hero {
            text-align: center;
            margin-bottom: 40px;
            padding: 40px 20px;
            background: linear-gradient(45deg, #ff6b6b, #ff8e53);
            border-radius: 15px;
            color: white;
            box-shadow: 0 15px 35px rgba(255, 107, 107, 0.3);
        }
        
        .hero h1 {
            font-size: 2.8rem;
            font-weight: bold;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.02); }
        }
        
        .hero .subheader {
            font-size: 1.4rem;
            margin-bottom: 30px;
            opacity: 0.95;
        }
        
        .cta-button {
            display: inline-block;
            background: linear-gradient(45deg, #28a745, #20c997);
            color: white;
            padding: 18px 40px;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.2rem;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 1px;
            box-shadow: 0 10px 25px rgba(40, 167, 69, 0.3);
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }
        
        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 35px rgba(40, 167, 69, 0.4);
        }
        
        .section {
            margin-bottom: 50px;
            padding: 30px;
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            border-radius: 15px;
            border-left: 5px solid #ff6b6b;
        }
        
        .section h2 {
            font-size: 2.2rem;
            color: #2c3e50;
            margin-bottom: 25px;
            text-align: center;
            position: relative;
        }
        
        .section h2:after {
            content: '';
            display: block;
            width: 80px;
            height: 3px;
            background: linear-gradient(45deg, #ff6b6b, #ff8e53);
            margin: 15px auto;
            border-radius: 2px;
        }
        
        .section p {
            margin-bottom: 20px;
            font-size: 1.1rem;
            line-height: 1.8;
        }
        
        .highlight {
            background: linear-gradient(120deg, #ff6b6b 0%, #ff8e53 100%);
            color: white;
            padding: 2px 8px;
            border-radius: 4px;
            font-weight: bold;
        }
        
        .bold {
            font-weight: bold;
            color: #2c3e50;
        }
        
        .italic {
            font-style: italic;
            color: #555;
        }
        
        .caps {
            text-transform: uppercase;
            font-weight: bold;
            color: #e74c3c;
        }
        
        .bullets {
            list-style: none;
            padding: 0;
        }
        
        .bullets li {
            margin-bottom: 15px;
            padding-left: 30px;
            position: relative;
            font-size: 1.1rem;
            line-height: 1.7;
        }
        
        .bullets li:before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #28a745;
            font-weight: bold;
            font-size: 1.3rem;
        }
        
        .value-stack {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
        }
        
        .value-stack h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            text-align: center;
        }
        
        .guarantee {
            background: linear-gradient(135deg, #ffecd2 0%, #fcb69f 100%);
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            margin: 30px 0;
            border: 2px solid #ff8e53;
        }
        
        .guarantee h3 {
            color: #d63031;
            margin-bottom: 15px;
            font-size: 1.4rem;
        }
        
        .faq {
            margin-top: 40px;
        }
        
        .faq-item {
            margin-bottom: 25px;
            padding: 20px;
            background: #f8f9fa;
            border-radius: 10px;
            border-left: 4px solid #007bff;
        }
        
        .faq-item h4 {
            color: #2c3e50;
            margin-bottom: 10px;
            font-size: 1.2rem;
        }
        
        .final-cta {
            text-align: center;
            padding: 50px 20px;
            background: linear-gradient(135deg, #2c3e50, #3498db);
            color: white;
            border-radius: 15px;
            margin-top: 40px;
        }
        
        .final-cta h3 {
            font-size: 2rem;
            margin-bottom: 20px;
        }
        
        .urgency {
            background: #e74c3c;
            color: white;
            padding: 15px;
            border-radius: 8px;
            margin: 20px 0;
            text-align: center;
            font-weight: bold;
            animation: blink 2s infinite;
        }
        
        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0.7; }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- HERO SECTION -->
        <div class="preheader">
            For High-Performing Executives, Entrepreneurs & Business Leaders
        </div>
        
        <div class="hero">
            <h1>Drop 20-40 Pounds of Fat & Build Unstoppable Energy in 90 Days</h1>
            <div class="subheader">
                Without sacrificing your career, spending hours in the gym, or following another crash diet that leaves you burned out
            </div>
            <a href="#offer" class="cta-button">Claim Your Transformation Now</a>
        </div>

        <!-- PROBLEM IDENTIFICATION -->
        <div class="section">
            <h2>The High-Performer's Health Crisis That's Sabotaging Your Success</h2>
            
            <p>You're crushing it in the boardroom...</p>
            
            <p>Building businesses. Closing deals. Leading teams.</p>
            
            <p>But every morning, you look in the mirror and see the <span class="bold">cost of your success</span> staring back at you.</p>
            
            <p>The extra 20... 30... even 40 pounds that crept up while you were busy changing the world.</p>
            
            <p>The energy that <span class="italic">used to carry you through 12-hour days</span> now barely gets you to lunch without reaching for another coffee.</p>
            
            <p>You've tried the trendy diets...</p>
            
            <p>Keto lasted 3 weeks before a client dinner derailed everything.</p>
            
            <p>Intermittent fasting worked until your travel schedule made it impossible.</p>
            
            <p>Those 5 AM gym sessions? <span class="caps">Gone</span> the moment your workload doubled.</p>
            
            <p>And now you're caught in the <span class="highlight">high-performer's trap</span>:</p>
            
            <p>The more successful you become, the worse your health gets...</p>
            
            <p>The worse your health gets, the harder it becomes to maintain that success.</p>
            
            <p>But what if I told you there's a way to <span class="bold">break this cycle completely</span>?</p>
        </div>

        <!-- SOLUTION REVELATION -->
        <div class="section">
            <h2>The "Executive Edge" Method That Changes Everything</h2>
            
            <p>Here's what I discovered after working with hundreds of high-performing executives...</p>
            
            <p>The reason every diet and workout plan has failed you isn't because you lack willpower.</p>
            
            <p><span class="bold">It's because they were designed for people who have 2 hours a day to meal prep and work out.</span></p>
            
            <p>Not for someone who's running board meetings, traveling across time zones, and making million-dollar decisions before most people finish their morning coffee.</p>
            
            <p>So I created something different...</p>
            
            <p>A system that works <span class="italic">with</span> your demanding schedule, not against it.</p>
            
            <p><span class="caps">Introducing the Executive Edge Method:</span></p>
            
            <ul class="bullets">
                <li><span class="bold">Strategic Nutrition</span> that fuels peak performance without complicated meal plans or giving up business dinners</li>
                <li><span class="bold">Time-Efficient Training</span> that builds muscle and burns fat in 20-minute sessions that fit between meetings</li>
                <li><span class="bold">Recovery Protocols</span> that turn your sleep into a fat-burning, energy-boosting machine</li>
                <li><span class="bold">Stress-Proof Mindset</span> strategies that prevent burnout from derailing your progress</li>
            </ul>
            
            <p>The result?</p>
            
            <p>You wake up with <span class="highlight">more energy than you've had in years</span>.</p>
            
            <p>Your clothes fit better. Your confidence soars. Your mental clarity is razor-sharp.</p>
            
            <p>And your career? It doesn't just survive your transformation...</p>
            
            <p><span class="caps">It thrives because of it.</span></p>
        </div>

        <!-- PRODUCT INTRODUCTION -->
        <div class="section">
            <h2>Executive Body Transformation: Your Personal Success System</h2>
            
            <p>This isn't another generic fitness program...</p>
            
            <p>It's a <span class="bold">complete lifestyle transformation system</span> built specifically for leaders who refuse to choose between their health and their success.</p>
            
            <p>You get direct access to me as your personal transformation coach...</p>
            
            <p>Plus a proven blueprint that's already helped executives at McKinsey, Amazon, Meta, and Shopify drop 20-45 pounds while <span class="italic">increasing</span> their performance at work.</p>
            
            <div class="value-stack">
                <h3>Here's Everything You Get:</h3>
                
                <ul class="bullets">
                    <li><span class="bold">1-on-1 Coaching Calls</span> - Weekly strategy sessions to keep you on track and adjust your plan as your schedule changes</li>
                    <li><span class="bold">The Executive Nutrition Blueprint</span> - Eat the foods you love while burning fat and building energy (no more restrictive diets)</li>
                    <li><span class="bold">20-Minute Power Workouts</span> - Build muscle and torch fat with workouts that fit in your hotel room or home office</li>
                    <li><span class="bold">Recovery & Sleep Optimization</span> - Turn your rest into your secret weapon for fat loss and peak performance</li>
                    <li><span class="bold">Stress-Proof Protocols</span> - Bulletproof your progress against deadlines, travel, and high-pressure situations</li>
                    <li><span class="bold">24/7 Text Support</span> - Direct line to me when you need quick answers or motivation</li>
                </ul>
            </div>
            
            <p>This is the same system a 52-year-old real estate entrepreneur used to drop 32 pounds while closing his biggest deal ever...</p>
            
            <p>The same approach a 67-year-old executive used to build more muscle at 67 than he had at 47...</p>
            
            <p>And the exact blueprint a busy female consultant used to transform her body and <span class="caps">double her energy</span> in just 12 weeks.</p>
        </div>

        <!-- OFFER STRUCTURE -->
        <div class="section" id="offer">
            <h2>Your Investment in Peak Performance</h2>
            
            <p>Let's be honest...</p>
            
            <p>You've probably spent more on a single business lunch than most people invest in their entire health transformation.</p>
            
            <p>But what's it costing you to stay where you are?</p>
            
            <p>The low energy that's limiting your decision-making ability...</p>
            
            <p>The lack of confidence that's affecting how you show up in important meetings...</p>
            
            <p>The stress and burnout that's threatening everything you've built...</p>
            
            <p><span class="bold">The full Executive Body Transformation program normally costs $5,000.</span></p>
            
            <p>But for the next 24 hours, I'm making it available for just <span class="highlight">$2,997</span>.</p>
            
            <div class="guarantee">
                <h3>🛡️ My Performance Guarantee</h3>
                <p>If you don't see significant improvements in your energy, body composition, and overall performance within 60 days, I'll refund every penny and let you keep all the materials.</p>
            </div>
            
            <div class="urgency">
                ⚠️ Limited to 10 Spots This Month - Only 3 Remaining
            </div>
            
            <div style="text-align: center; margin-top: 30px;">
                <a href="#" class="cta-button">Transform Your Body & Performance Now</a>
            </div>
        </div>

        <!-- FAQ SECTION -->
        <div class="faq">
            <h2>Your Questions Answered</h2>
            
            <div class="faq-item">
                <h4>Q: I barely have time to eat lunch. How can I possibly follow a fitness program?</h4>
                <p>That's exactly WHY this program works. It's designed for people with zero extra time. The workouts take 20 minutes. The nutrition fits your existing lifestyle. And the results come faster because we're not wasting time on inefficient methods.</p>
            </div>
            
            <div class="faq-item">
                <h4>Q: I travel constantly. Will this work with my schedule?</h4>
                <p>Absolutely. I've worked with executives who spend 200+ days a year on the road. The system is built to work in hotel rooms, airport lounges, and conference centers. Your travel schedule becomes an asset, not an obstacle.</p>
            </div>
            
            <div class="faq-item">
                <h4>Q: What if I've tried everything and nothing has worked?</h4>
                <p>Perfect. That means you've eliminated all the methods that DON'T work for high-performers. This system is specifically designed for people who've failed with traditional approaches because they weren't built for your lifestyle.</p>
            </div>
            
            <div class="faq-item">
                <h4>Q: Is this just another online course?</h4>
                <p>Not even close. This is high-touch, personal coaching with direct access to me. You get weekly calls, 24/7 text support, and a completely customized approach. It's like having a personal trainer, nutritionist, and performance coach in your pocket.</p>
            </div>
        </div>

        <!-- FINAL CTA -->
        <div class="final-cta">
            <h3>Your Two Choices</h3>
            
            <p>You can keep doing what you're doing...</p>
            
            <p>Watching your energy decline, your confidence shrink, and your health deteriorate while you tell yourself you'll "figure it out later."</p>
            
            <p>Or...</p>
            
            <p>You can make the same decision that hundreds of other high-performers have made...</p>
            
            <p>To finally put yourself first and build the body and energy that matches your ambition.</p>
            
            <p><span class="bold">The choice is yours.</span></p>
            
            <p>But choose quickly...</p>
            
            <div class="urgency">
                This offer expires in 24 hours
            </div>
            
            <a href="#" class="cta-button" style="margin-top: 20px;">Claim Your Transformation Now</a>
            
            <p style="margin-top: 20px; font-size: 0.9em; opacity: 0.8;">
                Your future self is counting on the decision you make today.
            </p>
        </div>
    </div>
</body>
</html>
