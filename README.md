# Stock-haven-Mashla-<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Stock Haven Masala - premium everyday Indian powdered spices.">
  <title>Stock Haven Masala | Pure Taste. Everyday Tradition.</title>
  <style>
    :root{
      --green:#173f2a; --green2:#285c3f; --cream:#fffaf0; --gold:#d99b28;
      --red:#a83222; --ink:#1d241f; --muted:#68706a; --white:#fff;
      --shadow:0 12px 35px rgba(22,40,28,.10); --radius:20px;
    }
    *{box-sizing:border-box;margin:0;padding:0}
    html{scroll-behavior:smooth}
    body{font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;color:var(--ink);background:var(--cream);line-height:1.5}
    button,input,select{font:inherit}
    a{text-decoration:none;color:inherit}
    .container{width:min(1120px,92%);margin:auto}
    header{position:sticky;top:0;z-index:50;background:rgba(255,250,240,.96);backdrop-filter:blur(12px);border-bottom:1px solid #eadfca}
    .nav{height:74px;display:flex;align-items:center;justify-content:space-between;gap:20px}
    .brand{display:flex;align-items:center;gap:10px;font-weight:900;color:var(--green);font-size:1.2rem}
    .logo{width:42px;height:42px;border-radius:13px;background:var(--green);display:grid;place-items:center;color:#fff;font-size:1.35rem;box-shadow:var(--shadow)}
    nav{display:flex;gap:25px;font-weight:650;color:#39433c}
    nav a:hover{color:var(--red)}
    .actions{display:flex;gap:9px;align-items:center}
    .icon-btn{border:1px solid #ded4c1;background:#fff;border-radius:12px;width:42px;height:42px;cursor:pointer;position:relative}
    .cart-count{position:absolute;right:-5px;top:-6px;background:var(--red);color:#fff;font-size:11px;min-width:19px;height:19px;border-radius:50%;display:grid;place-items:center}
    .menu{display:none}
    .hero{padding:70px 0 65px;background:radial-gradient(circle at 85% 20%,#f4ddb1 0 14%,transparent 15%),linear-gradient(135deg,#fffaf0,#f4ecd8)}
    .hero-grid{display:grid;grid-template-columns:1.1fr .9fr;align-items:center;gap:50px}
    .eyebrow{display:inline-block;color:var(--red);font-weight:800;letter-spacing:.08em;text-transform:uppercase;font-size:.8rem;margin-bottom:14px}
    h1{font-size:clamp(2.5rem,6vw,5rem);line-height:.98;color:var(--green);letter-spacing:-.045em}
    .hero p{margin:22px 0;color:var(--muted);font-size:1.08rem;max-width:590px}
    .btn{border:0;border-radius:13px;padding:13px 19px;font-weight:800;cursor:pointer;display:inline-flex;align-items:center;justify-content:center;gap:8px;transition:.2s}
    .btn-primary{background:var(--green);color:#fff}.btn-primary:hover{background:#0e2e1e;transform:translateY(-1px)}
    .btn-outline{background:#fff;color:var(--green);border:1px solid #cfc4af}
    .hero-card{min-height:410px;border-radius:34px;background:linear-gradient(150deg,#1a4a30,#102d20);display:grid;place-items:center;box-shadow:0 25px 70px rgba(16,45,32,.25);position:relative;overflow:hidden}
    .hero-card:before{content:"";position:absolute;width:300px;height:300px;border-radius:50%;background:#e0a92d;opacity:.22;top:-100px;right:-70px}
    .spice-bowl{width:250px;height:250px;border-radius:50%;background:radial-gradient(circle at 35% 28%,#ffd16d 0 7%,transparent 8%),radial-gradient(circle at 65% 45%,#a83222 0 12%,transparent 13%),radial-gradient(circle at 35% 65%,#d99b28 0 14%,transparent 15%),#b94a22;box-shadow:inset 0 -30px 55px rgba(0,0,0,.22),0 25px 35px rgba(0,0,0,.28);border:13px solid #f5d28a}
    .badge{position:absolute;bottom:30px;left:30px;background:#fff;color:var(--green);padding:12px 16px;border-radius:14px;font-weight:900}
    section{padding:75px 0}.section-head{text-align:center;margin-bottom:35px}.section-head h2{font-size:2.25rem;color:var(--green)}.section-head p{color:var(--muted);margin-top:7px}
    .benefits{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:-25px;position:relative}
    .benefit{background:#fff;padding:22px;border-radius:17px;box-shadow:var(--shadow);text-align:center}.benefit strong{display:block;color:var(--green);margin:7px 0}.benefit span{color:var(--muted);font-size:.92rem}
    .products{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}
    .product{background:#fff;border:1px solid #eee4d2;border-radius:20px;overflow:hidden;box-shadow:var(--shadow);display:flex;flex-direction:column}
    .product-img{height:205px;display:grid;place-items:center;background:linear-gradient(145deg,#f8e9c6,#fff8e9);font-size:5rem}
    .product-body{padding:18px;display:flex;flex-direction:column;gap:9px;flex:1}.product h3{color:var(--green);font-size:1.15rem}.product p{font-size:.9rem;color:var(--muted)}
    .product-row{display:flex;align-items:center;justify-content:space-between;margin-top:auto;padding-top:7px}.price{font-weight:900;font-size:1.15rem;color:var(--red)}
    .about{background:#173f2a;color:#fff}.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:50px;align-items:center}.about h2{font-size:2.4rem}.about p{color:#d8e5db;margin:15px 0}.about-box{background:#285c3f;padding:28px;border-radius:25px}.about-box li{list-style:none;padding:12px 0;border-bottom:1px solid rgba(255,255,255,.12)}.about-box li:last-child{border:0}
    .contact{display:grid;grid-template-columns:1fr 1fr;gap:25px}.contact-card{background:#fff;border-radius:20px;padding:25px;box-shadow:var(--shadow)}.contact-card h3{color:var(--green);margin-bottom:12px}.contact-card p{color:var(--muted);margin:8px 0}
    footer{background:#102d20;color:#d8e5db;padding:30px 0}.footer-row{display:flex;justify-content:space-between;gap:20px;flex-wrap:wrap}.footer-brand{font-weight:900;color:#fff}
    .drawer-backdrop{position:fixed;inset:0;background:rgba(0,0,0,.45);z-index:80;display:none}.drawer-backdrop.open{display:block}
    .cart-drawer{position:fixed;right:0;top:0;height:100%;width:min(420px,94vw);background:#fff;z-index:90;transform:translateX(100%);transition:.25s;display:flex;flex-direction:column}
    .cart-drawer.open{transform:translateX(0)}.drawer-head{padding:20px;border-bottom:1px solid #eee;display:flex;justify-content:space-between;align-items:center}.drawer-body{padding:18px;overflow:auto;flex:1}.drawer-foot{padding:18px;border-top:1px solid #eee}
    .cart-item{display:flex;gap:12px;padding:13px 0;border-bottom:1px solid #eee}.cart-emoji{width:55px;height:55px;border-radius:12px;background:#fff3d8;display:grid;place-items:center;font-size:1.7rem}.cart-info{flex:1}.cart-info strong{display:block}.qty{display:flex;align-items:center;gap:8px;margin-top:5px}.qty button{border:1px solid #ddd;background:#fff;border-radius:7px;width:27px;height:27px;cursor:pointer}
    .total{display:flex;justify-content:space-between;font-weight:900;font-size:1.15rem;margin-bottom:13px}.full{width:100%}
    .modal{position:fixed;inset:0;background:rgba(0,0,0,.55);display:none;place-items:center;z-index:100;padding:18px}.modal.open{display:grid}.modal-card{background:#fff;width:min(650px,100%);max-height:90vh;overflow:auto;border-radius:22px;padding:25px}.modal-head{display:flex;justify-content:space-between;align-items:center;margin-bottom:18px}.close{border:0;background:#f2eee5;border-radius:10px;width:38px;height:38px;cursor:pointer}
    .form-grid{display:grid;grid-template-columns:1fr 1fr;gap:14px}.field{display:flex;flex-direction:column;gap:6px}.field.full-field{grid-column:1/-1}.field label{font-weight:700;font-size:.9rem}.field input,.field textarea,.field select{border:1px solid #d8d1c3;border-radius:11px;padding:12px;outline:none}.field input:focus,.field textarea:focus,.field select:focus{border-color:var(--green)}.field textarea{min-height:85px;resize:vertical}
    .empty{text-align:center;color:var(--muted);padding:45px 10px}.notice{padding:12px;background:#eef7ef;border-radius:10px;color:var(--green);font-size:.9rem;margin-bottom:15px}
    @media(max-width:800px){
      nav{display:none}.menu{display:block}.hero-grid,.about-grid,.contact{grid-template-columns:1fr}.hero{padding-top:45px}.hero-card{min-height:300px}.benefits{grid-template-columns:1fr;margin-top:0}.products{grid-template-columns:repeat(2,1fr)}
    }
    @media(max-width:520px){
      .nav{height:65px}.brand{font-size:1rem}.logo{width:36px;height:36px}.hero h1{font-size:2.65rem}.products{grid-template-columns:1fr}.product-img{height:180px}.form-grid{grid-template-columns:1fr}.field.full-field{grid-column:auto}.section-head h2{font-size:1.9rem}
    }
  </style>
</head>
<body>
<header>
  <div class="container nav">
    <a class="brand" href="#home"><span class="logo">🌶️</span>Stock Haven Masala</a>
    <nav>
      <a href="#home">Home</a><a href="#shop">Shop</a><a href="#about">About</a><a href="#contact">Contact</a>
    </nav>
    <div class="actions">
      <button class="icon-btn menu" onclick="toggleMobileNav()" aria-label="Menu">☰</button>
      <button class="icon-btn" onclick="openCart()" aria-label="Cart">🛒<span class="cart-count" id="cartCount">0</span></button>
    </div>
  </div>
</header>

<main>
<section class="hero" id="home">
  <div class="container hero-grid">
    <div>
      <span class="eyebrow">Premium Indian Spices</span>
      <h1>Pure Taste.<br>Everyday Tradition.</h1>
      <p>Freshly packed powdered spices made for everyday Indian cooking. Bring authentic colour, aroma and flavour to your kitchen.</p>
      <div style="display:flex;gap:10px;flex-wrap:wrap">
        <a href="#shop" class="btn btn-primary">Shop Spices →</a>
        <a href="#about" class="btn btn-outline">Our Story</a>
      </div>
    </div>
    <div class="hero-card"><div class="spice-bowl"></div><div class="badge">🌿 Quality • Aroma • Taste</div></div>
  </div>
</section>

<div class="container benefits">
  <div class="benefit">🌱<strong>Quality First</strong><span>Carefully selected ingredients.</span></div>
  <div class="benefit">📦<strong>Freshly Packed</strong><span>Sealed for aroma and freshness.</span></div>
  <div class="benefit">🚚<strong>Easy Delivery</strong><span>Convenient doorstep ordering.</span></div>
</div>

<section id="shop">
  <div class="container">
    <div class="section-head"><h2>Shop Our Spices</h2><p>Everyday essentials for your kitchen.</p></div>
    <div class="products" id="productGrid"></div>
  </div>
</section>

<section class="about" id="about">
  <div class="container about-grid">
    <div><span class="eyebrow" style="color:#f4c85d">About the Brand</span><h2>Made for the food you love.</h2><p>Stock Haven Masala is built around a simple idea: good food starts with good spices. Our range is designed for everyday Indian kitchens, with careful sourcing and hygienic packing.</p><p><strong>Our promise:</strong> honest products, clear pricing and dependable service.</p></div>
    <div class="about-box"><ul><li>🌶️ Authentic everyday flavour</li><li>🧼 Hygienic processing & packing</li><li>📦 Multiple pack sizes</li><li>🤝 Customer-first service</li></ul></div>
  </div>
</section>

<section id="contact">
  <div class="container">
    <div class="section-head"><h2>Contact Stock Haven Masala</h2><p>Questions, bulk orders or wholesale enquiries.</p></div>
    <div class="contact">
      <div class="contact-card"><h3>📱 WhatsApp</h3><p>For quick orders and support.</p><a class="btn btn-primary" id="waLink" target="_blank" rel="noopener">Chat on WhatsApp</a></div>
      <div class="contact-card"><h3>📍 Business Details</h3><p>Email: <span id="emailText">hello@stockhavenmasala.in</span></p><p>Phone: +91 81012 03958</p><p>India • Delivery across selected locations</p></div>
    </div>
  </div>
</section>
</main>

<footer><div class="container footer-row"><div class="footer-brand">🌶️ Stock Haven Masala</div><div>© <span id="year"></span> Stock Haven Masala. All rights reserved.</div></div></footer>

<div class="drawer-backdrop" id="backdrop" onclick="closeCart()"></div>
<aside class="cart-drawer" id="cartDrawer">
  <div class="drawer-head"><h2>Your Cart</h2><button class="close" onclick="closeCart()">✕</button></div>
  <div class="drawer-body" id="cartItems"></div>
  <div class="drawer-foot"><div class="total"><span>Total</span><span id="cartTotal">₹0</span></div><button class="btn btn-primary full" onclick="openCheckout()">Proceed to Checkout</button></div>
</aside>

<div class="modal" id="checkoutModal">
  <div class="modal-card">
    <div class="modal-head"><h2>Checkout</h2><button class="close" onclick="closeCheckout()">✕</button></div>
    <div class="notice">This demo checkout supports Cash on Delivery and WhatsApp order confirmation.</div>
    <form id="checkoutForm">
      <div class="form-grid">
        <div class="field"><label>Full name *</label><input name="name" required placeholder="Your name"></div>
        <div class="field"><label>Phone *</label><input name="phone" required inputmode="tel" placeholder="+91"></div>
        <div class="field full-field"><label>Delivery address *</label><textarea name="address" required placeholder="House, street, village/city, PIN"></textarea></div>
        <div class="field"><label>PIN code *</label><input name="pin" required inputmode="numeric" maxlength="6" placeholder="6-digit PIN"></div>
        <div class="field"><label>Payment</label><select name="payment"><option>Cash on Delivery</option><option>Online Payment (connect gateway)</option></select></div>
      </div>
      <div style="margin-top:18px"><button class="btn btn-primary full" type="submit">Place Order</button></div>
    </form>
  </div>
</div>

<script>
  const products = [
    {id:1,name:"Red Chilli Powder",emoji:"🌶️",price:89,weight:"100g",desc:"Bold colour and balanced heat."},
    {id:2,name:"Turmeric Powder",emoji:"🟡",price:69,weight:"100g",desc:"Aromatic turmeric for everyday cooking."},
    {id:3,name:"Coriander Powder",emoji:"🌿",price:79,weight:"100g",desc:"Fresh, earthy flavour for curries."},
    {id:4,name:"Cumin Powder",emoji:"🟤",price:99,weight:"100g",desc:"Warm aroma with a rich, nutty taste."},
    {id:5,name:"Garam Masala",emoji:"🔥",price:129,weight:"100g",desc:"A fragrant blend for Indian dishes."},
    {id:6,name:"Biryani Masala",emoji:"🍛",price:139,weight:"100g",desc:"Aromatic blend for delicious biryani."}
  ];

  let cart = JSON.parse(localStorage.getItem("shmCart") || "[]");

  function money(n){return "₹"+n.toLocaleString("en-IN")}
  function save(){localStorage.setItem("shmCart",JSON.stringify(cart));renderCart()}
  function renderProducts(){
    document.getElementById("productGrid").innerHTML = products.map(p => `
      <article class="product">
        <div class="product-img">${p.emoji}</div>
        <div class="product-body">
          <h3>${p.name}</h3><p>${p.desc}</p><small>${p.weight} pack</small>
          <div class="product-row"><span class="price">${money(p.price)}</span><button class="btn btn-primary" onclick="addToCart(${p.id})">Add to Cart</button></div>
        </div>
      </article>`).join("");
  }
  function addToCart(id){
    const item=cart.find(x=>x.id===id);
    if(item)item.qty++; else cart.push({id,qty:1});
    save(); openCart();
  }
  function changeQty(id,d){
    const item=cart.find(x=>x.id===id); if(!item)return;
    item.qty+=d; if(item.qty<=0)cart=cart.filter(x=>x.id!==id); save();
  }
  function renderCart(){
    const box=document.getElementById("cartItems");
    if(!cart.length){box.innerHTML='<div class="empty">Your cart is empty.<br><br>🌶️ Add some spices to get started.</div>'}
    else box.innerHTML=cart.map(i=>{const p=products.find(x=>x.id===i.id);return `
      <div class="cart-item"><div class="cart-emoji">${p.emoji}</div><div class="cart-info"><strong>${p.name}</strong><span>${money(p.price)} × ${i.qty}</span>
      <div class="qty"><button onclick="changeQty(${p.id},-1)">−</button><span>${i.qty}</span><button onclick="changeQty(${p.id},1)">+</button></div></div><strong>${money(p.price*i.qty)}</strong></div>`}).join("");
    const total=cart.reduce((s,i)=>s+products.find(p=>p.id===i.id).price*i.qty,0);
    document.getElementById("cartTotal").textContent=money(total);
    document.getElementById("cartCount").textContent=cart.reduce((s,i)=>s+i.qty,0);
  }
  function openCart(){document.getElementById("cartDrawer").classList.add("open");document.getElementById("backdrop").classList.add("open")}
  function closeCart(){document.getElementById("cartDrawer").classList.remove("open");document.getElementById("backdrop").classList.remove("open")}
  function openCheckout(){
    if(!cart.length){alert("Please add a product to your cart first.");return}
    document.getElementById("checkoutModal").classList.add("open");closeCart();
  }
  function closeCheckout(){document.getElementById("checkoutModal").classList.remove("open")}
  function toggleMobileNav(){
    const nav=document.querySelector("nav");
    const open=nav.style.display==="flex";
    nav.style.display=open?"none":"flex";
    nav.style.position="absolute";nav.style.top="65px";nav.style.left="0";nav.style.right="0";
    nav.style.background="#fffaf0";nav.style.padding="18px 4%";nav.style.flexDirection="column";nav.style.borderBottom="1px solid #eadfca";
  }
  document.getElementById("checkoutForm").addEventListener("submit",e=>{
    e.preventDefault();
    const data=new FormData(e.target);
    const total=cart.reduce((s,i)=>s+products.find(p=>p.id===i.id).price*i.qty,0);
    const lines=cart.map(i=>{const p=products.find(x=>x.id===i.id);return `${p.name} x ${i.qty} = ${money(p.price*i.qty)}`}).join("\n");
    const message=`Hello Stock Haven Masala!%0A%0AI want to place an order.%0A%0A${encodeURIComponent(lines)}%0A%0ATotal: ${money(total)}%0AName: ${encodeURIComponent(data.get("name"))}%0APhone: ${encodeURIComponent(data.get("phone"))}%0AAddress: ${encodeURIComponent(data.get("address"))}%0APIN: ${encodeURIComponent(data.get("pin"))}%0APayment: ${encodeURIComponent(data.get("payment"))}`;
    window.open("https://wa.me/918101203958?text="+message,"_blank");
    cart=[];save();closeCheckout();alert("Your order details were prepared for WhatsApp. Replace the demo WhatsApp number in the code with your real business number.");
  });
  document.getElementById("waLink").href="https://wa.me/918101203958?text=Hello%20Stock%20Haven%20Masala%2C%20I%20want%20to%20order%20spices.";
  document.getElementById("year").textContent=new Date().getFullYear();
  renderProducts();renderCart();
</script>
</body>
</html>
