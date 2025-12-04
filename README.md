# Velarium--velas-arom-ticas-
Velas aromáticas feitas por estudantes
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Velarium - Aromaterapia com Essências Naturais</title>
    <style>
        :root {
            --color-primary: #208085;
            --color-secondary: #d4a574;
            --color-accent: #f5e6d3;
            --color-text: #2d2d2d;
            --color-light: #faf8f5;
            --color-border: #e0d5c7;
            --color-strawberry: #FF6B8B;
            --color-blossom: #F8B5D6;
            --color-success: #4CAF50;
            --color-warning: #FF9800;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            font-size: 16px;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.5;
            color: var(--color-text);
            background-color: var(--color-light);
        }

        body {
            background-color: var(--color-light);
        }

        /* Header */
        header {
            background: linear-gradient(135deg, var(--color-primary) 0%, #1a6a6e 100%);
            color: white;
            padding: 2rem 1rem;
            text-align: center;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .header-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 1.5rem;
            flex-wrap: wrap;
        }

        .logo {
            width: 80px;
            height: 80px;
            object-fit: contain;
            border-radius: 50%;
            border: 3px solid white;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }

        h1 {
            font-size: 2.8rem;
            font-weight: 300;
            letter-spacing: 3px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }

        .tagline {
            font-size: 1.2rem;
            opacity: 0.95;
            margin-top: 0.5rem;
            font-weight: 300;
        }

        /* Main Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem 1rem;
        }

        /* Intro Section */
        .intro {
            text-align: center;
            margin-bottom: 3rem;
            padding: 2.5rem;
            background: white;
            border-radius: 15px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
            position: relative;
            overflow: hidden;
        }

        .intro::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: linear-gradient(90deg, var(--color-strawberry) 0%, var(--color-blossom) 100%);
        }

        .intro h2 {
            font-size: 2rem;
            color: var(--color-primary);
            margin-bottom: 1.2rem;
            font-weight: 400;
        }

        .intro p {
            color: #666;
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 1.5rem;
            line-height: 1.6;
        }

        /* Offer Banner */
        .offer-banner {
            background: linear-gradient(135deg, var(--color-strawberry) 0%, #ff8fab 100%);
            color: white;
            padding: 1.2rem;
            border-radius: 10px;
            margin-bottom: 2rem;
            text-align: center;
            font-size: 1.3rem;
            font-weight: 600;
            box-shadow: 0 4px 15px rgba(255, 107, 139, 0.3);
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.02); }
            100% { transform: scale(1); }
        }

        /* Highlight Section */
        .highlight {
            background: linear-gradient(135deg, #fff0f5 0%, #f8f0ff 100%);
            border-radius: 15px;
            padding: 2.5rem;
            margin-bottom: 3rem;
            text-align: center;
            border: 2px solid transparent;
            border-image: linear-gradient(90deg, var(--color-strawberry), var(--color-blossom)) 1;
            position: relative;
        }

        .highlight h3 {
            color: var(--color-primary);
            font-size: 1.8rem;
            margin-bottom: 1.2rem;
            font-weight: 500;
        }

        .highlight p {
            color: #666;
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto;
            line-height: 1.6;
        }

        /* Products Grid */
        .products-section {
            margin-bottom: 3rem;
        }

        .section-title {
            font-size: 1.8rem;
            color: var(--color-primary);
            margin-bottom: 2.5rem;
            text-align: center;
            font-weight: 400;
            letter-spacing: 1px;
            position: relative;
            padding-bottom: 1rem;
        }

        .section-title::after {
            content: "";
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: linear-gradient(90deg, var(--color-strawberry), var(--color-blossom));
            border-radius: 3px;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 2.5rem;
            margin-bottom: 2rem;
        }

        .product-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            transition: all 0.4s ease;
            display: flex;
            flex-direction: column;
            position: relative;
        }

        .product-card::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
        }

        .product-card.strawberry::before {
            background: var(--color-strawberry);
        }

        .product-card.blossom::before {
            background: var(--color-blossom);
        }

        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.15);
        }

        .product-image {
            width: 100%;
            height: 280px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .product-card:hover .product-image {
            transform: scale(1.05);
        }

        .product-info {
            padding: 2rem;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        .product-name {
            font-size: 1.6rem;
            margin-bottom: 0.8rem;
            font-weight: 600;
        }

        .strawberry .product-name {
            color: var(--color-strawberry);
        }

        .blossom .product-name {
            color: var(--color-blossom);
        }

        .product-description {
            color: #666;
            font-size: 1rem;
            margin-bottom: 1.2rem;
            flex-grow: 1;
            line-height: 1.6;
        }

        .benefits-list {
            background: linear-gradient(135deg, #f9f9f9 0%, #f0f0f0 100%);
            padding: 1.2rem;
            border-radius: 10px;
            margin-bottom: 1.5rem;
            border-left: 4px solid var(--color-primary);
        }

        .benefits-list h4 {
            color: var(--color-primary);
            margin-bottom: 0.8rem;
            font-size: 1.1rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .benefits-list ul {
            list-style: none;
            color: #555;
        }

        .benefits-list li {
            margin-bottom: 0.5rem;
            padding-left: 1.5rem;
            position: relative;
            line-height: 1.5;
        }

        .benefits-list li::before {
            content: "✓";
            position: absolute;
            left: 0;
            color: var(--color-success);
            font-weight: bold;
        }

        .quantity-controls {
            display: flex;
            align-items: center;
            gap: 0.8rem;
            margin-bottom: 1.5rem;
            padding: 0.8rem;
            background: var(--color-light);
            border-radius: 10px;
        }

        .quantity-btn {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            border: 2px solid var(--color-primary);
            background: white;
            color: var(--color-primary);
            font-size: 1.3rem;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            font-weight: bold;
        }

        .quantity-btn:hover {
            background: var(--color-primary);
            color: white;
            transform: scale(1.1);
        }

        .quantity-display {
            min-width: 50px;
            text-align: center;
            font-size: 1.4rem;
            font-weight: 700;
            color: var(--color-text);
        }

        .unit-price {
            color: #777;
            font-size: 0.9rem;
            margin-top: 0.3rem;
        }

        .product-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: auto;
            padding-top: 1rem;
            border-top: 1px solid var(--color-border);
        }

        .product-price {
            font-size: 1.6rem;
            color: var(--color-secondary);
            font-weight: 700;
        }

        .add-to-cart-btn {
            background: linear-gradient(135deg, var(--color-primary) 0%, #1a6a6e 100%);
            color: white;
            border: none;
            border-radius: 10px;
            padding: 1rem 2rem;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            letter-spacing: 0.5px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            box-shadow: 0 4px 15px rgba(32, 128, 133, 0.2);
        }

        .add-to-cart-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(32, 128, 133, 0.3);
            background: linear-gradient(135deg, #1a6a6e 0%, var(--color-primary) 100%);
        }

        /* Cart Summary */
        .cart-summary {
            background: white;
            border-radius: 15px;
            padding: 2.5rem;
            box-shadow: 0 4px 25px rgba(0, 0, 0, 0.1);
            margin-top: 3rem;
            position: sticky;
            bottom: 20px;
            border: 2px solid var(--color-accent);
        }

        .cart-title {
            font-size: 1.6rem;
            color: var(--color-primary);
            margin-bottom: 1.8rem;
            font-weight: 500;
            display: flex;
            align-items: center;
            gap: 0.8rem;
        }

        .selected-items {
            margin-bottom: 1.8rem;
            max-height: 350px;
            overflow-y: auto;
            padding-right: 0.5rem;
        }

        .selected-items::-webkit-scrollbar {
            width: 6px;
        }

        .selected-items::-webkit-scrollbar-track {
            background: var(--color-light);
            border-radius: 3px;
        }

        .selected-items::-webkit-scrollbar-thumb {
            background: var(--color-primary);
            border-radius: 3px;
        }

        .selected-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem;
            background: var(--color-light);
            border-radius: 10px;
            margin-bottom: 1rem;
            font-size: 1rem;
            transition: all 0.3s ease;
            border-left: 4px solid var(--color-primary);
        }

        .selected-item:hover {
            transform: translateX(5px);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }

        .selected-item-info {
            flex-grow: 1;
        }

        .selected-item-name {
            color: var(--color-text);
            font-weight: 600;
            display: block;
            margin-bottom: 0.5rem;
            font-size: 1.1rem;
        }

        .selected-item-quantity {
            color: #777;
            font-size: 0.9rem;
            background: white;
            padding: 0.2rem 0.8rem;
            border-radius: 20px;
            display: inline-block;
        }

        .selected-item-price {
            color: var(--color-secondary);
            font-weight: 700;
            min-width: 120px;
            text-align: right;
            font-size: 1.2rem;
        }

        .remove-btn {
            background: #ff6b6b;
            color: white;
            border: none;
            border-radius: 6px;
            padding: 0.5rem 1rem;
            cursor: pointer;
            font-size: 0.9rem;
            transition: all 0.3s ease;
            margin-left: 1rem;
            font-weight: 600;
        }

        .remove-btn:hover {
            background: #ff5252;
            transform: scale(1.05);
        }

        .cart-total {
            display: flex;
            justify-content: space-between;
            padding: 1.5rem;
            background: linear-gradient(135deg, var(--color-accent) 0%, #e8dfd0 100%);
            border-radius: 10px;
            font-size: 1.4rem;
            font-weight: 700;
            color: var(--color-primary);
            margin-bottom: 1.8rem;
            border: 2px solid var(--color-border);
        }

        .empty-cart {
            text-align: center;
            color: #999;
            padding: 2rem;
            font-style: italic;
            font-size: 1.1rem;
        }

        .checkout-btn {
            width: 100%;
            padding: 1.2rem;
            background: linear-gradient(135deg, var(--color-success) 0%, #45a049 100%);
            color: white;
            border: none;
            border-radius: 10px;
            font-size: 1.2rem;
            font-weight: 700;
            cursor: pointer;
            transition: all 0.3s ease;
            letter-spacing: 1px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.8rem;
            box-shadow: 0 4px 20px rgba(76, 175, 80, 0.2);
        }

        .checkout-btn:hover:not(:disabled) {
            transform: translateY(-3px);
            box-shadow: 0 6px 25px rgba(76, 175, 80, 0.3);
            background: linear-gradient(135deg, #45a049 0%, var(--color-success) 100%);
        }

        .checkout-btn:disabled {
            opacity: 0.5;
            cursor: not-allowed;
            transform: none;
        }

        /* Footer */
        .footer {
            text-align: center;
            padding: 2rem;
            color: #777;
            font-size: 0.9rem;
            margin-top: 3rem;
            border-top: 1px solid var(--color-border);
        }

        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }

            .products-grid {
                grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
                gap: 2rem;
            }

            .cart-summary {
                position: static;
                margin-top: 2rem;
            }

            .header-container {
                flex-direction: column;
                gap: 1rem;
            }

            .intro h2 {
                font-size: 1.6rem;
            }

            .intro p {
                font-size: 1.1rem;
            }

            .offer-banner {
                font-size: 1.1rem;
                padding: 1rem;
            }
        }

        @media (max-width: 480px) {
            .container {
                padding: 1rem;
            }

            .products-grid {
                grid-template-columns: 1fr;
            }

            h1 {
                font-size: 1.8rem;
            }

            .section-title {
                font-size: 1.5rem;
            }

            .product-card:hover {
                transform: translateY(-5px);
            }

            .product-info {
                padding: 1.5rem;
            }

            .add-to-cart-btn {
                padding: 0.8rem 1.2rem;
                font-size: 1rem;
            }

            .quantity-btn {
                width: 35px;
                height: 35px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-container">
            <img src="https://i.ibb.co/1f1tdL5p/Whats-App-Image-2024-12-21-at-15-05-12.jpg" alt="Velarium Logo" class="logo">
            <div>
                <h1>VELARIUM</h1>
                <p class="tagline">Aromaterapia que transforma seu ambiente e sua vida</p>
            </div>
        </div>
    </header>

    <div class="container">
        <div class="intro">
            <h2>✨ Essências que Curam, Energizam e Transformam ✨</h2>
            <p>Cada vela Velarium é uma experiência sensorial única. Criadas com essências 100% naturais, nossas velas não apenas perfumam seu ambiente, mas também equilibram suas emoções, renovam suas energias e transformam qualquer espaço em um santuário de paz e bem-estar.</p>
        </div>

        <div class="offer-banner">
            🎯 PROMOÇÃO ESPECIAL: R$ 15,00 cada | Compre quantas quiser! 🎯
        </div>

        <div class="highlight">
            <h3>🌟 COMBO PERFEITO PARA SUA CASA 🌟</h3>
            <p><strong>Morango Silvestre</strong> para energia e alegria + <strong>Flor de Cerejeira</strong> para paz e relaxamento. A combinação ideal para criar o equilíbrio perfeito no seu lar. Mix de emoções em cada aroma!</p>
        </div>

        <section class="products-section">
            <h3 class="section-title">Escolha suas Essências</h3>
            <div class="products-grid" id="productsGrid"></div>
        </section>
    </div>

    <div class="container">
        <div class="cart-summary">
            <h3 class="cart-title">🛒 Seu Carrinho de Aromas</h3>
            <div class="selected-items" id="selectedItems">
                <div class="empty-cart">Adicione suas essências favoritas aqui</div>
            </div>
            <div class="cart-total">
                <span>Total do Pedido:</span>
                <span id="totalPrice">R$ 0,00</span>
            </div>
            <button class="checkout-btn" id="checkoutBtn" disabled>
                <span>✅ Finalizar Compra Agora</span>
            </button>
        </div>
    </div>

    <div class="footer">
        <p>Velarium &copy; 2024 - Aromaterapia para alma. Todos os direitos reservados.</p>
        <p>Entrega em toda cidade | Enviamos para todo Brasil</p>
    </div>

    <script>
        const products = [
            {
                id: 1,
                name: "Essência de Morango Silvestre",
                description: "Doce, vibrante e revigorante. Esta essência captura a energia pura do verão e a alegria contagiante dos morangos frescos colhidos ao amanhecer. Perfeita para momentos que precisam de um up energético!",
                price: 15.00,
                image: "https://i.ibb.co/1f1tdL5p/Whats-App-Image-2024-12-21-at-15-05-12.jpg",
                benefits: [
                    "Eleva instantaneamente o humor e combate a tristeza",
                    "Estimula a criatividade e pensamento positivo",
                    "Reduz o estresse e ansiedade do dia a dia",
                    "Cria um ambiente acolhedor e energizante",
                    "Ideal para reuniões e momentos criativos"
                ],
                type: "strawberry",
                quantity: 0
            },
            {
                id: 2,
                name: "Essência de Flor de Cerejeira",
                description: "Suave, delicada e harmoniosa. O aroma das cerejeiras em flor traz paz interior profunda e conexão genuína com a natureza. Transforma qualquer quarto em um templo de serenidade.",
                price: 15.00,
                image: "https://i.ibb.co/wt2H7cM/Whats-App-Image-2024-12-21-at-15-05-11.jpg",
                benefits: [
                    "Promove relaxamento profundo e meditação",
                    "Ajuda a aliviar insônia e melhora a qualidade do sono",
                    "Renova as energias e purifica o ambiente",
                    "Facilita a concentração e clareza mental",
                    "Perfeita para yoga e momentos de introspecção"
                ],
                type: "blossom",
                quantity: 0
            }
        ];

        let cart = [];

        function renderProducts() {
            const grid = document.getElementById('productsGrid');
            grid.innerHTML = products.map(product => `
                <div class="product-card ${product.type}">
                    <img src="${product.image}" alt="${product.name}" class="product-image">
                    <div class="product-info">
                        <h4 class="product-name">${product.name}</h4>
                        <p class="product-description">${product.description}</p>
                        
                        <div class="benefits-list">
                            <h4>💫 Benefícios Terapêuticos:</h4>
                            <ul>
                                ${product.benefits.map(benefit => `<li>${benefit}</li>`).join('')}
                            </ul>
                        </div>
                        
                        <div class="quantity-controls">
                            <button class="quantity-btn" onclick="updateQuantity(${product.id}, -1)">-</button>
                            <span class="quantity-display" id="quantity-${product.id}">${product.quantity}</span>
                            <button class="quantity-btn" onclick="updateQuantity(${product.id}, 1)">+</button>
                            <div style="margin-left: auto; text-align: right;">
                                <div style="font-weight: 600; color: var(--color-text);">Quantas você quer?</div>
                                <div class="unit-price">R$ ${product.price.toFixed(2).replace('.', ',')} cada</div>
                            </div>
                        </div>
                        
                        <div class="product-footer">
                            <div>
                                <div style="font-size: 0.9rem; color: #777;">Subtotal:</div>
                                <div class="product-price" id="subtotal-${product.id}">R$ 0,00</div>
                            </div>
                            <button class="add-to-cart-btn" onclick="addToCart(${product.id})">
                                ${product.quantity > 0 ? `🛒 Adicionar ${product.quantity}` : '🛒 Adicionar ao Carrinho'}
                            </button>
                        </div>
                    </div>
                </div>
            `).join('');
            
            // Update subtotals
            products.forEach(product => {
                updateSubtotal(product.id);
            });
        }

        function updateQuantity(productId, change) {
            const product = products.find(p => p.id === productId);
            const newQuantity = Math.max(0, product.quantity + change);
            product.quantity = newQuantity;
            
            document.getElementById(`quantity-${productId}`).textContent = newQuantity;
            const btn = document.querySelector(`[onclick="addToCart(${productId})"]`);
            btn.innerHTML = newQuantity > 0 ? `🛒 Adicionar ${newQuantity}` : '🛒 Adicionar ao Carrinho';
            
            updateSubtotal(productId);
        }

        function updateSubtotal(productId) {
            const product = products.find(p => p.id === productId);
            const subtotal = product.price * product.quantity;
            document.getElementById(`subtotal-${productId}`).textContent = `R$ ${subtotal.toFixed(2).replace('.', ',')}`;
        }

        function addToCart(productId) {
            const product = products.find(p => p.id === productId);
            
            if (product.quantity === 0) {
                alert(`❌ Selecione pelo menos 1 unidade de "${product.name}"`);
                return;
            }
            
            // Remove if already in cart
            cart = cart.filter(item => item.id !== productId);
            
            // Add with quantity
            cart.push({
                id: product.id,
                name: product.name,
                price: product.price,
                quantity: product.quantity,
                type: product.type
            });
            
            // Reset quantity
            product.quantity = 0;
            document.getElementById(`quantity-${productId}`).textContent = '0';
            const btn = document.querySelector(`[onclick="addToCart(${productId})"]`);
            btn.innerHTML = '🛒 Adicionar ao Carrinho';
            updateSubtotal(productId);
            
            renderCart();
            
            // Success animation
            const cartTitle = document.querySelector('.cart-title');
            cartTitle.style.color = 'var(--color-success)';
            setTimeout(() => {
                cartTitle.style.color = 'var(--color-primary)';
            }, 1000);
        }

        function renderCart() {
            const selectedItemsDiv = document.getElementById('selectedItems');
            const checkoutBtn = document.getElementById('checkoutBtn');
            const totalPriceSpan = document.getElementById('totalPrice');

            if (cart.length === 0) {
                selectedItemsDiv.innerHTML = '<div class="empty-cart">Adicione suas essências favoritas aqui</div>';
                checkoutBtn.disabled = true;
            } else {
                selectedItemsDiv.innerHTML = cart.map(item => `
                    <div class="selected-item">
                        <div class="selected-item-info">
                            <span class="selected-item-name">${item.name}</span>
                            <span class="selected-item-quantity">${item.quantity} unidade${item.quantity > 1 ? 's' : ''}</span>
                        </div>
                        <span class="selected-item-price">R$ ${(item.price * item.quantity).toFixed(2).replace('.', ',')}</span>
                        <button class="remove-btn" onclick="removeFromCart(${item.id})">✕ Remover</button>
                    </div>
                `).join('');
                checkoutBtn.disabled = false;
            }

            const total = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);
            totalPriceSpan.textContent = `R$ ${total.toFixed(2).replace('.', ',')}`;
        }

        function removeFromCart(productId) {
            cart = cart.filter(item => item.id !== productId);
            renderCart();
        }

        function handleCheckout() {
            if (cart.length === 0) return;
            
            const total = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);
            const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);
            
            let productsList = '';
            cart.forEach(item => {
                productsList += `• ${item.name}: ${item.quantity} unidade${item.quantity > 1 ? 's' : ''} - R$ ${(item.price * item.quantity).toFixed(2).replace('.', ',')}\n`;
            });
            
            const message = `🎉 COMPRA CONFIRMADA! 🎉\n\nObrigado por escolher a aromaterapia Velarium!\n\n📋 SEU PEDIDO:\n${productsList}\n📦 Total de itens: ${totalItems}\n💰 VALOR TOTAL: R$ ${total.toFixed(2).replace('.', ',')}\n\n📱 Iremos entrar em contato pelo WhatsApp em até 24 horas para combinar a entrega!\n\n💝 Que suas essências tragam paz, energia e muito amor ao seu lar!\n\n✨ Aromaterapia que transforma vidas ✨`;
            
            alert(message);
            
            // Reset cart
            cart = [];
            renderCart();
            
            // Confetti effect simulation
            const checkoutBtn = document.getElementById('checkoutBtn');
            checkoutBtn.innerHTML = '🎉 COMPRA FINALIZADA! 🎉';
            checkoutBtn.style.background = 'linear-gradient(135deg, #FF9800 0%, #FF5722 100%)';
            setTimeout(() => {
                checkoutBtn.disabled = true;
                checkoutBtn.innerHTML = '✅ Finalizar Compra Agora';
                checkoutBtn.style.background = 'linear-gradient(135deg, var(--color-success) 0%, #45a049 100%)';
            }, 3000);
        }

        document.getElementById('checkoutBtn').addEventListener('click', handleCheckout);

        // Initial render
        renderProducts();
        renderCart();
        
        // Initial animation
        setTimeout(() => {
            const cards = document.querySelectorAll('.product-card');
            cards.forEach((card, index) => {
                setTimeout(() => {
                    card.style.opacity = '1';
                    card.style.transform = 'translateY(0)';
                }, index * 200);
            });
        }, 500);
    </script>
</body>
</html>
