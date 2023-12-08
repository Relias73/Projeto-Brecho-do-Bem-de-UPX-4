# Projeto Brecho-do-Bem: desenvolvido durante o Curso de UPx-4 - 4* Semestre ADS - FACENS - 2023

1. Proposta e propósitos do projeto:

A proposta deste projeto experimental é desenvolver um website voltado para a captação de doações de roupas e calçados, com o objetivo de promover o desenvolvimento sustentável das cidades e apoiar entidades filantrópicas que atuam na distribuição desses itens para pessoas em situação de vulnerabilidade. O projeto tem como propósito central a promoção do Objetivo de Desenvolvimento Sustentável (ODS) número 11 da ONU, que visa tornar as cidades e comunidades mais inclusivas, seguras, resilientes e sustentáveis.

2. Objetivos:

Os objetivos deste projeto são:
a. Criar um website funcional e intuitivo que permita aos doadores cadastrarem suas doações de roupas e calçados de forma fácil e rápida.
b. Facilitar o cadastro de entidades filantrópicas interessadas em receber as doações, garantindo que elas atendam a critérios de transparência e eficiência na distribuição.
c. Promover a conscientização sobre a importância da doação de roupas e calçados como uma prática sustentável e solidária.
d. Estabelecer parcerias com empresas e organizações locais para incentivar a participação ativa na doação de roupas e calçados.
e. Medir o impacto das doações na melhoria das condições de vida das comunidades atendidas pelas entidades filantrópicas cadastradas na plataforma.

3. Revisão de literatura e estado da arte:

A literatura e o estado da arte relacionados a projetos similares destacam a importância da economia circular e da redução do desperdício têxtil como parte integrante do desenvolvimento sustentável. Além disso, estudos indicam que a doação de roupas e calçados usados pode contribuir significativamente para a redução da pegada ambiental da moda, evitando a produção de novos produtos e o descarte inadequado.
Existem várias plataformas e organizações em todo o mundo que já estão trabalhando para conectar doadores a entidades filantrópicas, aproveitando a tecnologia digital para facilitar esse processo. Essas iniciativas demonstram que a captação de doações online pode ser uma ferramenta eficaz para alcançar os objetivos de desenvolvimento sustentável.
Uma referência de sucesso em arrecadação de doações é o Exército da Salvação (The Salvation Army), fundado em 1865, atua no Brasil desde 1922 com unidades de atendimento a crianças em situação de risco, projetos educacionais, programas de capacitação profissional, lares para idosos, entre outros. Foi indicado mais de 20 vezes ao Prêmio Nobel da Paz, e é uma das mais respeitadas instituições de caridade do mundo. Através do seu site: Exército de Salvação - Doações - Doe roupas, móveis, brinquedos, eletrodomésticos, computadores e outros. (exercitodoacoes.org.br) – pode-se ter acesso às informações de campanhas, doações, pontos de coletas, bazares e outras da instituição.

4. Justificativa:

A justificativa para a realização deste projeto reside na necessidade de abordar questões sociais e ambientais de forma integrada e eficaz. Doar roupas e calçados usados não apenas ajuda as pessoas em situação de vulnerabilidade, mas também contribui para a redução do desperdício têxtil e a minimização do impacto ambiental da indústria da moda. Além disso, ao promover a gestão de cidades sustentáveis, o projeto se alinha diretamente com o ODS 11 da ONU, que busca tornar as cidades mais inclusivas, seguras e sustentáveis para todos os seus habitantes.
Este projeto também se justifica pela crescente importância da tecnologia digital como facilitadora de ações solidárias e sustentáveis. A criação de uma plataforma online para a captação de doações de roupas e calçados permite alcançar um público mais amplo e engajar empresas, organizações e indivíduos na causa da sustentabilidade urbana e da ajuda humanitária. Portanto, o projeto se apresenta como uma oportunidade relevante para contribuir com o desenvolvimento sustentável das cidades e o bem-estar de seus habitantes.

5. Código BACK END

A criação do código back end da aplicação foi conduzida com a utilização do Spring Initializr. Esse framework é amplamente reconhecido por sua capacidade de fornecer uma base sólida para o desenvolvimento de aplicações web seguras e escaláveis. A escolha do Spring Framework foi respaldada pela sua robustez e pela ampla comunidade de desenvolvedores que o suporta.
O framework Spring, disponível em https://start.spring.io/, é um frame de código aberto para o desenvolvimento de aplicativos Java.
A arquitetura aplicada é do modelo padrão MVC (Model – View – Controller), a fim de buscar a qualidade do código, reduzir erros e aumentar a eficiência do desenvolvimento. Resumidamente, após um chamado externo, as APIs interagem com o Controlador, que por sua vez interage com o Serviço. O serviço chama o Repositório que interage com o Banco de Dados. 
Esta arquitetura padrão tornar a base de código sustentável, escalável e de manutenção acessível a longo prazo. 

DIAGRAMA DA ARQUITETURA DO REST APIS: 

![image](https://github.com/Relias73/Brecho-do-Bem/assets/105240567/22082bb6-59e7-42a2-81c3-a4259b710dd5)


6. Interface com o Banco de Dados
A interface entre o código back end e o banco de dados é uma parte crítica da aplicação. Garantiu-se que essa conexão seja confiável e segura, permitindo que a aplicação acesse e gerencie informações de forma eficaz. Essa é uma garantia da integridade e do desempenho da aplicação.

6.1. Modelo / Entidade
Modelo é a entidade básica que tem uma relação direta com a estrutura de uma tabela no banco de dados. Em outras palavras, esses modelos servem como contêineres que contêm dados semelhantes e relativos que são usados para transportar esses dados de clientes para o banco de dados. Perfil de Usuário (Doador ou Instituição Receptora), Itens doados, Doações e Categorias são alguns dos modelos deste aplicativo.

6.2. Repositório
O repositório é uma interface que atua como uma ponte entre o banco de dados e o aplicativo. Ele carrega os dados do modelo para o banco de dados. Cada modelo terá um repositório exclusivo para o transporte de dados.

6.3.	Serviço
Serviço é a parte da arquitetura em que o repositório é instanciado e a lógica de negócios é aplicada. Os dados do cliente que chegam aqui são manipulados e enviados através do repositório para o banco de dados.

6.4.	Controlador
O controlador é a parte da arquitetura onde as solicitações dos clientes são tratadas pela primeira vez. Controla os processos que devem ser executados no back end e a resposta que deve ser entregue aos clientes. Ele interage com o serviço que, por sua vez, interage com o repositório que, por sua vez, interage com o banco de dados usando modelos.

Como se movem os dados em sua jornada entre o cliente e o BD:

![image](https://github.com/Relias73/Brecho-do-Bem/assets/105240567/11a9822d-352b-4f7b-8d51-6e98823e416a)








