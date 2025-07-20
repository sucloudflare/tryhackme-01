<h1>🏴‍☠️ Como hackeei o FakeBank no TryHackMe</h1>

  <p>Durante o desafio do <strong>TryHackMe</strong>, explorei uma aplicação bancária fictícia chamada <em>FakeBank</em> para simular um ataque realista como hacker ético. Veja o passo a passo abaixo:</p>

  <h2>🧭 1. Descoberta de diretórios com Gobuster</h2>
  <p>Utilizei a ferramenta <code>Gobuster</code> para encontrar páginas ocultas no site. O comando foi:</p>

  <div class="caixa">
    <code>gobuster -u http://fakebank.thm -w wordlist.txt dir</code>
  </div>

  <p>Isso revelou a página <code>/bank-transfer</code>, que estava acessível sem autenticação.</p>

  <h2>🏦 2. Acesso ao formulário de transferência</h2>
  <p>Ao acessar <code>/bank-transfer</code>, encontrei um formulário que permitia transferir dinheiro entre contas. Realizei a seguinte operação:</p>
  <ul>
    <li>De: conta <strong>2276</strong></li>
    <li>Para: minha conta <strong>8881</strong></li>
    <li>Valor: <strong>$2000</strong></li>
  </ul>

  <p>Essa vulnerabilidade simula o que seria um <strong>acesso indevido a funções críticas</strong> da aplicação.</p>

  <h2>🎯 3. Captura da flag</h2>
  <p>Após a transferência, acessei a página da minha conta e encontrei a mensagem:</p>

  <div class="flag">
    🎉 <strong>Congratulations - you hacked the bank!</strong><br>
    The answer to the TryHackMe question is: <strong>BANK-HACKED</strong>
  </div>

  <h2>💡 Conclusão</h2>
  <p>Esse exercício foi uma ótima introdução à <strong>segurança ofensiva</strong>, onde pratiquei:</p>
  <ul>
    <li>Enumeração de diretórios</li>
    <li>Exploração de funcionalidades mal protegidas</li>
    <li>Reconhecimento e coleta de informações sensíveis</li>
  </ul>

  <p>Esse tipo de simulação ajuda a entender como vulnerabilidades reais podem ser exploradas — e como preveni-las.</p>

  <p>🔐 <em>Essa atividade foi feita em ambiente controlado com permissão total. Nunca tente explorar sistemas reais sem autorização.</em></p>
