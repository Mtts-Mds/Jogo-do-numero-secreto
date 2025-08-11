alert('Boas-vindas ao jogo do número secreto');
let numeroSecreto = 4;
console.log(numeroSecreto);
let chute; 
let tentativas = 1;

// enquanto o chute não for igual ao n.s
while (chute != numeroSecreto) {
     chute = prompt('Escolha um número entre 1 e 20');
    // se o numero for igual ao número secreto
      if (chute == numeroSecreto) {
     alert (`Isso aí! Você descobriu o número secreto ${numeroSecreto} com ${tentativas} tentativas.`);
     } else {
     if (chute > numeroSecreto) {
          alert(`o numero secreto é menor que ${chute}`);
       }  else {
           alert(`o numero secreto é maior que ${chute}`);    
          } 
          tentativas++;
     }
}
