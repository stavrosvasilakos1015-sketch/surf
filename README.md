<!DOCTYPE html>
<html lang="el">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surf Life | Σχολή & Εξοπλισμός Surf</title>
    <style>
        /* Βασικές Ρυθμίσεις */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            color: #333;
            line-height: 1.6;
            background-color: #f4f9fc;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* Επικεφαλίδα (Navigation) */
        header {
            background-color: #0077b6;
            color: #fff;
            padding: 20px 50px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            letter-spacing: 1px;
        }

        header nav ul {
            display: flex;
            list-style: none;
        }

        header nav ul li {
            margin-left: 20px;
        }

        header nav ul li a {
            font-weight: 500;
            transition: color 0.3s;
        }

        header nav ul li a:hover {
            color: #90e0ef;
        }

        /* Αρχική Εικόνα (Hero Section) */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), 
                        url('https://unsplash.com') no-repeat center center/cover;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: #fff;
            padding: 0 20px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.6);
        }

        .hero p {
            font-size: 20px;
            margin-bottom: 30px;
            max-width: 600px;
            text-shadow: 1px 1px 3px rgba(0,0,0,0.6);
        }

        .btn {
            background-color: #00b4d8;
            color: #fff;
            padding: 12px 30px;
            border-radius: 25px;
            font-size: 18px;
            font-weight: bold;
            transition: background 0.3s;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            background-color: #0077b6;
        }

        /* Ενότητες Περιεχομένου */
        .container {
            max-width: 1100px;
            margin: auto;
            padding: 60px 20px;
        }

        .section-title {
            text-align: center;
            font-size: 32px;
            margin-bottom: 40px;
            color: #03045e;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background-color: #00b4d8;
            margin: 10px auto 0;
        }

        /* Υπηρεσίες (Grid) */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: #fff;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }

        .service-card:hover {
            transform: translateY(-5px);
        }

        .service-card h3 {
            margin: 15px 0;
            color: #0077b6;
        }

        /* Σχετικά με Εμάς */
        .about-text {
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
            font-size: 18px;
        }

        /* Φόρμα Επικοινωνίας */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: #fff;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
        }

        .form-group input, .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 16px;
        }

        /* Υποσέλιδο (Footer) */
        footer {
            background-color: #03045e;
            color: #fff;
            text-align: center;
            padding: 20px;
            margin-top: 40px;
            font-size: 14px;
        }

        /* Responsive για Κινητά */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                padding: 15px;
            }
            header nav ul {
                margin-top: 15px;
            }
            .hero h1 {
                font-size: 32px;
            }
            .hero p {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>

    <!-- Επικεφαλίδα & Μενού -->
    <header>
        <div class="logo">🏄‍♂️ SURF LIFE</div>
        <nav>
            <ul>
                <li><a href="#home">Αρχική</a></li>
                <li><a href="#services">Υπηρεσίες</a></li>
                <li><a href="#about">Σχετικά</a></li>
                <li><a href="#contact">Επικοινωνία</a></li>
            </ul>
        </nav>
    </header>

    <!-- Αρχική Εικόνα (Hero) -->
    <section id="home" class="hero">
        <h1>Δάμασε τα Κύματα μαζί μας</h1>
        <p>Μάθε surf από τους καλύτερους επαγγελματίες εκπαιδευτές και νιώσε την απόλυτη ελευθερία στη θάλασσα.</p>
        <a href="#services" class="btn">Ξεκίνα Τώρα</a>
    </section>

    <!-- Υπηρεσίες -->
    <section id="services" class="container">
        <h2 class="section-title">Οι Υπηρεσίες Μας</h2>
        <div class="services-grid">
            <div class="service-card">
                <h2>🏄‍♀️</h2>
                <h3>Μαθήματα Surf</h3>
                <p>Τμήματα για αρχάριους και προχωρημένους με έμπειρους ναυαγοσώστες και εκπαιδευτές.</p>
            </div>
            <div class="service-card">
                <h2>🛠️</h2>
                <h3>Ενοικίαση Εξοπλισμού</h3>
                <p>Διαθέτουμε σανίδες και στολές υψηλής ποιότητας για κάθε επίπεδο και σωματότυπο.</p>
            </div>
            <div class="service-card">
                <h2>🚐</h2>
                <h3>Surf Trips</h3>
                <p>Οργανωμένες εξορμήσεις στις καλύτερες παραλίες της Ελλάδας για ασταμάτητο ride.</p>
            </div>
        </div>
    </section>

    <!-- Σχετικά με Εμάς -->
    <section id="about" style="background-color: #e2eff5;">
        <div class="container">
            <h2 class="section-title">Ποιοι Είμαστε</h2>
            <p class="about-text">
                Η σχολή Surf Life δημιουργήθηκε από μια παρέα ανθρώπων με πάθος για τη θάλασσα και το surf. Στόχος μας είναι να μεταδώσουμε την αγάπη μας για το άθλημα με ασφάλεια, σεβασμό στο περιβάλλον και φυσικά, πολύ διασκέδαση!
            </p>
        </div>
    </section>

    <!-- Επικοινωνία -->
    <section id="contact" class="container">
        <h2 class="section-title">Επικοινωνήστε Μαζί Μας</h2>
        <form class="contact-form" action="#" method="POST" onsubmit="alert('Ευχαριστούμε! Θα επικοινωνήσουμε σύντομα μαζί σας.'); return false;">
            <div class="form-group">
                <label for="name">Όνομα</label>
                <input type="text" id="name" required placeholder="Το όνομά σας">
            </div>
            <div class="form-group">
                <label for="email">Email</label>
                <input type="email" id="email" required placeholder="Το email σας">
            </div>
            <div class="form-group">
                <label for="message">Μήνυμα</label>
                <textarea id="message" rows="5" required placeholder="Πώς μπορούμε να σας βοηθήσουμε;"></textarea>
            </div>
            <button type="submit" class="btn" style="width: 100%;">Αποστολή</button>
        </form>
    </section>

    <!-- Υποσέλιδο -->
    <footer>
        <p>&copy; 2026 Surf Life. Με επιφύλαξη παντός δικαιώματος.</p>
    </footer>

</body>
</html>
