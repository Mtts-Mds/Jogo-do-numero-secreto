alert('Boas-vindas ao jogo do número secreto');
let numeroMmaximo = 100;
let numeroSecreto = parseInt(Math.random() * numeroMmaximo + 1);
console.log(numeroSecreto);
let chute; 
let tentativas = 1;
while (chute != numeroSecreto) {
     chute = prompt(`Escolha um número entre 1 e ${numeroMmaximo}`);
      if (chute == numeroSecreto) {
          break
     } else {
     if (chute > numeroSecreto) {
          alert(`o numero secreto é menor que ${chute}`);
       }  else {
           alert(`o numero secreto é maior que ${chute}`);    
          } 
          tentativas++;
     }
}
let palavraTentativas = tentativas > 1 ? 'tentativas' : 'tentatibas';
alert (`Isso aí! Você descobriu o número secreto ${numeroSecreto} com ${tentativas} ${palavraTentativas}.`);  
