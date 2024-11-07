<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rose Dourado Estética e Massagens</title>
    <link rel="stylesheet" href="css/styles.css">
    <style>
        /* Estilos para o tema de spa */
        body {
            background-color: #f0efe9;
            color: #6d4e42;
            font-family: Arial, sans-serif;
        }
        header {
            background-color: #c0a080;
            color: #ffffff;
            padding: 20px;
            text-align: center;
        }
        nav ul {
            list-style-type: none;
            padding: 0;
            display: flex;
            justify-content: center;
            margin-top: 10px;
        }
        nav ul li {
            margin-right: 20px;
            cursor: pointer;
            font-weight: bold;
            color: #6d4e42;
        }
        nav ul li:hover,
        nav ul li.active-nav {
            color: #ffffff;
        }
        .section {
            display: none;
            padding: 30px;
            text-align: center;
        }
        .active {
            display: block;
        }
        .servicos {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
        }
        .servico-btn {
            background-color: #c0a080;
            color: #fff;
            padding: 15px 30px;
            font-size: 1.2em;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        .servico-btn:hover {
            background-color: #a68a60;
        }
        .promo {
            padding: 15px;
            background-color: #fff2e0;
            margin: 15px 0;
            border-radius: 10px;
            text-align: center;
        }
        #carrinho {
            list-style-type: none;
            padding: 0;
            text-align: left;
        }
        .form-container {
            max-width: 400px;
            margin: 0 auto;
            background-color: #ffffff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .form-container input, .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .form-container button {
            background-color: #c0a080;
            color: white;
            padding: 10px;
            width: 100%;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .form-container button:hover {
            background-color: #a68a60;
        }
    </style>
</head>
<body>
    <header>
        <h1>Rose Dourado Estética e Massagens</h1>
        <nav>
            <ul>
                <li id="homeLink" onclick="showSection('home')">Home</li>
                <li id="faciaisLink" onclick="showSection('faciais')">Tratamentos Faciais</li>
                <li id="massagensLink" onclick="showSection('massagens')">Lista de Massagens</li>
                <li id="carrinhoLink" onclick="showSection('carrinho')">Carrinho</li>
                <li id="agendamentoLink" onclick="showSection('agendamento')">Agendamento</li>
            </ul>
        </nav>
    </header>

    <!-- Seção Home -->
    <section id="home" class="section active">
        <h2>Bem-vindo à Rose Dourado</h2>
        <p>Experimente o luxo e o relaxamento com nossos serviços de spa e bem-estar.</p>
        
        <div class="servicos">
            <button class="servico-btn" onclick="showSection('massagens')">Massagens</button>
            <button class="servico-btn" onclick="showSection('faciais')">Tratamentos Faciais</button>
        </div>
    </section>

    <!-- Seção Tratamentos Faciais -->
    <section id="faciais" class="section">
        <h3>Tratamentos Faciais</h3>
        <ul>
            <li>Limpeza de Pele Profunda - Remove impurezas, células mortas e excesso de oleosidade, promovendo uma pele mais limpa e fresca.</li>
            <li>Hidratação Facial - Aumenta a umidade da pele, ideal para quem tem pele seca ou precisa de um programa de nutrientes.</li>
            <li>Peeling Facial - Tratamento que remove as camadas superficiais da pele, estimulando a renovação celular e melhorando a textura da pele.</li>
            <li>Microagulhamento - Estimula a produção de colágeno e elastina através de pequenas agulhas que causam microlesões na pele, auxiliando no tratamento de cicatrizes e rugas.</li>
            <li>Radiofrequência Facial - Utiliza ondas de rádio para estimular a produção de colágeno, ajudando a firmar a pele e reduzir a flacidez.</li>
            <li>Luz Pulsada - Utiliza flashes de luz para manchas, acne e até rosáceas, além de melhorar a textura da pele.</li>
            <li>Máscaras Faciais - Máscaras com diversos ativos, como argila, carvão, colágeno ou vitamina C, para hidratar, desintoxicar, iluminar ou combater a acne.</li>
            <li>Tratamento para Acne - Inclui limpeza profunda, remoção de cravos e aplicação de produtos específicos para combater a acne.</li>
            <li>Toxina Botulínica (Botox) - Aplicação de pequenas doses de toxina para suavizar rugas e linhas de expressão, especialmente na testa, ao redor dos olhos e boca.</li>
            <li>Preenchimento Facial - Técnica usada para preencher sulcos e áreas flácidas, como as olheiras e os vincos nas bochechas, com substância como ácido hialurônico.</li>
            <li>Laser CO2 Fracionado - Estimula a regeneração celular, ajuda a reduzir manchas, linhas finas e melhora a textura da pele.</li>
            <li>Lifting Facial Não Cirúrgico - Técnicas como fios de sustentação ou radiofrequência para combater a flacidez e levantar a pele sem necessidade de cirurgia.</li>
            <li>Tratamento para Rosácea - Cuidados específicos para diminuir as lesões e lesões causadas por essa condição.</li>
            <li>Facial com Vitamina C - Ajuda a clarear manchas, iluminar a pele e combater os sinais de envelhecimento.</li>
            <li>Fototerapia - Uso de luzes de diferentes núcleos para tratar acne, melasma, envelhecimento e estimular a produção de colágeno.</li>
            <li>Criolipólise Facial - Técnica que usa o frio para reduzir as células de gordura em áreas específicas do rosto, como o contorno da mandíbula.</li>
            <li>Drenagem Linfática Facial - Massageia os pontos de desvio linfático para reduzir o surto, melhorar a circulação e promover um aspecto mais definido.</li>
            <li>Tratamento para Manchas - Combinação de peelings, laser e produtos clareadores para tratar manchas solares, de idade ou melasma.</li>
        </ul>
        <button onclick="showSection('home')">Voltar ao Home</button>
    </section>

    <!-- Seção Lista de Massagens -->
    <section id="massagens" class="section">
        <h3>Lista de Massagens</h3>
        <ul>
            <li>Massagem Relaxante - R$ 120,00</li>
            <li>Massagem Terapêutica - R$ 150,00</li>
            <li>Massagem Sueca - R$ 130,00</li>
            <li>Massagem com Pedras Quentes - R$ 180,00</li>
            <li>Massagem de Shiatsu - R$ 140,00</li>
            <li>Massagem Linfática - R$ 160,00</li>
            <li>Massagem Reflexológica - R$ 120,00</li>
            <li>Massagem Deep Tissue - R$ 200,00</li>
            <li>Massagem Ayurvédica - R$ 160,00</li>
            <li>Massagem Esportiva - R$ 180,00</li>
            <li>Massagem de Bambuterapia - R$ 170,00</li>
            <li>Massagem para Gestante - R$ 150,00</li>
            <li>Massagem com Aromaterapia - R$ 140,00</li>
            <li>Massagem Antistresse - R$ 130,00</li>
            <li>Massagem Lomi Lomi - R$ 190,00</li>
        </ul>
        <button onclick="showSection('home')">Voltar ao Home</button>
    </section>

    <!-- Seção Carrinho -->
    <section id="carrinho" class="section">
        <h3>Carrinho de Compras</h3>
        <ul id="carrinho">
            <li>Tratamento Facial: Limpeza de Pele</li>
            <li>Massagem Relaxante</li>
            <li>Hidratação Facial</li>
        </ul>
        <button onclick="showSection('home')">Voltar ao Home</button>
    </section>

    <!-- Seção Agendamento -->
    <section id="agendamento" class="section">
        <h3>Agendamento</h3>
        <div class="form-container">
            <h4>Marque seu horário</h4>
            <form action="submit_form.php" method="POST">
                <input type="text" name="nome" placeholder="Seu nome" required>
                <input type="email" name="email" placeholder="Seu e-mail" required>
                <input type="text" name="telefone" placeholder="Seu telefone" required>
                <input type="date" name="data" required>
                <select name="servico" required>
                    <option value="massagem">Massagem Relaxante</option>
                    <option value="tratamento">Tratamento Facial</option>
                </select>
                <button type="submit">Agendar</button>
            </form>
        </div>
        <button onclick="showSection('home')">Voltar ao Home</button>
    </section>

    <script>
        // Função para alternar entre as seções
        function showSection(sectionId) {
            var sections = document.querySelectorAll('.section');
            var links = document.querySelectorAll('nav ul li');
            
            sections.forEach(function(section) {
                section.classList.remove('active');
            });

            links.forEach(function(link) {
                link.classList.remove('active-nav');
            });

            document.getElementById(sectionId).classList.add('active');
            document.getElementById(sectionId + 'Link').classList.add('active-nav');
        }
    </script>
</body>
</html>
