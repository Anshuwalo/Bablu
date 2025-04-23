<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Arya ❤️</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #ffcdd2, #f8bbd0, #e1bee7);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            margin: 0;
            padding: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            text-align: center;
        }

        @keyframes gradientBG {
            0% {background-position: 0% 50%;}
            50% {background-position: 100% 50%;}
            100% {background-position: 0% 50%;}
        }

        .container {
            max-width: 800px;
            padding: 30px;
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            position: relative;
            overflow: hidden;
            transform: scale(0.98);
            animation: pulse 3s infinite alternate;
        }

        @keyframes pulse {
            from {transform: scale(0.98); box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);}
            to {transform: scale(1); box-shadow: 0 15px 40px rgba(255, 64, 129, 0.4);}
        }

        h1 {
            color: #ff4081;
            margin-bottom: 20px;
            font-size: 32px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
            position: relative;
            display: inline-block;
        }

        h1::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 3px;
            bottom: -10px;
            left: 0;
            background: linear-gradient(to right, transparent, #ff4081, transparent);
        }

        p {
            font-size: 18px;
            line-height: 1.6;
            color: #333;
            margin-bottom: 20px;
        }

        .letter {
            background-color: #fff5f7;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(255, 64, 129, 0.2);
            margin: 30px 0;
            position: relative;
            font-family: 'Georgia', serif;
            font-size: 16px;
            line-height: 1.8;
            text-align: left;
            max-height: 300px;
            overflow-y: auto;
            display: none;
            border: 1px solid #ffcdd2;
        }

        .letter:before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, transparent 50%, #ff4081 50%);
            border-radius: 0 0 0 10px;
        }

        .btn {
            display: inline-block;
            padding: 12px 40px;
            margin: 15px;
            font-size: 18px;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            border: none;
            outline: none;
            font-weight: bold;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

        .btn-yes {
            background: linear-gradient(to right, #ff4081, #f50057);
            color: white;
        }

        .btn-no {
            background: linear-gradient(to right, #9e9e9e, #757575);
            color: white;
            position: relative;
        }

        .btn-yes:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 20px rgba(255, 64, 129, 0.4);
        }

        .hearts {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
            top: 0;
            left: 0;
            pointer-events: none;
            display: none;
        }

        .heart {
            position: absolute;
            font-size: 20px;
            color: #ff4081;
            animation: float 6s ease-in infinite;
            opacity: 0;
        }

        @keyframes float {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 0.5;
            }
            100% {
                transform: translateY(-800px) rotate(360deg);
                opacity: 0;
            }
        }

        .proposal-question, .response-message, .buttons-container {
            display: none;
        }

        .page {
            display: none;
        }

        #page1 {
            display: block;
        }

        .next-btn {
            background: linear-gradient(to right, #ff4081, #f50057);
            color: white;
            padding: 12px 30px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-size: 16px;
            margin-top: 20px;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

        .next-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(255, 64, 129, 0.4);
        }
        
        .response-message {
            font-size: 28px;
            color: #ff4081;
            font-weight: bold;
            margin: 30px 0;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.1);
        }

        .intro-image {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            margin: 20px auto;
            border: 5px solid white;
            box-shadow: 0 0 20px rgba(255, 64, 129, 0.3);
            animation: float-gentle 3s ease-in-out infinite alternate;
        }

        @keyframes float-gentle {
            from {transform: translateY(0);}
            to {transform: translateY(-15px);}
        }

        .envelope {
            width: 100px;
            height: 60px;
            background-color: #f50057;
            position: relative;
            margin: 20px auto;
            cursor: pointer;
            transition: all 0.3s ease;
            transform-style: preserve-3d;
        }

        .envelope-flap {
            width: 0;
            height: 0;
            border-left: 50px solid transparent;
            border-right: 50px solid transparent;
            border-bottom: 40px solid #f50057;
            position: absolute;
            top: -39px;
            left: 0;
            transform-origin: bottom;
            transition: transform 0.4s ease-in-out;
            z-index: 3;
        }

        .envelope:hover .envelope-flap {
            transform: rotateX(180deg);
        }

        .envelope-body {
            width: 100%;
            height: 100%;
            background-color: #ff4081;
            position: relative;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            font-weight: bold;
        }

        .flowers {
            position: absolute;
            bottom: -20px;
            width: 100%;
            display: flex;
            justify-content: space-around;
            z-index: -1;
        }

        .flower {
            font-size: 30px;
            animation: grow 3s ease-in-out infinite alternate;
        }

        @keyframes grow {
            from {transform: scale(0.8) translateY(0);}
            to {transform: scale(1.1) translateY(-15px);}
        }

        .confetti {
            position: absolute;
            width: 10px;
            height: 10px;
            background-color: #ff4081;
            opacity: 0;
        }

        @keyframes confettiDrop {
            0% {
                transform: translateY(-100vh) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(100vh) rotate(360deg);
                opacity: 0;
            }
        }

        .music-note {
            font-size: 24px;
            position: absolute;
            opacity: 0;
            animation: float-music 4s linear forwards;
        }

        @keyframes float-music {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 0.7;
            }
            100% {
                transform: translateY(-100px) rotate(20deg);
                opacity: 0;
            }
        }
        
        .proposal-animation {
            margin: 20px auto;
            height: 150px;
            position: relative;
        }
        
        .boy-figure {
            position: absolute;
            left: 30%;
            bottom: 0;
            font-size: 60px;
            transform: translateX(-50%);
        }
        
        .girl-figure {
            position: absolute;
            right: 30%;
            bottom: 0;
            font-size: 60px;
            transform: translateX(50%);
        }
        
        .flower-offer {
            position: absolute;
            left: 50%;
            bottom: 50px;
            font-size: 30px;
            transform: translateX(-50%);
            opacity: 0;
            animation: flower-appear 2s ease-in-out infinite;
        }
        
        @keyframes flower-appear {
            0% { opacity: 0; transform: translateX(-50%) translateY(20px); }
            50% { opacity: 1; transform: translateX(-50%) translateY(0); }
            100% { opacity: 0; transform: translateX(-50%) translateY(-20px); }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Page 1 - Initial greeting -->
        <div id="page1" class="page">
            <h1>💖 Dear Arya 💖</h1>
            <p>There's something I've been wanting to tell you... 🥰</p>
            <div class="flowers">
                <div class="flower">🌹</div>
                <div class="flower" style="animation-delay: 0.5s">🌷</div>
                <div class="flower" style="animation-delay: 1s">🌸</div>
                <div class="flower" style="animation-delay: 1.5s">🌹</div>
                <div class="flower" style="animation-delay: 2s">🌷</div>
            </div>
            <button class="next-btn" onclick="showPage('page2')">Continue ❤️</button>
        </div>

        <!-- Page 2 - Letter -->
        <div id="page2" class="page">
            <h1>I wanted to say something to you 💌</h1>
            <div class="envelope" onclick="openLetter()">
                <div class="envelope-flap"></div>
                <div class="envelope-body">For You</div>
            </div>
            <div class="letter" id="letter">
                Dear Arya,<br><br>
                
                We've met, we've shared some beautiful moments, and honestly, I wanted to say all of this to you when we met. But you know na, sometimes words get stuck, and heartbeats get louder than voices.<br><br>
                
               But feelings are feelings — it doesn't matter if they're expressed in person or through a few clumsy sentences here. What matters is that they come straight from the heart.<br><br>
                
                Every single moment I've spent talking to you has been the best part of my day. Your crazy witch-like laugh, your sudden cute tantrums, your random deep talks, your "I'm annoyed" face — everything about you is just… my favorite. And yes, you are my favorite too.<br><br>
                
               No matter how my day goes — good, bad, or complete disaster — the moment I talk to you, everything feels right again. Just looking at you makes me happy. Talking to you gives me peace. And honestly, I don't want anyone else getting that place in your life.<br><br>
                
                I want to be the one to see you, hear you, and be with you — every single day. Even if you drive me crazy sometimes, it's still you I want to be crazy about.<br><br>
                
                And listen carefully — no matter what happens, no matter how things change, I promise I'll always be there for you. Laughing with you, arguing with you, supporting you, and standing by you — every single time.<br><br>
                
                Arya, I love you.
            </div>
            <button class="next-btn" id="letter-continue-btn" style="display:none;" onclick="showPage('page3')">Continue ❤️</button>
        </div>

        <!-- Page 3 - First Proposal -->
        <div id="page3" class="page">
            <div class="proposal-animation">
                <div class="boy-figure">👦</div>
                <div class="flower-offer">🌹</div>
                <div class="girl-figure">👧</div>
            </div>
            <h1 class="proposal-question">Arya, will you be my girlfriend? 💘</h1>
            <div class="buttons-container">
                <button class="btn btn-yes" onclick="acceptProposal()">Yes</button>
                <button class="btn btn-no" onclick="showPage('page4')">No</button>
            </div>
        </div>
        
        <!-- Page 4 - Second Proposal (Seriously?) -->
        <div id="page4" class="page">
            <h1>Seriously? 😕</h1>
            <p>Acchese soch le, phirse puch rha hu... 🤔</p>
            <h1 class="proposal-question">Arya, will you be my girlfriend? 💖</h1>
            <div class="buttons-container">
                <button class="btn btn-yes" onclick="acceptProposal()">Yes</button>
                <button class="btn btn-no" onclick="showPage('page5')">No</button>
            </div>
        </div>
        
        <!-- Page 5 - Final Proposal (Please) -->
        <div id="page5" class="page">
            <h1>Please Arya manjaa! 🥺</h1>
            <p>Aakhri baar puch rha hu... 🙏</p>
            <h1 class="proposal-question">Arya, will you be my gf? ❤️</h1>
            <div class="buttons-container">
                <button class="btn btn-yes" onclick="acceptProposal()">Yes</button>
                <button class="btn btn-no" id="noButton" onmouseover="moveButton()">No</button>
            </div>
        </div>
        
        <!-- Final Success Page -->
        <div id="final-page" class="page">
            <h1>Haha, finally! 🎉</h1>
            <div class="emoji-decoration" style="font-size: 60px;">💑</div>
            <p>You are my girlfriend now! Love you so much! ❤️❤️❤️</p>
            <div id="music-container"></div>
            <div class="hearts" id="hearts"></div>
        </div>
    </div>

    <script>
        function showPage(pageId) {
            // Hide all pages
            document.querySelectorAll('.page').forEach(page => {
                page.style.display = 'none';
            });
            
            // Show the selected page
            document.getElementById(pageId).style.display = 'block';
            
            // If page3, page4, or page5, show proposal question and buttons
            if (pageId === 'page3' || pageId === 'page4' || pageId === 'page5') {
                if (document.querySelector('#' + pageId + ' .proposal-question')) {
                    document.querySelector('#' + pageId + ' .proposal-question').style.display = 'block';
                }
                if (document.querySelector('#' + pageId + ' .buttons-container')) {
                    document.querySelector('#' + pageId + ' .buttons-container').style.display = 'block';
                }
                
                // Add some music notes animation
                createMusicNotes();
            }
        }
        
        function openLetter() {
            document.getElementById('letter').style.display = 'block';
            document.querySelector('.envelope').style.display = 'none';
            document.getElementById('letter-continue-btn').style.display = 'block';
        }
        
        function moveButton() {
            const noButton = document.getElementById('noButton');
            const container = document.querySelector('.container');
            
            // Get container dimensions
            const containerWidth = container.offsetWidth - 100;
            const containerHeight = container.offsetHeight - 50;
            
            // Generate random position
            const randomX = Math.floor(Math.random() * containerWidth);
            const randomY = Math.floor(Math.random() * containerHeight);
            
            // Set new position
            noButton.style.position = 'absolute';
            noButton.style.left = randomX + 'px';
            noButton.style.top = randomY + 'px';
        }
        
        function acceptProposal() {
            // Show final page
            showPage('final-page');
            
            // Show hearts
            document.getElementById('hearts').style.display = 'block';
            
            // Create floating hearts and confetti
            createHearts();
            createConfetti();
        }
        
        function createHearts() {
            const heartsContainer = document.getElementById('hearts');
            const numberOfHearts = 50;
            
            for (let i = 0; i < numberOfHearts; i++) {
                setTimeout(() => {
                    const heart = document.createElement('div');
                    heart.classList.add('heart');
                    heart.innerHTML = '❤️';
                    
                    // Random position and size
                    const leftPos = Math.floor(Math.random() * 100);
                    const size = Math.floor(Math.random() * 20) + 10;
                    const delay = Math.random() * 5;
                    const duration = Math.random() * 5 + 5;
                    
                    heart.style.left = leftPos + '%';
                    heart.style.fontSize = size + 'px';
                    heart.style.animationDelay = delay + 's';
                    heart.style.animationDuration = duration + 's';
                    
                    heartsContainer.appendChild(heart);
                    
                    // Remove after animation
                    setTimeout(() => {
                        heart.remove();
                    }, duration * 1000);
                }, i * 150);
            }
        }
        
        function createConfetti() {
            const container = document.querySelector('.container');
            const confettiCount = 100;
            
            for (let i = 0; i < confettiCount; i++) {
                const confetti = document.createElement('div');
                confetti.classList.add('confetti');
                
                // Random properties
                const size = Math.floor(Math.random() * 10) + 5;
                const left = Math.floor(Math.random() * 100);
                const delay = Math.random() * 5;
                const duration = Math.random() * 3 + 3;
                const colors = ['#ff4081', '#ff80ab', '#f50057', '#c51162', '#ffcdd2', '#ffebee'];
                const color = colors[Math.floor(Math.random() * colors.length)];
                
                confetti.style.width = size + 'px';
                confetti.style.height = size + 'px';
                confetti.style.left = left + '%';
                confetti.style.backgroundColor = color;
                confetti.style.animation = `confettiDrop ${duration}s ease-in forwards`;
                confetti.style.animationDelay = delay + 's';
                
                container.appendChild(confetti);
                
                // Remove after animation
                setTimeout(() => {
                    confetti.remove();
                }, (delay + duration) * 1000);
            }
        }
        
        function createMusicNotes() {
            const container = document.querySelector('.container');
            const musicNotes = ['♪', '♫', '🎵', '🎶'];
            const noteCount = 15;
            
            for (let i = 0; i < noteCount; i++) {
                setTimeout(() => {
                    const note = document.createElement('div');
                    note.classList.add('music-note');
                    
                    // Random properties
                    const noteChar = musicNotes[Math.floor(Math.random() * musicNotes.length)];
                    const left = Math.floor(Math.random() * 80) + 10;
                    const delay = Math.random() * 2;
                    const duration = Math.random() * 2 + 2;
                    
                    note.innerHTML = noteChar;
                    note.style.left = left + '%';
                    note.style.bottom = '20px';
                    note.style.animation = `float-music ${duration}s linear forwards`;
                    note.style.animationDelay = delay + 's';
                    
                    container.appendChild(note);
                    
                    // Remove after animation
                    setTimeout(() => {
                        note.remove();
                    }, (delay + duration) * 1000);
                }, i * 200);
            }
        }
        
        // Create some initial music notes for the first page
        window.onload = function() {
            setTimeout(() => {
                const container = document.querySelector('.container');
                const musicNotes = ['♪', '♫', '🎵', '🎶'];
                
                for (let i = 0; i < 5; i++) {
                    const note = document.createElement('div');
                    note.classList.add('music-note');
                    
                    const noteChar = musicNotes[Math.floor(Math.random() * musicNotes.length)];
                    const left = Math.floor(Math.random() * 80) + 10;
                    const delay = Math.random() * 2;
                    const duration = Math.random() * 2 + 2;
                    
                    note.innerHTML = noteChar;
                    note.style.left = left + '%';
                    note.style.bottom = '20px';
                    note.style.animation = `float-music ${duration}s linear forwards`;
                    note.style.animationDelay = delay + 's';
                    
                    container.appendChild(note);
                    
                    setTimeout(() => {
                        note.remove();
                    }, (delay + duration) * 1000);
                }
            }, 1000);
        };
    </script>
</body>
</html>
