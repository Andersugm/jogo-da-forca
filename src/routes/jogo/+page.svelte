<script>
  // @ts-nocheck
  import { onMount } from "svelte";
  import { text } from "@sveltejs/kit";
  import style from "../../style/style.css";
  // @ts-nocheck

  let count = 0;
  let categoria = "país";
  let algum = "";
  let paises = ["BRASIL","ANGOLA", "GUIANA", "EQUADOR", "CHILE", "CHINA","PORTUGAL","PERU", 'FINLANDIA','CUBA', "VENEZUELA", "ARGENTINA", "MEXICO", "AUSTRIA"];

  let letras = 6;
  
  function palavra() {
    const indexPalavras = Math.floor(Math.random() * paises.length);
    algum = paises[indexPalavras];
    console.log(indexPalavras, algum);
  }
  palavra();
  
  export let divs = [
    { id: "letras1", content: "" },
  ];
  

  
  let letraClick = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-A");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };
  let letraClickB = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-B");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickC = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-C");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };
  console.log(count);
  let letraClickD = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-D");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickE = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-E");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickF = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-F");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickG = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-G");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickH = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-H");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickI = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-I");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickJ = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-J");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickK = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-K");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickL = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-L");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickM = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-M");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickN = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-N");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickO = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-O");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickP = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-P");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickQ = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-Q");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickR = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-R");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickS = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-S");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickT = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-T");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;

          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };
  let letraClickU = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-U");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickV = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-V");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickW = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-W");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickX = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-X");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickY = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-Y");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };

  let letraClickZ = function substituirLetra() {
    let check = true;
    const button = document.querySelector(".tecla-Z");
    let j = button.value;

    for (let i = 0; i <= algum.length; i++) {
      if (algum[i] === button.value) {
        if (i === 0) {
          const div = document.querySelector(".letras1");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 1) {
          const div = document.querySelector(".letras2");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 2) {
          const div = document.querySelector(".letras3");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;

          event.target.disabled = true;
        }
        if (i === 3) {
          const div = document.querySelector(".letras4");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 4) {
          const div = document.querySelector(".letras5");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 5) {
          const div = document.querySelector(".letras6");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 6) {
          const div = document.querySelector(".letras7");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 7) {
          const div = document.querySelector(".letras8");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 8) {
          const div = document.querySelector(".letras9");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
        if (i === 9) {
          const div = document.querySelector(".letras10");
          const newDiv = document.createElement("div");
          newDiv.textContent = j;
          div.append(newDiv);
          check = false;
          event.target.disabled = true;
        }
      } else if (i === algum.length && check) {
        const letraErrada = document.querySelector(".LetraErrada");
        const LERR = document.createElement("div");
        LERR.textContent = j;
        letraErrada.append(LERR);
        const errar = document.querySelector(".numero");
        const conterro = document.createElement("img");
        conterro.style.width = "30px";
        conterro.style.marginLeft = "3px";
        conterro.style.marginTop = "10px";
        conterro.src = "X.png";
        errar.append(conterro);
        count += 1;
        if (count == 6) {
          const Perdeu = document.querySelector(".resultado");
          const Perdedor = document.createElement("div");
          Perdedor.textContent = "YOU LOSE";
          Perdeu.append(Perdedor);
          console.log(count);
          return (event.target.disabled = true);
        } else {
          return (event.target.disabled = true);
        }
      }
    }
  };
function sortear(){
    if(algum.length < 9){
      const div = document.querySelector(".letras9");
      div.remove();
    }
    if(algum.length < 8){
      const div = document.querySelector(".letras8");
      div.remove();
    }
    if(algum.length < 7){
      const div = document.querySelector(".letras7");
      div.remove();
    }
    if(algum.length < 6){
      const div = document.querySelector(".letras6");
      div.remove();
    }
    if(algum.length < 5){
      const div = document.querySelector(".letras5");
      div.remove();
    }
    if(algum.length < 4){
      const div = document.querySelector(".letras4");
      div.remove();
    }
}
</script>

<div class="jogo">
  <div class="resultado"></div>
  <div class="LetraErrada">
    <header>Letras <br> Erradas</header>
  </div>
  
  <div class="ajustar">
    <button class="ajuste" on:click={sortear}>Sortear</button>
  </div>


  <div class="erros">
    <div class="numero"></div>
  </div>
  <title>Jogo da forca</title>
  <div class="container">
    <div id="categoria">
      {categoria}
    </div>

    <div class="palavra-secreta">
      {#each divs as div}
        <div class="letras1">
          {div["content"]}
        </div>
        <div class="letras2">
          {div["content"]}
        </div>
        <div class="letras3">
          {div["content"]}
        </div>
        <div class="letras4">
          {div["content"]}
        </div>
        <div class="letras5">
          {div["content"]}
        </div>
        <div class="letras6">
          {div["content"]}
        </div>
        <div class="letras7">
          {div["content"]}
        </div>
        <div class="letras8">
          {div["content"]}
        </div>
        <div class="letras9">
          {div["content"]}
        </div>
      {/each}
    </div>
    <div class="teclado">
      <div class="teclas">
        <button class="tecla-A" value="A" on:click={letraClick}>A</button>
        <button class="tecla-B" value="B" on:click={letraClickB}>B</button>
        <button class="tecla-C" value="C" on:click={letraClickC}>C</button>
        <button class="tecla-D" value="D" on:click={letraClickD}>D</button>
        <button class="tecla-E" value="E" on:click={letraClickE}>E</button>
        <button class="tecla-F" value="F" on:click={letraClickF}>F</button>
        <button class="tecla-G" value="G" on:click={letraClickG}>G</button>
        <button class="tecla-H" value="H" on:click={letraClickH}>H</button>
        <button class="tecla-I" value="I" on:click={letraClickI}>I</button>
      </div>
      <div class="teclas" id="teclas1">
        <button class="tecla-J" value="J" on:click={letraClickJ}>J</button>
        <button class="tecla-K" value="K" on:click={letraClickK}>K</button>
        <button class="tecla-L" value="L" on:click={letraClickL}>L</button>
        <button class="tecla-M" value="M" on:click={letraClickM}>M</button>
        <button class="tecla-N" value="N" on:click={letraClickN}>N</button>
        <button class="tecla-O" value="O" on:click={letraClickO}>O</button>
        <button class="tecla-P" value="P" on:click={letraClickP}>P</button>
        <button class="tecla-Q" value="Q" on:click={letraClickQ}>Q</button>
        <button class="tecla-R" value="R" on:click={letraClickR}>R</button>
      </div>
      <div class="teclas" id="teclas1">
        <button class="tecla-S" value="S" on:click={letraClickS}>S</button>
        <button class="tecla-T" value="T" on:click={letraClickT}>T</button>
        <button class="tecla-U" value="U" on:click={letraClickU}>U</button>
        <button class="tecla-V" value="V" on:click={letraClickV}>V</button>
        <button class="tecla-W" value="W" on:click={letraClickW}>W</button>
        <button class="tecla-X" value="X" on:click={letraClickX}>X</button>
        <button class="tecla-Y" value="Y" on:click={letraClickY}>Y</button>
        <button class="tecla-Z" value="Z" on:click={letraClickZ}>Z</button>
      </div>
    </div>
  </div>
</div>
<div class="back">
  <button class="buttonBack"><a href="/">Voltar</a></button>
</div>
<div class="reset">
  <button class="buttonreset" on:click={() => window.location.reload()}>Reiniciar</button>
</div>

