<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Consórcio - Realize Seus Sonhos</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
            line-height: 1.6;
        }
        
        header {
            background-color: #003366;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px 0;
        }
        
        .hero {
            background-image: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://via.placeholder.com/1200x400');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
            margin-bottom: 30px;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .btn {
            display: inline-block;
            background-color: #ff6600;
            color: white;
            padding: 12px 30px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 20px;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #e65c00;
        }
        
        .benefits {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin: 40px 0;
        }
        
        .benefit-card {
            flex-basis: 30%;
            background: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin-bottom: 20px;
            text-align: center;
        }
        
        .benefit-card i {
            font-size: 2.5rem;
            color: #003366;
            margin-bottom: 15px;
        }
        
        .form-section {
            background-color: white;
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin: 40px 0;
        }
        
        .form-section h2 {
            text-align: center;
            margin-bottom: 30px;
            color: #003366;
        }
        
        form {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
        }
        
        .form-group input, 
        .form-group select {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        
        .full-width {
            grid-column: 1 / -1;
        }
        
        footer {
            background-color: #003366;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 40px;
        }
        
        @media (max-width: 768px) {
            .benefit-card {
                flex-basis: 100%;
            }
            
            form {
                grid-template-columns: 1fr;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>Consórcio Imobiliário</h1>
            <p>A forma inteligente de realizar seus sonhos</p>
        </div>
    </header>
    
    <section class="hero">
        <div class="container">
            <h1>Adquira seu imóvel sem juros e sem complicações</h1>
            <p>Com o consórcio você pode conquistar a casa própria, carro ou outros bens de forma planejada e sem sustos no orçamento.</p>
            <a href="#formulario" class="btn">Quero Saber Mais</a>
        </div>
    </section>
    
    <div class="container">
        <section class="benefits">
            <div class="benefit-card">
                <i class="fas fa-percentage"></i>
                <h3>Sem Juros</h3>
                <p>Você paga apenas o valor real do bem, sem juros abusivos como em financiamentos tradicionais.</p>
            </div>
            
            <div class="benefit-card">
                <i class="fas fa-hand-holding-usd"></i>
                <h3>Parcelas Fixas</h3>
                <p>Parcelas que cabem no seu bolso e não mudam durante todo o período do consórcio.</p>
            </div>
            
            <div class="benefit-card">
                <i class="fas fa-medal"></i>
                <h3>Crédito Garantido</h3>
                <p>Não depende de aprovação de crédito em bancos ou taxas de juros do mercado.</p>
            </div>
        </section>
        
        <section id="formulario" class="form-section">
            <h2>Solicite uma Proposta</h2>
            <p>Preencha o formulário abaixo e um de nossos consultores entrará em contato para apresentar as melhores opções para você.</p>
            
            <form action="#" method="POST">
                <div class="form-group">
                    <label for="nome">Nome Completo</label>
                    <input type="text" id="nome" name="nome" required>
                </div>
                
                <div class="form-group">
                    <label for="email">E-mail</label>
                    <input type="email" id="email" name="email" required>
                </div>
                
                <div class="form-group">
                    <label for="telefone">Telefone</label>
                    <input type="tel" id="telefone" name="telefone" required>
                </div>
                
                <div class="form-group">
                    <label for="cidade">Cidade</label>
                    <input type="text" id="cidade" name="cidade" required>
                </div>
                
                <div class="form-group">
                    <label for="tipo">Tipo de Consórcio</label>
                    <select id="tipo" name="tipo" required>
                        <option value="">Selecione...</option>
                        <option value="imovel">Imóvel</option>
                        <option value="carro">Automóvel</option>
                        <option value="servicos">Serviços</option>
                        <option value="outros">Outros</option>
                    </select>
                </div>
                
                <div class="form-group">
                    <label for="valor">Valor Pretendido (R$)</label>
                    <input type="number" id="valor" name="valor" required>
                </div>
                
                <div class="form-group full-width">
                    <label for="mensagem">Mensagem (Opcional)</label>
                    <textarea id="mensagem" name="mensagem" rows="4"></textarea>
                </div>
                
                <div class="form-group full-width">
                    <button type="submit" class="btn">Enviar Solicitação</button>
                </div>
            </form>
        </section>
    </div>
    
    <footer>
        <div class="container">
            <p>&copy; 2023 Consórcio Imobiliário. Todos os direitos reservados.</p>
            <p>CNPJ: 00.000.000/0000-00</p>
        </div>
    </footer>
</body>
</html>
