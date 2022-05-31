# Nike
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="style.css" />
    <title>Nike</title>
  </head>
  <body>
    <style>
      *{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --button: #FF0000;
  --main-background:  #C4C4C4;
  --background: #E5E5E5;
  --text: #000;
  --footer: #000;
  --text-description: #9C9696;
}

body{
  width: 90rem;
  height: 67.5rem;

  font-family: 'Roboto', sans-serif;

  background: var(--background);
  
  display: grid;
  grid-template-areas: 
     "nav main"
     "header main"
     "footer footer"  
  ;
}

#nav{
  position: absolute;
  grid-area: nav;
  display: flex;
  width: 82.5rem;
  height: 3rem;
  margin-inline: 3.75rem;
  margin-top: 2.43rem;
  justify-content: space-between;
  align-items: center;
}

.list{
  display: flex;
  gap: 5rem;
  margin-left: 4rem;
  text-align: center;
  list-style-type: none;

  font-weight: 700;
  font-size: 1.5rem;
  line-height: 1.75rem;
}

.list a{
  text-decoration: none;
  color: var(--text);
}

#nav input{
  width: 13.75rem;
  height: 2.81rem;

  margin-right: 5.12rem;
  padding-left: 2.62rem;

  font-family: 'Roboto', sans-serif;
  font-weight: 500;
  font-size: 1.12rem;

  border: none;
}

.lupa{
  position: relative;
  left: 5rem;
}

main{
  grid-area: main ;
  width: 56.25rem;
  height: 57.12rem;
  background: var(--main-background);
  margin-left: auto; 
}

main img{
  margin-top: 10.7rem;
}

.first{
  width: 37.31rem;
  height: 31.8rem;
  /* align-items: center; */
  margin-left: 7rem;
}

.photos{
  width: 16rem;
  position: relative;
  bottom: 10rem;
  margin-left: 1.12rem;
  display: flex;
  justify-content: space-between;
  gap: 2.31rem;

  cursor: pointer;
}

#main .choice{
  height: 11.74rem;
  border-bottom: 0.25rem solid var(--button);
}

header{
  grid-area: header;
  width: 22.31rem;
  height: 33.31rem;
  margin-left: 6.93rem;
  position: relative;
  bottom: 10rem;
}

header h1{
  margin-bottom: 1.31rem;
  font-size: 3.75rem;
  color: var(--text);
}

header p{
  margin-bottom: 1.31rem;
  font-size: 1rem;
  font-weight: 700;
  color: var(--text-description);
}

header h2{
  margin-bottom: 1.87rem;
  font-size: 2.5rem;
  font-weight: 700;
  color: var(--text);
}

header button{
  width: 17.12rem;
  height: 5.62rem;

  background-color: var(--button);
  
  border: none;
  color: var(--background);

  font-family: 'Roboto', sans-serif;
  font-size: 1.5rem;
  font-weight: 700;

  cursor: pointer;
}

footer{
  grid-area: footer;
  height: 10.39rem;
  display: flex;
} 

footer iframe{
  width: 15.62rem;
  height: 10.39rem;
}

.contact{
  display: flex;
  gap: 5.6rem;
  list-style-type: none;
  margin-top: 4.43rem;
  margin-left: 2.9rem;
}

.contact a{
  text-decoration: none;
  color: var(--text);
  font-family: 'Roboto', sans-serif;
  font-size: 1.12rem;
  font-weight: 700;
}

footer button{
  width: 27.31rem;
  height: 10.4rem;
  margin-left: 12rem;
  
  
  background-color: var(--footer);
  color: var(--background);
  border: 1rem var(--footer);

  font-size: 1.5rem;
  font-weight: 700;

  cursor: pointer;
}
    </style>
    <nav id="nav">
      <a href="#"><img src="/assets/logo.svg" alt="tenis" /></a>
      <ul class="list">
        <li><a href="#">HOMEM</a></li>
        <li><a href="#">MULHER</a></li>
        <li><a href="#">CRIANÇA</a></li>
        <li><a href="#">CUSTOMIZAR</a></li>
      </ul>
      <img class="lupa" src="/assets/icon-search.svg" alt="" />
      <input type="search" placeholder="Pesquisar" />
      <a href="#"><img src="/assets/icon-bag.svg" alt="" /></a>
    </nav>
    <header id="header">
      <h1>
        Tênis <br />
        Esportivo <br />
        Para Corrida <br />
        Top
      </h1>
      <p>
        Esse tênis tem o intuito de te deixar ainda mais fitness, focado, e
        musculoso.
      </p>
      <h2>R$ 1.000,00</h2>
      <button>COMPRAR</button>
    </header>
    <main id="main">
      <img class="first" src="/assets/tenis-1-ampliado.png" alt="" />
      <div class="photos">
        <img src="/assets/tenis-1-galeria.png" alt="" />
        <img class="choice" src="/assets/tenis-2-galeria.png" alt="" />
        <img src="/assets/tenis-3-galeria.png" alt="" />
      </div>
    </main>
    <footer id="footer">
      <iframe
        width="699"
        height="393"
        src="https://www.youtube.com/embed/S1-QwIRjM-A"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
      <ul class="contact">
        <li><a href="#">FACEBOOK</a></li>
        <li><a href="#">INSTAGRAM</a></li>
        <li><a href="#">YOUTUBE</a></li>
        <li><a href="#">TWITTER</a></li>
      </ul>
      <button>EXPLORE MAIS</button>
    </footer>
  </body>
</html>
