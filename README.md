<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Website</title>
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f9f9f9;
            color: #333;
            transition: background-color 0.3s, color 0.3s;
        }

        .dark-mode {
            background-color: #333;
            color: white;
        }

        header {
            background-color: #333;
            color: white;
            padding: 1rem 0;
            text-align: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .dark-mode header {
            background-color: #222;
        }

        header nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            margin: 0;
        }

        header nav ul li {
            margin: 0 1rem;
        }

        header nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 700;
            transition: color 0.3s;
        }

        header nav ul li a:hover {
            color: #ff6347;
        }

        #theme-toggle {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: none;
            border: 1px solid white;
            color: white;
            padding: 0.5rem 1rem;
            cursor: pointer;
            transition: background 0.3s, color 0.3s;
        }

        .dark-mode #theme-toggle {
            border: 1px solid #ff6347;
            color: #ff6347;
        }

        #hero {
            background-color: #282c34;
            color: white;
            padding: 4rem 2rem;
            text-align: center;
            margin-top: 70px;
            transition: background-color 0.3s, color 0.3s;
        }

        .dark-mode #hero {
            background-color: #1b1e23;
        }

        #hero h2 {
            margin-bottom: 1rem;
            font-size: 2.5rem;
        }

        #hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto;
            line-height: 1.5;
        }

        #projects {
            padding: 4rem 2rem;
            background-color: #f4f4f4;
            transition: background-color 0.3s;
        }

        .dark-mode #projects {
            background-color: #2c2f33;
        }

        #projects h2 {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2rem;
        }

        .project {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 2rem;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s, background-color 0.3s;
        }

        .dark-mode .project {
            background-color: #3a3e44;
            color: white;
        }

        .project:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
        }

        .project h3 {
            margin-bottom: 1rem;
            font-size: 1.5rem;
            color: #333;
        }

        .dark-mode .project h3 {
            color: #ff6347;
        }

        .project p {
            font-size: 1rem;
            color: #666;
        }

        .dark-mode .project p {
            color: #ccc;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1rem;
            transition: background-color 0.3s, color 0.3s;
        }

        .dark-mode footer {
            background-color: #222;
        }

        footer a {
            color: #ff6347;
            text-decoration: none;
            font-weight: 700;
        }

        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>My Portfolio</h1>
        <nav>
            <ul class="nav justify-content-center">
                <li class="nav-item">
                    <a class="nav-link" href="#hero">Home</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#projects">Projects</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#footer">Contact</a>
                </li>
            </ul>
        </nav>
        <button id="theme-toggle">Toggle Theme</button>
    </header>

    <section id="hero" class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-lg-8">
                <h2>Welcome to My Portfolio</h2>
                <p>I am Akshat Dhamija, a sophomore in chemical engineering. My biggest passion is entrepreneurship and I love to work with startups and I'm even working on my own ventures.</p>
            </div>
        </div>
    </section>

    <section id="projects" class="container py-5">
        <h2>My Projects</h2>
        <div id="projectsCarousel" class="carousel slide" data-ride="carousel">
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <div class="row justify-content-center">
                        <div class="col-md-6 col-lg-4 mb-4">
                            <div class="card project">
                                <div class="card-body">
                                    <h3 class="card-title">Karyama</h3>
                                    <p class="card-text">I made an app that helps in fundraising for charities. It is an interface provision for accountability. Two accountability partners come together to achieve their respective goals and the one that does not keep his word according to the details filled in their Karya contract loses a certain amount of money to the charities they chose from our anti karma bucket list.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="carousel-item">
                    <div class="row justify-content-center">
                        <div class="col-md-6 col-lg-4 mb-4">
                            <div class="card project">
                                <div class="card-body">
                                    <h3 class="card-title">Matknow</h3>
                                    <p class="card-text">Making a material selection software that could help RND teams decide on what materials to use for their engineering problem. Helping in cutting down extensive literature review and iterative simulation costs.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <a class="carousel-control-prev" href="#projectsCarousel" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#projectsCarousel" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
    </section>

    <footer id="footer">
        <p>Contact me at: <a href="mailto:akshat@karyama.com">akshat@karyama.com</a></p>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/gsap.min.js"></script>
    <script>
        const themeToggle = document.getElementById('theme-toggle');
        const body = document.body;

        themeToggle.addEventListener('click', () => {
            body.classList.toggle('dark-mode');
            if (body.classList.contains('dark-mode')) {
                themeToggle.textContent = 'Light Mode';
            } else {
                themeToggle.textContent = 'Dark Mode';
            }
        });

        gsap.from('header', { duration: 1, y: -50, opacity: 0, ease: 'power4.out' });
        gsap.from('#hero', { duration: 1, y: 50, opacity: 0, delay: 0.2, ease: 'power4.out' });
        gsap.from('.project', { duration: 1, y: 50, opacity: 0, stagger: 0.2, ease: 'power4.out', delay: 0.4 });
    </script>
</body>
</html>

