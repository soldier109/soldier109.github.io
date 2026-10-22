# soldier109.github.io
*{ margin:0; padding:0; box-sizing:border-box; }

html{ scroll-behavior:smooth; }

body{
  font-family: "Segoe UI", system-ui, -apple-system, Arial, sans-serif;
  background: #f7f8fa;
  color: #1f2430;
  line-height: 1.6;
  font-size: 16px;
}

a{ color: inherit; }

.container{
  max-width: 820px;
  margin: 0 auto;
  padding: 0 24px;
}

/*==========================*/
.nav{
  position: sticky;
  top: 0;
  z-index: 10;
  background: rgba(247,248,250,.9);
  backdrop-filter: blur(8px);
  border-bottom: 1px solid #e5e7eb;
}
.nav-inner{
  max-width: 820px;
  margin: 0 auto;
  padding: 16px 24px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
}
.logo{
  font-weight: 700;
  text-decoration: none;
  font-size: 1rem;
}
.nav-links{
  display: flex;
  gap: 22px;
  list-style: none;
  font-size: .9rem;
}
.nav-links a{
  color: #5b6475;
  text-decoration: none;
  transition: color .2s;
}
.nav-links a:hover{ color: #1f2430; }

/*==========================*/
.hero{
  padding: 80px 0 60px;
}
.hero h1{
  font-size: clamp(2rem, 5vw, 2.8rem);
  font-weight: 800;
  letter-spacing: -.02em;
}
.role{
  margin-top: 12px;
  color: #5b6475;
  font-size: 1.05rem;
}
.hero-text{
  margin-top: 18px;
  max-width: 560px;
  color: #444b5b;
}
.actions{
  margin-top: 28px;
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}
.btn{
  display: inline-block;
  padding: 11px 22px;
  border-radius: 8px;
  font-size: .92rem;
  font-weight: 600;
  text-decoration: none;
  background: #1f2430;
  color: #fff;
  border: 1px solid #1f2430;
  transition: background .2s, color .2s;
}
.btn:hover{ background: #2d3444; }
.btn-outline{
  background: transparent;
  color: #1f2430;
}
.btn-outline:hover{
  background: #1f2430;
  color: #fff;
}

/*==========================*/
.section{
  padding: 56px 0;
  border-top: 1px solid #e5e7eb;
}
.section.alt{
  background: #ffffff;
}
.section h2{
  font-size: 1.4rem;
  font-weight: 700;
  margin-bottom: 20px;
}
.section p{
  color: #444b5b;
  margin-bottom: 12px;
}

/*==========================*/
.skills{
  list-style: none;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 12px 32px;
}
.skills li{
  display: flex;
  justify-content: space-between;
  padding: 8px 0;
  border-bottom: 1px dashed #e5e7eb;
  font-size: .95rem;
}
.skills .level{
  color: #7a8395;
  font-size: .85rem;
}

/*==========================*/
.item{
  margin-bottom: 24px;
}
.item:last-child{ margin-bottom: 0; }
.item h3{
  font-size: 1.05rem;
  font-weight: 700;
  margin-bottom: 4px;
}
.item .meta{
  font-size: .85rem;
  color: #7a8395;
  margin-bottom: 6px;
}
.item p{
  font-size: .95rem;
}

/*==========================*/
.contact p{
  margin-bottom: 20px;
}
.contacts{
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
}
.contacts a{
  display: inline-block;
  padding: 9px 18px;
  border-radius: 8px;
  border: 1px solid #e5e7eb;
  background: #fff;
  text-decoration: none;
  font-size: .9rem;
  font-weight: 600;
  transition: border-color .2s, color .2s;
}
.contacts a:hover{
  border-color: #1f2430;
  color: #1f2430;
}

/*==========================*/
footer{
  border-top: 1px solid #e5e7eb;
  padding: 24px 0;
  text-align: center;
  font-size: .82rem;
  color: #7a8395;
}

/*==========================*/
@media (max-width: 640px){
  .nav-links{ display: none; }
  .hero{ padding: 56px 0 40px; }
  .section{ padding: 44px 0; }
  .skills{ grid-template-columns: 1fr; }
}

/* ===== HERO С КАРТИНКОЙ ===== */
.hero-grid{
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  gap: 36px;
  align-items: center;
}

.hero-text-block{
  min-width: 0;
}

.hero-grid .hero-text{
  max-width: 100%;
}

.hero-image{
  margin: 0;
}

.hero-image img{
  display: block;
  width: 100%;
  height: auto;
  max-height: 360px;
  object-fit: cover;
  border-radius: 14px;
  border: 1px solid #e5e7eb;
}

@media (max-width: 760px){
  .hero-grid{
    grid-template-columns: 1fr;
    gap: 24px;
  }
}
