# aquidapet-showcase

## Sumário

- [aquidapet-showcase](#aquidapet-showcase)
  - [Sumário](#sumário)
  - [Motivação](#motivação)
  - [Pilha de tecnologia](#pilha-de-tecnologia)
    - [API](#api)
    - [Aplicativo](#aplicativo)

## Motivação

Após a última atividade individual de Programação para Dispositivos Móveis II que consistiu em criar um aplicativo com a biblioteca de interface de usuário sorteada pelo professor, o professor decidiu que a próxima atividade será criar um projeto com arquitetura REST valendo pelas duas notas do segundo bimestre. O projeto deve contemplar no mínimo um dos dezessete Objetivos de Desenvolvimento Sustentável da Organização das Nações Unidas. Apesar de a unidade curricular ser Programação para Dispositivos Móveis II, esse projeto multidisciplinar requer conhecimentos construídos ao longo da formação do acadêmico, como a documentação da especificação de requisitos de software; a diagramação do Diagrama Entidade Relacionamento e respectivo Modelo Entidade Relacionamento; a persistência de dados através de uma tecnologia de mapeamento objeto-relacional ou correlata; o desenvolvimento da API; a configuração do mecanismo de compartilhamento de recursos com origens diferentes; a hospedagem da API e do banco de dados remoto; o desenvolvimento do aplicativo em si utilizando React Native _etc_.

Como destacado pelo professor, o principal intuito de um projeto deste porte é enriquecer o currículo do discente e fazê-lo adquirir experiência com as estratégias de implementação adotadas, bem como com as adversidades na trajetória do desenvolvimento de software. A turma foi convidada a se dividir em grupos de um a três discentes, logo, eu optei pela entrega individual desta atividade. Conforme o cronograma abaixo, a definição dos grupos ocorreu do dia dezessete ao dia vinte e quatro de outubro. Do dia vinte e quatro em diante, o projeto foi desenvolvido em etapas organizadas pelo próprio grupo.

| Data | Descrição da atividade |
|---|---|
| 17/10/2023 | Lançamento do projeto |
| 24/10/2023 | Definição dos grupos e entrega dos temas escolhidos para o desenvolvimento do projeto |
| 31/10/2023 | Entrega do projeto de engenharia de software do aplicativo |
| 07/11/2023 | Entrega dos mockups do aplicativo |
| 14/11/2023 | Desenvolvimento da aplicação |
| 21/11/2023 | Desenvolvimento da aplicação |
| 28/11/2023 | Desenvolvimento da aplicação |
| 05/12/2023 | Entrega do projeto final |

Em conclusão, o tema do meu projeto é o **desenvolvimento de um aplicativo para localização de pets desaparecidos**. Estes são trechos da justificativa contendo um breve estudo de viabilidade do projeto:

> Por motivos diversos, alguns tutores enfrentam o problema do desaparecimento de seu pet. Para alertar seus contatos e contar com a colaboração deles, tais tutores costumam procurar por fotos do pet desaparecido e montar uma imagem, geralmente com orientação retrato, contendo fotos que facilitem sua identificação; além de textos verbais como número de telefone de contato, último local em que foi visto, valor da recompensa por achá-lo etc. Nesse sentido, o compartilhamento de fotos de pets desaparecidos é uma prática comum e eficaz para aumentar as chances de encontrar um pet desaparecido. Entretanto, essa prática também apresenta alguns problemas que podem dificultar a localização do pet.
>
> Um dos principais problemas é a falta de atenção dos usuários das redes sociais. Na correria do dia a dia, é comum que as pessoas não tenham tempo ou disposição para ler todos os status e stories que aparecem em suas timelines. Com isso, é possível que uma foto de um pet desaparecido passe despercebida por muitas pessoas.
>
> Outro problema é a falta de colaboração de quem vê o pet desaparecido. Mesmo que alguém veja um pet que se encaixe na descrição de um alerta de desaparecimento, nem sempre essa pessoa se dá ao trabalho de ajudar. Isso pode acontecer por diversos motivos, como a falta de interesse, a desconfiança ou a falta de tempo.
>
> Um dos motivos para a falta de colaboração é a burocracia envolvida. Para ajudar, a pessoa precisa abrir o app da Câmera para tirar foto do pet, depois salvar o contato do tutor visitando a foto do pet desaparecido, a qual ele também deve localizar em seu dispositivo móvel; para só então abrir o WhatsApp (assumindo que ambos usem WhatsApp) e mandar sua localização após ativá-la nas permissões do aplicativo.
>
> Além desses problemas, existem outros relacionados ao compartilhamento de fotos de pets desaparecidos. Por exemplo, é importante que as fotos sejam de boa qualidade e que o pet seja identificado de forma clara. Também é importante que as informações fornecidas no alerta sejam precisas e atualizadas.

Na data final, cinco de dezembro, foi entregue um Produto Mínimo Viável, um aplicativo com cadastro de usuários e verificação de número de telefone via SMS e cadastro de pets desaparecidos com armazenamento de imagem via Firebase Storage. Atualmente (01/01/24), o aplicativo se encontra $\frac{7}{26}$ concluído. Devido a alguns _issues_[<sup>1</sup>](#nota-de-rodape-1) relacionados à incompatibilidade da ferramenta de mapeamento objeto-relacional TypeORM e o banco de dados MongoDB, a API carece de refatoração na camada de objeto de acesso a dados; entretanto, seu andaime está completo e já foram documentadas todas as rotas necessárias.

Vale destacar que o acesso à documentação e ao código-fonte do projeto é restrito, o que justifica a existência deste repositório.

Os repositórios de código apresentados no Curso Superior de TSI do IFMS como requisito para obtenção da nota parcial das atividades da unidade curricular Programação para Dispositivos Móveis II estão privados. Entretanto, este é o _quarto_ repositório de código _público_ da unidade curricular cujo intuito é manter a lista de repositórios de código ordenada.

<sup id="nota-de-rodape-1">1</sup> Alguns exemplos: [typeorm/typeorm#3964](https://github.com/typeorm/typeorm/issues/3964); [typeorm/typeorm#9037](https://github.com/typeorm/typeorm/issues/9037); [nestjsx/crud#152](https://github.com/nestjsx/crud/issues/152).

| [&larr; Repositório anterior](https://github.com/mdccg/reddit-clone) |
|-|

## Pilha de tecnologia

### API

| Papel | Tecnologia |
|-|-|
| Framework | [Express](https://expressjs.com/pt-br/) |
| Armazenamento de imagens | [Firebase](https://firebase.google.com/?hl=pt) |
| Mensageria | [Twilio](https://www.twilio.com/) |
| Hospedagem do banco de dados | [MongoDB Atlas](https://www.mongodb.com/atlas/database) |
| Mapeamento objeto-relacional | [TypeORM](https://typeorm.io/) |
| Ferramenta de TDD | [Postman](https://www.postman.com/) |

### Aplicativo

| Papel | Tecnologia |
|-|-|
| [Prototipagem](https://figma.fun/MEb06b) | [Figma](https://figma.com/) |
| Biblioteca de desenvolvimento | [React Native](https://reactnative.dev/) |
| Bundler | [Expo](https://expo.dev/) |

Os créditos pelas mídias utilizadas estão disponíveis nos repositórios privados do projeto. 