<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">

    <meta name="viewport"
          content="width=device-width, initial-scale=1.0">

    <meta name="description"
          content="The Next Generation Movement - NGM">

    <meta name="keywords"
          content="NGM, Next Generation Movement, Nigeria, membership">

    <meta name="author"
          content="The Next Generation Movement">

    <title>Next Generation Movement | NGM</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f5f7f6;
            color: #17221c;
            line-height: 1.6;
        }

        /* =========================
           HEADER
        ========================== */

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(8, 45, 28, 0.97);
            box-shadow: 0 3px 15px rgba(0,0,0,0.2);
        }

        .navbar {
            max-width: 1250px;
            margin: auto;
            padding: 15px 25px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
            color: white;
            text-decoration: none;
        }

        .logo-circle {
            width: 48px;
            height: 48px;
            border-radius: 50%;
            background: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            color: #075c36;
            border: 3px solid #d6b35a;
        }

        .logo-text {
            font-size: 20px;
            font-weight: bold;
        }

        .logo-small {
            font-size: 11px;
            color: #d6b35a;
            display: block;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 25px;
        }

        nav a {
            color: white;
            text-decoration: none;
            font-size: 14px;
            font-weight: bold;
            transition: 0.3s;
        }

        nav a:hover {
            color: #e0bd62;
        }

        .join-button {
            background: #d4af37;
            color: #102619 !important;
            padding: 10px 18px;
            border-radius: 25px;
        }

        /* =========================
           HERO
        ========================== */

        .hero {
            min-height: 100vh;
            padding: 130px 25px 80px;
            background:
                linear-gradient(
                    rgba(2, 36, 22, 0.86),
                    rgba(2, 36, 22, 0.92)
                ),
                url("ngm-background.jpg");

            background-size: cover;
            background-position: center;

            color: white;

            display: flex;
            align-items: center;
            justify-content: center;
        }

        .hero-container {
            max-width: 1150px;
            width: 100%;
            display: grid;
            grid-template-columns: 1fr 1.2fr;
            gap: 70px;
            align-items: center;
        }

        .leader-photo {
            text-align: center;
        }

        .leader-photo img {
            width: 330px;
            height: 400px;
            object-fit: cover;
            border-radius: 20px;
            border: 6px solid #d4af37;
            box-shadow: 0 20px 50px rgba(0,0,0,0.45);
        }

        .leader-title {
            margin-top: 18px;
            font-size: 16px;
            color: #e4c76a;
            font-weight: bold;
            letter-spacing: 1px;
        }

        .hero-content h1 {
            font-size: 60px;
            line-height: 1.05;
            margin-bottom: 15px;
        }

        .hero-content h1 span {
            color: #d4af37;
        }

        .hero-content h2 {
            font-size: 25px;
            margin-bottom: 20px;
            font-weight: normal;
        }

        .hero-content p {
            color: #e0e7e3;
            max-width: 700px;
            font-size: 17px;
        }

        .hero-buttons {
            margin-top: 30px;
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .button {
            display: inline-block;
            padding: 14px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
        }

        .button-primary {
            background: #d4af37;
            color: #112518;
        }

        .button-secondary {
            border: 1px solid white;
            color: white;
        }

        /* =========================
           MEMBER COUNTER
        ========================== */

        .counter-section {
            background: white;
            padding: 55px 20px;
            text-align: center;
        }

        .counter-title {
            color: #526058;
            font-size: 15px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .counter {
            color: #075c36;
            font-size: 55px;
            font-weight: bold;
            margin: 5px 0;
        }

        .counter-label {
            font-size: 17px;
            color: #555;
        }

        /* =========================
           GENERAL SECTIONS
        ========================== */

        section {
            padding: 90px 20px;
        }

        .section-container {
            max-width: 1150px;
            margin: auto;
        }

        .section-heading {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-heading h2 {
            color: #075c36;
            font-size: 38px;
            margin-bottom: 10px;
        }

        .section-heading p {
            color: #68736c;
            max-width: 700px;
            margin: auto;
        }

        /* =========================
           MISSION / VISION
        ========================== */

        .mission-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
        }

        .info-card {
            background: white;
            padding: 40px;
            border-radius: 18px;
            box-shadow: 0 8px 30px rgba(0,0,0,0.07);
            border-top: 5px solid #d4af37;
        }

        .info-card h3 {
            color: #075c36;
            margin-bottom: 15px;
            font-size: 25px;
        }

        /* =========================
           OBJECTIVES
        ========================== */

        .objectives {
            background: #eef3ef;
        }

        .objective-grid {
            display: grid;
            grid-template-columns: repeat(3,1fr);
            gap: 25px;
        }

        .objective-card {
            background: white;
            padding: 30px;
            border-radius: 16px;
            box-shadow: 0 6px 20px rgba(0,0,0,0.06);
        }

        .objective-number {
            width: 45px;
            height: 45px;
            border-radius: 50%;
            background: #075c36;
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            margin-bottom: 18px;
        }

        .objective-card h3 {
            color: #075c36;
            margin-bottom: 10px;
        }

        /* =========================
           MEMBERSHIP
        ========================== */

        .membership {
            background:
                linear-gradient(
                    rgba(4,45,28,0.97),
                    rgba(4,45,28,0.97)
                );
            color: white;
        }

        .membership .section-heading h2 {
            color: #d4af37;
        }

        .membership .section-heading p {
            color: #dbe5df;
        }

        .registration-box {
            background: white;
            color: #17221c;
            max-width: 900px;
            margin: auto;
            padding: 45px;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.25);
        }

        .form-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .form-group {
            display: flex;
            flex-direction: column;
        }

        .form-group.full {
            grid-column: 1 / -1;
        }

        label {
            font-weight: bold;
            margin-bottom: 7px;
            color: #304038;
        }

        input,
        select {
            width: 100%;
            padding: 14px;
            border: 1px solid #ccd4ce;
            border-radius: 8px;
            font-size: 15px;
            outline: none;
        }

        input:focus,
        select:focus {
            border-color: #075c36;
            box-shadow: 0 0 0 3px rgba(7,92,54,0.1);
        }

        .photo-upload {
            padding: 10px;
            background: #f3f5f4;
        }

        .privacy-box {
            margin-top: 20px;
            padding: 15px;
            background: #f0f5f1;
            border-left: 4px solid #075c36;
            font-size: 13px;
            color: #53605a;
        }

        .checkbox {
            display: flex;
            gap: 10px;
            margin-top: 20px;
            align-items: flex-start;
        }

        .checkbox input {
            width: auto;
            margin-top: 4px;
        }

        .submit-button {
            margin-top: 25px;
            width: 100%;
            padding: 16px;
            border: none;
            border-radius: 30px;
            background: #075c36;
            color: white;
            font-size: 17px;
            font-weight: bold;
            cursor: pointer;
        }

        .submit-button:hover {
            background: #064529;
        }

        /* =========================
           ID CARD PREVIEW
        ========================== */

        .id-section {
            background: #f5f7f6;
        }

        .id-card {
            max-width: 600px;
            margin: auto;
            background: linear-gradient(
                135deg,
                #06452a,
                #0b7044
            );
            border-radius: 18px;
            padding: 25px;
            color: white;
            box-shadow: 0 15px 45px rgba(0,0,0,0.2);
            position: relative;
            overflow: hidden;
        }

        .id-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid rgba(255,255,255,0.3);
            padding-bottom: 15px;
        }

        .id-header h3 {
            color: #e0bd62;
        }

        .id-body {
            display: flex;
            gap: 25px;
            margin-top: 25px;
            align-items: center;
        }

        .id-photo {
            width: 110px;
            height: 130px;
            background: white;
            border-radius: 8px;
            object-fit: cover;
        }

        .id-information p {
            margin-bottom: 7px;
        }

        .id-information strong {
            color: #e2c56b;
        }

        .qr {
            margin-left: auto;
            width: 85px;
            height: 85px;
            background: white;
            color: black;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 11px;
            text-align: center;
        }

        /* =========================
           FOOTER
        ========================== */

        footer {
            background: #061d12;
            color: white;
            padding: 50px 20px 25px;
        }

        .footer-container {
            max-width: 1150px;
            margin: auto;
            display: grid;
            grid-template-columns: 2fr 1fr 1fr;
            gap: 40px;
        }

        footer h3 {
            color: #d4af37;
            margin-bottom: 15px;
        }

        footer ul {
            list-style: none;
        }

        footer li {
            margin-bottom: 8px;
        }

        footer a {
            color: #dbe5df;
            text-decoration: none;
        }

        .copyright {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.15);
            color: #9aa9a0;
            font-size: 13px;
        }

        /* =========================
           MOBILE
        ========================== */

        @media(max-width: 850px) {

            nav ul {
                display: none;
            }

            .hero-container {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero-content h1 {
                font-size: 42px;
            }

            .hero-buttons {
                justify-content: center;
            }

            .mission-grid,
            .objective-grid,
            .form-grid,
            .footer-container {
                grid-template-columns: 1fr;
            }

            .form-group.full {
                grid-column: auto;
            }

            .registration-box {
                padding: 25px;
            }

            .leader-photo img {
                width: 260px;
                height: 320px;
            }

            .id-body {
                flex-wrap: wrap;
            }

            .qr {
                margin-left: 0;
            }
        }

    </style>
</head>

<body>

<!-- =========================
     NAVIGATION
========================== -->

<header>

    <div class="navbar">

        <a href="#home" class="logo">

            <div class="logo-circle">
                NGM
            </div>

            <div>
                <div class="logo-text">
                    NEXT GENERATION MOVEMENT
                </div>

                <span class="logo-small">
                    NGM OFFICIAL PLATFORM
                </span>
            </div>

        </a>

        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#objectives">Objectives</a></li>
                <li><a href="#membership">Membership</a></li>
                <li><a href="#idcard">ID Card</a></li>
                <li>
                    <a href="#membership" class="join-button">
                        JOIN NGM
                    </a>
                </li>
            </ul>
        </nav>

    </div>

</header>


<!-- =========================
     HERO
========================== -->

<section class="hero" id="home">

    <div class="hero-container">

        <div class="leader-photo">

            <!--
                REPLACE "chairman.jpg"
                WITH YOUR ACTUAL PHOTO
            -->

            <img src="chairman.jpg"
                 alt="NGM Patron and Chairman">

            <div class="leader-title">
                PATRON & CHAIRMAN
                <br>
                THE NEXT GENERATION MOVEMENT
            </div>

        </div>


        <div class="hero-content">

            <h1>
                THE NEXT
                <span>GENERATION</span>
                MOVEMENT
            </h1>

            <h2>
                NGM
            </h2>

            <p>
                A platform for citizens who wish to participate
                constructively in civic and political life,
                promote responsible leadership and contribute
                to the development of Nigeria.
            </p>

            <div class="hero-buttons">

                <a href="#membership"
                   class="button button-primary">
                    Become a Member
                </a>

                <a href="#about"
                   class="button button-secondary">
                    Learn More
                </a>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     MEMBER COUNTER
========================== -->

<section class="counter-section">

    <div class="counter-title">
        Registered NGM Members
    </div>

    <div class="counter" id="memberCounter">
        0
    </div>

    <div class="counter-label">
        Growing membership community
    </div>

</section>


<!-- =========================
     ABOUT
========================== -->

<section id="about">

    <div class="section-container">

        <div class="section-heading">

            <h2>
                About NGM
            </h2>

            <p>
                The Next Generation Movement is a civic and
                political movement focused on participation,
                leadership development and community engagement.
            </p>

        </div>


        <div class="mission-grid">

            <div class="info-card">

                <h3>
                    Our Mission
                </h3>

                <p>
                    To encourage responsible participation in
                    public affairs, develop future leaders,
                    promote civic responsibility and provide
                    opportunities for members of the next
                    generation to contribute to society.
                </p>

            </div>


            <div class="info-card">

                <h3>
                    Our Vision
                </h3>

                <p>
                    To build an active and responsible generation
                    of citizens equipped to participate in
                    leadership, community development and
                    democratic processes.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     OBJECTIVES
========================== -->

<section class="objectives" id="objectives">

    <div class="section-container">

        <div class="section-heading">

            <h2>
                Aims & Objectives
            </h2>

            <p>
                Key areas of focus for the movement.
            </p>

        </div>


        <div class="objective-grid">

            <div class="objective-card">

                <div class="objective-number">
                    01
                </div>

                <h3>
                    Youth Participation
                </h3>

                <p>
                    Encourage young Nigerians to participate
                    constructively in civic and public affairs.
                </p>

            </div>


            <div class="objective-card">

                <div class="objective-number">
                    02
                </div>

                <h3>
                    Leadership Development
                </h3>

                <p>
                    Encourage leadership development,
                    responsibility and public service.
                </p>

            </div>


            <div class="objective-card">

                <div class="objective-number">
                    03
                </div>

                <h3>
                    Community Engagement
                </h3>

                <p>
                    Promote community-based initiatives and
                    constructive citizen participation.
                </p>

            </div>


            <div class="objective-card">

                <div class="objective-number">
                    04
                </div>

                <h3>
                    Education
                </h3>

                <p>
                    Support awareness, education and opportunities
                    that can strengthen civic participation.
                </p>

            </div>


            <div class="objective-card">

                <div class="objective-number">
                    05
                </div>

                <h3>
                    Accountability
                </h3>

                <p>
                    Encourage responsible conduct, transparency
                    and accountability among members.
                </p>

            </div>


            <div class="objective-card">

                <div class="objective-number">
                    06
                </div>

                <h3>
                    National Development
                </h3>

                <p>
                    Encourage members to contribute positively
                    to Nigeria's social and economic development.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     MEMBERSHIP REGISTRATION
========================== -->

<section class="membership" id="membership">

    <div class="section-container">

        <div class="section-heading">

            <h2>
                Become an Active Member
            </h2>

            <p>
                Complete the membership application below.
            </p>

        </div>


        <div class="registration-box">

            <form id="membershipForm">

                <div class="form-grid">


                    <div class="form-group">

                        <label for="firstName">
                            First Name
                        </label>

                        <input
                            type="text"
                            id="firstName"
                            required
                            placeholder="Enter first name">

                    </div>


                    <div class="form-group">

                        <label for="lastName">
                            Last Name
                        </label>

                        <input
                            type="text"
                            id="lastName"
                            required
                            placeholder="Enter surname">

                    </div>


                    <div class="form-group">

                        <label for="dob">
                            Date of Birth
                        </label>

                        <input
                            type="date"
                            id="dob"
                            required>

                    </div>


                    <div class="form-group">

                        <label for="nationality">
                            Nationality
                        </label>

                        <input
                            type="text"
                            id="nationality"
                            required
                            placeholder="e.g. Nigerian">

                    </div>


                    <div class="form-group">

                        <label for="state">
                            State of Origin
                        </label>

                        <input
                            type="text"
                            id="state"
                            required
                            placeholder="State of origin">

                    </div>


                    <div class="form-group">

                        <label for="lga">
                            Local Government Area
                        </label>

                        <input
                            type="text"
                            id="lga"
                            required
                            placeholder="Local Government">

                    </div>


                    <div class="form-group">

                        <label for="email">
                            Email Address
                        </label>

                        <input
                            type="email"
                            id="email"
                            required
                            placeholder="you@example.com">

                    </div>


                    <div class="form-group">

                        <label for="phone">
                            Phone Number
                        </label>

                        <input
                            type="tel"
                            id="phone"
                            required
                            placeholder="08000000000">

                    </div>


                    <div class="form-group full">

                        <label for="nin">
                            National Identification Number (NIN)
                        </label>

                        <input
                            type="text"
                            id="nin"
                            maxlength="11"
                            inputmode="numeric"
                            placeholder="Enter NIN">

                    </div>


                    <div class="form-group full">

                        <label for="photo">
                            Passport Photograph
                        </label>

                        <input
                            class="photo-upload"
                            type="file"
                            id="photo"
                            accept="image/*">

                    </div>

                </div>


                <div class="privacy-box">

                    <strong>Privacy Notice:</strong>

                    Personal information submitted through the
                    production membership system should be processed
                    only for legitimate membership administration,
                    identity verification and related purposes.
                    Sensitive identity information should be stored
                    securely and accessed only by authorized personnel.

                </div>


                <div class="checkbox">

                    <input
                        type="checkbox"
                        id="agreement"
                        required>

                    <label for="agreement">

                        I confirm that the information provided is
                        accurate and agree to the movement's
                        membership rules and privacy requirements.

                    </label>

                </div>


                <button
                    type="submit"
                    class="submit-button">

                    SUBMIT MEMBERSHIP APPLICATION

                </button>

            </form>

        </div>

    </div>

</section>


<!-- =========================
     ID CARD PREVIEW
========================== -->

<section class="id-section" id="idcard">

    <div class="section-container">

        <div class="section-heading">

            <h2>
                NGM Membership ID Card
            </h2>

            <p>
                Example of the membership identification card
                that can be generated automatically after
                successful registration.
            </p>

        </div>


        <div class="id-card">

            <div class="id-header">

                <h3>
                    NGM
                </h3>

                <span>
                    ACTIVE MEMBER
                </span>

            </div>


            <div class="id-body">

                <img
                    class="id-photo"
                    src="member-placeholder.jpg"
                    alt="Member photograph">


                <div class="id-information">

                    <p>
                        <strong>Name:</strong>
                        MEMBER NAME
                    </p>

                    <p>
                        <strong>ID Number:</strong>
                        NGM-00000001
                    </p>

                    <p>
                        <strong>Status:</strong>
                        Active Member
                    </p>

                    <p>
                        <strong>Organization:</strong>
                        Next Generation Movement
                    </p>

                </div>


                <div class="qr">

                    QR
                    <br>
                    VERIFICATION

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     FOOTER
========================== -->

<footer>

    <div class="footer-container">

        <div>

            <h3>
                NEXT GENERATION MOVEMENT
            </h3>

            <p>
                Official digital platform of the
                Next Generation Movement (NGM).
            </p>

        </div>


        <div>

            <h3>
                Navigation
            </h3>

            <ul>

                <li>
                    <a href="#home">Home</a>
                </li>

                <li>
                    <a href="#about">About</a>
                </li>

                <li>
                    <a href="#objectives">Objectives</a>
                </li>

                <li>
                    <a href="#membership">
                        Membership
                    </a>
                </li>

            </ul>

        </div>


        <div>

            <h3>
                Membership
            </h3>

            <ul>

                <li>
                    <a href="#membership">
                        Join NGM
                    </a>
                </li>

                <li>
                    <a href="#idcard">
                        Membership ID
                    </a>
                </li>

                <li>
                    <a href="#">
                        Privacy Policy
                    </a>
                </li>

            </ul>

        </div>

    </div>


    <div class="copyright">

        © 2026 The Next Generation Movement (NGM).
        All rights reserved.

    </div>

</footer>


<!-- =========================
     BASIC DEMO JAVASCRIPT
========================== -->

<script>

    /*
       IMPORTANT:

       This is ONLY a front-end demonstration.

       It does NOT provide secure membership storage,
       real duplicate prevention, email delivery,
       ID-card generation or a global member database.

       Those functions must be moved to a secure backend.
    */


    const form =
        document.getElementById("membershipForm");

    const counter =
        document.getElementById("memberCounter");


    /*
       Demo counter.

       This only exists inside the visitor's browser.
       It is NOT a real global membership counter.
    */

    let demoMembers =
        Number(localStorage.getItem("ngmDemoMembers")) || 0;

    counter.textContent =
        demoMembers.toLocaleString();


    form.addEventListener("submit", function(event) {

        event.preventDefault();


        /*
           Demo behavior only.

           A real website should send the form to
           a secure backend API.
        */

        demoMembers++;

        localStorage.setItem(
            "ngmDemoMembers",
            demoMembers
        );

        counter.textContent =
            demoMembers.toLocaleString();


        alert(
            "Thank you. Your NGM membership application has been submitted in this demonstration."
        );


        form.reset();

    });

</script>

</body>
</html>
