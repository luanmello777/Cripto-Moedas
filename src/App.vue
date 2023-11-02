<template> 
  <v-app class="bg-yellow-lighten-3">
    <v-app-bar class="bg-yellow-accent-4 elevation-24">

      <v-app-bar-title>
        <h2 class="font d-flex justify-center align-center">CriptoMoedas</h2>
      </v-app-bar-title>

    </v-app-bar>
    
    <br>

    <v-container class="bg-yellow-accent-4 mt-16 d-flex justify-space-between elevation-24">

      <div>
        <v-parallax src="/criptomoedas.jpg" width="600" :class="smAndDown ? 'w-0 h-0' : ''" />
      </div>

      <div>
        <h1 class="font ml-10 mr-10 text-white">O que são CriptoMoedas?</h1>
        <h3 class="font ml-10 mr-10 mt-3" :class="smAndDown ? 'mb-5 mt-5' : ''">As criptomoedas são formas de moeda
          digital que utilizam criptografia para
          garantir a segurança das transações
          e controlar a criação de novas unidades.<p></p>Elas são descentralizadas, o que significa que não são
          controladas por
          um governo central ou instituição financeira, como um banco central. Em vez disso, as criptomoedas operam em uma
          rede de computadores distribuídos, muitas vezes chamada de blockchain.</h3>

        <div class="mt-5 d-flex justify-center align-center">
          <v-dialog width="500">
            <template v-slot:activator="{ props }">
              <v-btn color="black" width="200" class="mt-2" :class="smAndDown ? 'mb-5 mt-10' : ''"
                v-bind="props" text="CriptoMoedas"> </v-btn>
            </template>

            <template v-slot:default="{ isActive }">
              <v-card title="Principais CriptoMoedas">
                <v-card-text>
                  <span class="text-amber-darken-4"><v-avatar image="/bitcoin.png"></v-avatar> Bitcoin (BTC)</span>: O
                  Bitcoin continua sendo a criptomoeda mais
                  valiosa e amplamente reconhecida. É
                  frequentemente usado como reserva de valor e meio de troca.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/ethereum.png"></v-avatar> Ethereum (ETH)</span>: O
                  Ethereum é uma plataforma de contrato
                  inteligente que permite a criação de aplicativos
                  descentralizados (DApps). O Ethereum é a criptomoeda nativa da plataforma.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/binance.png"></v-avatar> Binance Coin (BNB)</span>: A
                  Binance Coin é a criptomoeda nativa da
                  exchange Binance e é usada para pagar taxas
                  na plataforma.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/tether.png"></v-avatar> Tether (USDT)</span>: O
                  Tether é uma criptomoeda estável (stablecoin)
                  projetada para manter um valor estável
                  atrelado ao dólar dos EUA. É frequentemente usado para fins de trading e como uma forma de evitar a
                  volatilidade.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/cardano.png"></v-avatar> Cardano (ADA)</span>:
                  Cardano é uma plataforma de contrato
                  inteligente que se concentra em segurança e
                  escalabilidade. ADA é a criptomoeda que alimenta a plataforma.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/solana.png"></v-avatar> Solana (SOL)</span>: Solana é
                  uma blockchain de alto desempenho que
                  visa melhorar a escalabilidade e a
                  velocidade das transações.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/xrp.png"></v-avatar> XRP (XRP)</span>: XRP é a
                  criptomoeda associada à Ripple, uma
                  plataforma que visa facilitar transações
                  transnacionais.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/polkadot.png"></v-avatar> Polkadot (DOT)</span>:
                  Polkadot é uma plataforma que conecta
                  diferentes blockchains para facilitar a
                  interoperabilidade.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/avax.png"></v-avatar> Avalanche (AVAX)</span>:
                  Avalanche é uma plataforma de contrato
                  inteligente que busca oferecer
                  interoperabilidade entre diferentes blockchains.
                  <br>
                  <br>
                  <span class="text-amber-darken-4"><v-avatar image="/doge.png"></v-avatar> Dogecoin (DOGE)</span>: O
                  Dogecoin começou como uma criptomoeda de
                  meme, mas ganhou popularidade como uma forma
                  de gorjeta e em transações menores.
                </v-card-text>
                <v-card-actions>
                  <v-spacer></v-spacer>
                  <v-btn class="bg-black" text="Fechar" @click="isActive.value = false"></v-btn>
                </v-card-actions>
              </v-card>
            </template>
          </v-dialog>
        </div>
      </div>
    </v-container>



    <div class="bg-yellow-accent-4">
      <v-img src="/criptomoedas.jpg" :class="smAndDown ? 'w-100 h-75' : 'w-0 h-0'" />
    </div>


    <v-container class="bg-yellow-accent-4 mt-5 d-flex justify-space-between elevation-24">

      <div>
        <h1 class="font ml-10 mr-10 text-white">Qual é o impacto ambiental?</h1>
        <h3 class="font ml-10 mr-10 mt-3" :class="smAndDown ? 'mb-5 mt-5' : ''">Muito se fala sobre a virtualidade dos
          ativos digitais. Como eles não existem no mundo físico, evitam o uso de metais e papel. Nesse ponto de vista,
          podem até ser considerados ecológicos, mas não é bem assim.
          As transações de criptos afetam o meio ambiente, e isso é uma preocupação não somente dos proprietários das
          moedas, mas também dos desenvolvedores das tecnologias e de estudiosos ambientais. Veja como as coins afetam o
          ambiente e o que fazer para reduzir esse impacto.</h3>

        <div>
          <v-img src="/impacto.png" width="650" :class="smAndDown ? 'w-100 h-75' : 'w-0 h-0'" />
        </div>
      </div>



      <div>
        <v-img src="/impacto.png" width="650" :class="smAndDown ? 'w-0 h-0' : ''" />
      </div>
    </v-container>

    <v-container class="bg-yellow-accent-4 elevation-24">
     
      <div class="mt-5 mb-5">
        <v-chip class="font bg-white pb-5 pt-5">EMISSÃO DE GASES</v-chip>
        <h3 class="font mt-3 ml-3 mr-10">O processo de fabricação de papel gera um impacto considerável no ambiente, em
          várias etapas. Primeiro, há a derrubada das árvores, que tiram de cena um excelente conversor de gás carbônico
          em oxigênio, por meio da fotossíntese. Ao irem para a fábrica, emitem mais gases no processo.
          As máquinas da linha de produção que transformam a madeira em papel e as substâncias químicas utilizadas na
          fábrica produzem mais gases e resíduos tóxicos. Assim, o resultado desse processo vai além do papel em si,
          englobando o rastro de poluentes e emissão de CO2 que deixa no caminho.
          Portanto, lidar com as finanças de forma digital (criptomoedas) não poupa o ambiente
          desse tipo de poluição. Ainda há outro fator poluente que não é facilmente percebido, e vamos mostrar o porquê.
        </h3>

        <br>

        <v-chip class="font bg-white pb-5 pt-5">MINERAR CRIPTOMOEDAS</v-chip>
        <h3 class="font mt-3 ml-3 mr-10">Um exemplo de impacto ambiental das criptomoedas é o Bitcoin, que usa o modelo de
          mineração Proof-of-Work (PoW). Ele funciona à base de recompensa pelo trabalho. Assim, para um novo bloco ser
          adicionado à rede, cálculos complexos são realizados pelos computadores que resolvem as equações no chain.
          Os computadores usam energia elétrica para funcionar. Assim, a mineração de criptomoedas no esquema PoW precisa
          de uma grande quantidade de eletricidade para existir. Isso consome recursos naturais e deixa um rastro de
          poluição.
          O impacto ambiental das criptomoedas vai além da produção de energia. Os computadores que fazem os cálculos no
          chain ainda usam recursos minerais, como silício, metais raros nos chips, plástico (que vem do petróleo), entre
          outros.
        </h3>

        <br>

        <v-chip class="font bg-white pb-5 pt-5">POLUIÇÃO INDIRETA</v-chip>
        <h3 class="font mt-3 ml-3 mr-10">A relação entre criptomoedas e meio ambiente mostra mais uma poluição indireta.
          Ela não mostra as árvores sendo derrubadas ou a fumaça que sai das chaminés das fábricas. A produção de energia,
          que no Brasil, majoritariamente, vem das hidrelétricas, é uma poluição pouco visível, mas não menos destrutiva.
          Para construir uma barragem de armazenamento de água para fazer a usina funcionar, muitos rios são desviados e
          áreas inteiras são inundadas, muitas vezes, florestas e cidades desaparecem completamente. Essa é uma enorme
          mudança no ambiente.
          Para construir as máquinas que processam os dados do blockchain, a extração e o processamento das
          matérias-primas até se transformarem no produto final são responsáveis pela emissão de carbono e outros
          resíduos, por meio da liberação de gás.
        </h3>

        <br>

        <v-chip class="font bg-white pb-5 pt-5">CUSTO DAS COINS</v-chip>
        <h3 class="font mt-3 ml-3 mr-10">Viver de minerar criptomoedas no esquema PoW está cada vez mais custoso. No caso
          do Bitcoin, os cálculos para encontrar novos blocos estão cada vez mais complexos, fazendo com que as máquinas
          precisem usar muita energia para criar uma nova moeda.
          Computadores tradicionais não têm a mesma agilidade para fazer esses cálculos, levam mais tempo e gastam mais
          energia. Assim, vale ver outros mecanismos de consenso, como o Proof of Stake (PoS), no qual os usuários validam
          os blocos, e o Proof of Authority (PoA), que valida novas moedas por meio da reputação.
        </h3>
      </div>
    </v-container>

    <v-container class="bg-yellow-accent-4 mt-5 elevation-24">

      <div>
        <h1 class="font ml-10 mr-10 text-white d-flex justify-center align-center">Possiveis soluções :</h1>
        <h3 class="font ml-10 mr-10 mt-5" :class="smAndDown ? 'mb-5 mt-5' : ''">
          1. <span class="text-white"> Migração para fontes de energia limpa :</span> Uma das maneiras mais eficazes de
          reduzir o impacto ambiental das
          criptomoedas é a mineração utilizando fontes de energia renovável, como energia solar, eólica e hidrelétrica. A
          migração para fontes limpas de energia reduzirá a pegada de carbono das operações de mineração.
        </h3>

        <h3 class="font ml-10 mr-10 mt-10" :class="smAndDown ? 'mb-5 mt-5' : ''">
          2. <span class="text-white"> Uso de hardware eficiente :</span> A escolha de hardware de mineração mais
          eficiente
          em termos de energia, como ASICs (Application-Specific Integrated Circuits), em vez de GPUs (Unidades de
          Processamento Gráfico), pode reduzir significativamente o consumo de eletricidade.
        </h3>


        <h3 class="font ml-10 mr-10 mt-10" :class="smAndDown ? 'mb-5 mt-5' : ''">
          3. <span class="text-white"> Consenso mais ecológico :</span> Alguns projetos de criptomoedas estão explorando
          alternativas mais sustentáveis ao algoritmo de prova de trabalho (PoW), como a prova de participação (PoS) e a
          prova de autoridade (PoA), que consomem consideravelmente menos energia.
        </h3>

        <h3 class="font ml-10 mr-10 mt-10" :class="smAndDown ? 'mb-5 mt-5' : ''">
          4. <span class="text-white"> Migração para redes de segunda camada :</span> Usar redes de segunda camada, como a
          Lightning Network para o Bitcoin, pode reduzir a carga de transações na cadeia principal, diminuindo a demanda
          de energia global da rede.
        </h3>

        <h3 class="font ml-10 mr-10 mt-10" :class="smAndDown ? 'mb-5 mt-5' : ''">
          5. <span class="text-white"> Educação e conscientização : </span> É importante educar os mineradores e
          entusiastas de criptomoedas sobre a importância de minimizar o impacto ambiental e incentivar boas práticas
          ambientais.
        </h3>

        <h3 class="font ml-10 mr-10 mt-10" :class="smAndDown ? 'mb-5 mt-5' : ''">
          6. <span class="text-white"> Regulamentação ambiental : </span> Os governos podem estabelecer regulamentações
          que exijam que as operações de mineração de criptomoedas atendam a padrões ambientais específicos, incentivando
          a transição para fontes de energia mais limpas e práticas mais sustentáveis.
        </h3>

        <h3 class="font ml-10 mr-10 mt-10" :class="smAndDown ? 'mb-5 mt-5' : ''">
          7. <span class="text-white"> Descentralização da mineração : </span> A concentração da mineração em áreas com
          eletricidade barata frequentemente leva a um uso excessivo de energia. Promover a descentralização da mineração,
          incentivando a criação de operações de mineração em locais com acesso a fontes de energia limpa e abundante,
          pode contribuir para a redução do impacto ambiental.
        </h3>
      </div>
      
      <v-img src="/impacto.jpg" class="mt-10"/>
    </v-container>


    <v-main>
      <HelloWorld />
    </v-main>  
  </v-app>
</template>


<style scoped>
.font {
  font-family: 'Jost', sans-serif;
}
</style>



<script setup>
import HelloWorld from '@/components/HelloWorld.vue'
import { useDisplay } from 'vuetify';

const { smAndDown } = useDisplay()

</script>
