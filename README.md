- 👋 Hi, I’m @PLAYTVGH
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
5-word summary: African map play button logo

![Image][]

Now, let's begin coding the PLAY TV GH app:```html
<!DOCTYPE html><html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PLAY TV GH - African Music Video Streaming</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css">
    <style>
        :root {
            --primary-red: #FF0000;
            --primary-black: #000000;
            --secondary-gray: #333333;
        }

        body {
            background-color: var(--primary-black);
            color: white;
            font-family: 'Arial', sans-serif;
        }

        .logo {
            width: 100px;
            height: 100px;
            background-image: url('https://image.pollinations.ai/prompt/African%20map%20outline%20with%20black%20star%20center%20and%20red%20play%20button%20icon%20minimalist%20vector%20style%20logo%20design?width=400&height=400');
            background-size: cover;
            background-position: center;
        }

        .nav-link {
            position: relative;
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        .nav-link:hover {
            color: var(--primary-red);
        }

        .nav-link::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 2px;
            bottom: -5px;
            left: 0;
            background-color: var(--primary-red);
            transform: scaleX(0);
            transition: transform 0.3s ease;
        }

        .nav-link:hover::after {
            transform: scaleX(1);
        }

        .hero {
            background-image: url('https://picsum.photos/1920/1080?random=1');
            background-size: cover;
            background-position: center;
            height: 70vh;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.5);
        }

        .hero-content {
            z-index: 1;
            text-align: center;
        }

        .btn {
            background-color: var(--primary-red);
            color: white;
            padding: 10px 20px;
            border-radius: 25px;
            text-decoration: none;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .btn:hover {
            background-color: #CC0000;
            transform: scale(1.05);
        }

        .genre-section {
            background-color: var(--secondary-gray);
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 20px;
        }

        .video-card {
            background-color: var(--secondary-gray);
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s ease;
        }

        .video-card:hover {
            transform: translateY(-5px);
        }

        .video-player {
            width: 100%;
            height: 0;
            padding-bottom: 56.25%; /* 16:9 aspect ratio */
            position: relative;
            overflow: hidden;
            border-radius: 10px;
        }

        .video-player iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }

        .share-btn {
            background-color: #25D366; /* WhatsApp green */
            color: white;
            padding: 5px 10px;
            border-radius: 5px;
            margin-right: 5px;
        }

        .share-btn.facebook {
            background-color: #1877F2; /* Facebook blue */
        }

        .share-btn.instagram {
            background: linear-gradient(45deg, #405DE6, #5851DB, #833AB4, #C13584, #E1306C, #FD1D1D);
        }

        @keyframes pulse {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.05);
            }
            100% {
                transform: scale(1);
            }
        }

        .pulse {
            animation: pulse 2s infinite;
        }
    </style>
</head>
<body>
    <header class="bg-black py-4">
        <nav class="container mx-auto flex justify-between items-center">
            <div class="logo"></div>
            <div>
                <a href="#" class="nav-link">Home</a>
                <a href="#" class="nav-link">Genres</a>
                <a href="#" class="nav-link">Top 10</a>
                <a href="#" class="nav-link">My Playlist</a>
                <a href="#" class="nav-link">Account</a>
            </div>
        </nav>
    </header>

    <main>
        <section class="hero">
            <div class="hero-content">
                <h1 class="text-4xl font-bold mb-4">Welcome to PLAY TV GH</h1>
                <p class="text-xl mb-6">Your ultimate destination for African music videos</p>
                <a href="#" class="btn pulse">Start Watching Now</a>
            </div>
        </section>

        <section class="container mx-auto mt-12">
            <h2 class="text-3xl font-bold mb-6">Featured Genres</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div class="genre-section">
                    <h3 class="text-2xl font-bold mb-4">High Life Music</h3>
                    <div class="video-card">
                        <div class="video-player">
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="text-xl font-bold mb-2">Top High Life Hit</h4>
                            <p class="mb-4">Artist Name</p>
                            <div class="flex">
                                <a href="#" class="share-btn"><i class="fab fa-whatsapp"></i></a>
                                <a href="#" class="share-btn facebook"><i class="fab fa-facebook-f"></i></a>
                                <a href="#" class="share-btn instagram"><i class="fab fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="genre-section">
                    <h3 class="text-2xl font-bold mb-4">Hip Life Music</h3>
                    <div class="video-card">
                        <div class="video-player">
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="text-xl font-bold mb-2">Hip Life Banger</h4>
                            <p class="mb-4">Artist Name</p>
                            <div class="flex">
                                <a href="#" class="share-btn"><i class="fab fa-whatsapp"></i></a>
                                <a href="#" class="share-btn facebook"><i class="fab fa-facebook-f"></i></a>
                                <a href="#" class="share-btn instagram"><i class="fab fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="genre-section">
                    <h3 class="text-2xl font-bold mb-4">Afrobeats</h3>
                    <div class="video-card">
                        <div class="video-player">
                            <iframe src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen></iframe>
                        </div>
                        <div class="p-4">
                            <h4 class="text-xl font-bold mb-2">Afrobeats Sensation</h4>
                            <p class="mb-4">Artist Name</p>
                            <div class="flex">
                                <a href="#" class="share-btn"><i class="fab fa-whatsapp"></i></a>
                                <a href="#" class="share-btn facebook"><i class="fab fa-facebook-f"></i></a>
                                <a href="#" class="share-btn instagram"><i class="fab fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="container mx-auto mt-12">
            <h2 class="text-3xl font-bold mb-6">Top 10 Chart</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-5 gap-6">
                <!-- Top 10 videos will be dynamically inserted here -->
            </div>
        </section>
    </main>

    <footer class="bg-black py-8 mt-12">
        <div class="container mx-auto text-center">
            <p>&copy; 2023 PLAY TV GH. All rights reserved.</p>
        </div>
    </footer>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <script>
        $(document).ready(function() {
            // Simulating dynamic content loading
            const topChartVideos = [
                {title: "Song 1", artist: "Artist 1", thumbnail: "https://picsum.photos/300/200?random=1"},
                {title: "Song 2", artist: "Artist 2", thumbnail: "https://picsum.photos/300/200?random=2"},
                {title: "Song 3", artist: "Artist 3", thumbnail: "https://picsum.photos/300/200?random=3"},
                {title: "Song 4", artist: "Artist 4", thumbnail: "https://picsum.photos/300/200?random=4"},
                {title: "Song 5", artist: "Artist 5", thumbnail: "https://picsum.photos/300/200?random=5"},
                {title: "Song 6", artist: "Artist 6", thumbnail: "https://picsum.photos/300/200?random=6"},
                {title: "Song 7", artist: "Artist 7", thumbnail: "https://picsum.photos/300/200?random=7"},
                {title: "Song 8", artist: "Artist 8", thumbnail: "https://picsum.photos/300/200?random=8"},
                {title: "Song 9", artist: "Artist 9", thumbnail: "https://picsum.photos/300/200?random=9"},
                {title: "Song 10", artist: "Artist 10", thumbnail: "https://picsum.photos/300/200?random=10"}
            ];

            const $topChartSection = $('.container:last .grid');
            topChartVideos.forEach((video, index) => {
                const $videoCard = $(`
                    <div class="video-card">
                        <img src="${video.thumbnail}" alt="${video.title}" class="w-full h-40 object-cover">
                        <div class="p-4">
                            <h4 class="text-xl font-bold mb-2">${index + 1}. ${video.title}</h4>
                            <p class="mb-4">${video.artist}</p>
                            <div class="flex">
                                <a href="#" class="share-btn"><i class="fab fa-whatsapp"></i></a>
                                <a href="#" class="share-btn facebook"><i class="fab fa-facebook-f"></i></a>
                                <a href="#" class="share-btn instagram"><i class="fab fa-instagram"></i></a>
                            </div>
                        </div>
                    </div>
                `);
                $topChartSection.append($videoCard);
            });

            // Smooth scrolling for navigation links
            $('a[href^="#"]').on('click', function(event) {
                event.preventDefault();
                $('html, body').animate({
                    scrollTop: $($.attr(this, 'href')).offset().top
                }, 500);
            });

            // Add hover effect to video cards
            $('.video-card').hover(
                function() { $(this).addClass('shadow-lg'); },
                function() { $(this).removeClass('shadow-lg'); }
            );
        });
    </script>
</body>
</html>
```

This code creates a responsive and interactive music video streaming app called PLAY TV GH with the following features:

1. Red and black color scheme
2. Logo with African map, black star, and play icon
3. Featured genres: High Life Music, Hip Life Music, and Afrobeats (easily expandable to include Afro Dancehall and Amapiano)
4. Top 10 chart
5. Video playback using YouTube embedded players
6. Social sharing buttons for WhatsApp, Facebook, and Instagram
7. Responsive design for various screen sizes
8. Interactive elements with hover effects and smooth animations
9. Dynamic content loading for the Top 10 chart

<!---
PLAYTVGH/PLAYTVGH is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
