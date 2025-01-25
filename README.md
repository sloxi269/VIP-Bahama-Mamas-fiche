<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VIP Bahama Mamas</title>
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        /* Fond personnalisable */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background: url('VOTRE_IMAGE_DE_FOND_URL') no-repeat center center fixed;
            background-size: cover;
            color: #fff;
        }

        .container {
            max-width: 600px;
            margin: 50px auto;
            padding: 30px;
            background: rgba(0, 0, 0, 0.8);
            border-radius: 15px;
            box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.5);
        }

        h1 {
            font-family: 'Pacifico', cursive;
            text-align: center;
            font-size: 2.5rem;
            color: #ffcc00;
            margin-bottom: 20px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        label {
            font-size: 1rem;
            color: #ffcc00;
            display: block;
            margin-bottom: 8px;
        }

        input, select, textarea, button {
            width: 100%;
            padding: 10px;
            font-size: 1rem;
            border: none;
            border-radius: 5px;
        }

        input, select, textarea {
            background: #fff;
            color: #333;
        }

        textarea {
            resize: none;
            height: 100px;
        }

        button {
            background: #ffcc00;
            color: #000;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        button:hover {
            background: #ffaa00;
        }

        .price {
            font-size: 1.5rem;
            color: #ffcc00;
            text-align: center;
            margin: 20px 0;
            font-weight: bold;
        }

        footer {
            text-align: center;
            margin-top: 30px;
            color: #fff;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>VIP Bahama Mamas</h1>
    <form action="send_email.php" method="POST">
        <!-- Nom complet -->
        <div class="form-group">
            <label for="name">Nom RP :</label>
            <input type="text" id="name" name="name" placeholder="Entrez votre nom RP" required>
        </div>

        <!-- Age RP -->
        <div class="form-group">
            <label for="age">Âge RP :</label>
            <input type="number" id="age" name="age" placeholder="Entrez votre âge RP" required>
        </div>

        <!-- Profession RP -->
        <div class="form-group">
            <label for="job">Profession RP :</label>
            <input type="text" id="job" name="job" placeholder="Entrez votre profession RP" required>
        </div>

        <!-- Raison pour devenir VIP -->
        <div class="form-group">
            <label for="reason">Raison pour devenir VIP :</label>
            <textarea id="reason" name="reason" placeholder="Expliquez pourquoi vous voulez devenir VIP" required></textarea>
        </div>

        <!-- Mode de paiement (RP) -->
        <div class="form-group">
            <label for="payment">Mode de paiement (RP) :</label>
            <select id="payment" name="payment" required>
                <option value="cash">Cash</option>
                <option value="bank">Banque</option>
                <option value="black_money">Argent sale</option>
            </select>
        </div>

        <!-- Montant -->
        <div class="price">Montant : 15 000 $ (RP)</div>

        <!-- Soumettre -->
        <button type="submit">Acheter VIP</button>
    </form>
</div>

<footer>
    <p>&copy; 2025 Bahama Mamas RP | Expérience exclusive</p>
</footer>

</body>
</html>
