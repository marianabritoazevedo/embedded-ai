## :pencil: Article *"TinyMLOps: Operational Challenges for Widespread Edge AI Adoption"*

This activity aims to summarize the article *"TinyMLOps: Operational Challenges for Widespread Edge AI Adoption"*, written by Sam Leroux et al. The full article can be accessed [here](https://arxiv.org/pdf/2203.10923.pdf).

## ![brasil](https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Flag_of_Brazil.svg/22px-Flag_of_Brazil.svg.png) Resumo completo

<p align="justify">Com o crescimento da Inteligência Artificial nos últimos anos, surgiu-se um novo conceito que pode ser considerado uma nova fronteira nesse ramo, a edge AI, traduzida como Inteligência Artificial de Borda. Esse conceito se refere ao processamento de algoritmos de Inteligência Artificial não mais na nuvem, e sim nos próprios dispositivos que são utilizados pelos usuários. Isso significa que todos os dados são armazenados, processados e analisados diretamente nesses dispositivos.</p>
<p align="justify">Essa abordagem traz diversas vantagens para o usuário, como por exemplo, uma menor latência, maior robustez, maior facilidade para integração com dispositivos e até uma maior segurança e privacidade dos dados, já que eles ficarão armazenados apenas no próprio dispositivo do usuário. Entretanto, existem ainda vários obstáculos para a implementação de edge AI em larga escala, e no contexto de TinyML, muitas vezes não está relacionado apenas com os recursos computacionais disponíveis, como também do processamento limitado nesses dispositivos e várias questões operacionais. </p>
<p align="justify">Assim, o artigo TinyMLOps: Operational Challenges for Widespread Edge AI Adoption visa justamente entender essas dificuldades de implementar Machine Learning (ML) em dispositivos de borda e procura trazer sugestões de melhorias que poderiam ser implementadas no contexto de TinyMLOps. </p>
<p align="justify">Primeiramente, deve-se entender que o MLOps é uma extensão do DevOps que busca trazer práticas de automação, monitoramento, integração e testes para aplicativos ML. Logo, o TinyMLOps teria o mesmo objetivo, mas voltado para aplicações utilizando TinyML, e com isso surgem diversos desafios de sair de um aplicativo ML totalmente centralizado na nuvem para um aplicativo descentralizado implementado em borda. Entre os principais desafios, pode-se citar o gerenciamento de diversas versões de um modelo, a observabilidade, os modelos de negócio de pagamento por consulta e o treino e personalização dos modelos. </p>
<p align="justify">Sobre o primeiro desafio, diferentes dispositivos possuem diferentes características, o que faz necessário o uso de múltiplos modelos para que eles sejam suportados pelas diversas plataformas e aparelhos, sendo um grande obstáculo gerenciar todos os diferentes modelos existentes. Em relação à observabilidade, é importante sempre estar havendo a detecção de desvio de dados para que o modelo continue funcionando como o esperado.</p>
<p align="justify">Ademais, no que diz respeito ao modelo de negócios, é imprescindível analisar que há todo um custo de conhecimento e de tempo para desenvolver e treinar os modelos, e que é importante pensar em uma maneira do usuário pagar por esse serviço. Pode-se pensar em algumas opções como pagamentos por consulta ou pacotes pré-pagos, entretanto, fazer isso de forma offline (que é possível com o paradigma da computação em borda) e de forma segura ainda é um desafio. </p>
<p align="justify">Por fim, ainda existe a questão de retreinar e personalizar os modelos, que é mais fácil de gerenciar quando tudo está organizado de forma centralizada na nuvem. Uma solução que já vem sendo implementada nesse sentido é o Federated Learning, por exemplo.</p>
<p align="justify">Outro ponto muito importante ainda em relação aos desafios da implementação de ML em borda é a questão da propriedade intelectual do modelo. Há pessoas que tentam roubar, direta ou indiretamente modelos ML, e essa questão de segurança precisa ser bem avaliada. Já existem algumas técnicas que tentam proteger o modelo, como técnicas de criptografia, uso de ambientes de processamento seguro ou até a detecção de padrões em consultas roubadas, e também técnicas que não protegem diretamente o modelo, mas são úteis para comprovar fraude, que seria a utilização de marcas d’água, por exemplo.</p>
<p align="justify">Em suma, percebe-se que são diversas as dificuldades que ainda precisam ser enfrentadas na implementação de ML em borda, porém, já existem diversas sugestões de soluções que podem ser implementadas em um contexto de TinyMLOps.</p>

# ![eua](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/Flag_of_the_United_States.svg/22px-Flag_of_the_United_States.svg.png) Full summary
<p With the growth of Artificial Intelligence in recent years, a new concept emerged that can be considered a new frontier in this field, edge AI. This concept refers to the processing of Artificial Intelligence algorithms no longer in the cloud, but in the very devices that are used by users. This means that all data is stored, processed and analyzed directly on these devices.
</p>

<p align="justify">This approach brings several advantages to the user, such as lower latency, greater robustness, easier integration with devices and even greater data security and privacy, since they will only be stored on the user's own device. However, there are still several obstacles to the implementation of edge AI on a large scale, and in the context of TinyML, it is often not only related to the available computing resources, but also the limited processing on these devices and many operational issues.
</p>

<p align="justify">Thus, the article TinyMLOps: Operational Challenges for Widespread Edge AI Adoption aims precisely to understand these difficulties of implementing Machine Learning (ML) in edge devices and seeks to bring suggestions for improvements that could be implemented in the context of TinyMLOps.
</p>

<p align="justify">First, it should be understood that MLOps is an extension of DevOps that seeks to bring automation, monitoring, integration and testing practices to ML applications. Therefore, TinyMLOps would have the same objective, but focused on applications using TinyML, and with that, there are several challenges to go from a fully cloud-centric ML application to a decentralized application implemented at the edge. Among the main challenges, we can mention managing several versions of a model, observability, pay-per-query business models, and training and customizing the models.
</p>

<p align="justify">About the first challenge, different devices have different characteristics, which makes it necessary to use multiple models so that they are supported by different platforms and devices, being a major obstacle to manage all the different existing models. Regarding observability, it is important to always be detecting data deviation so that the model continues to work as expected.
</p>

<p align="justify">Furthermore, with regard to the business model, it is essential to analyze that there is a whole cost of knowledge and time to develop and train the models, and that it is important to think of a way for the user to pay for this service. It's possible to think of some options such as pay-per-view or prepaid packages, however, doing this offline (which is possible with the edge computing paradigm) and securely is still a challenge.
</p>

<p align="justify">Finally, there is still the issue of retraining and customizing the models, which is easier to manage when everything is centrally organized in the cloud. A solution that has already been implemented in this sense is Federated Learning, for example.
</p>

<p align="justify">Another very important point regarding the challenges of implementing ML at the edge is the issue of the intellectual property of the model. There are people who try to steal, directly or indirectly, ML models, and this security issue needs to be well evaluated. There are already some techniques that try to protect the model, such as encryption techniques, use of secure processing environments or even the detection of patterns in stolen queries, and also techniques that do not directly protect the model, but are useful to prove fraud, which would be the use of watermarks, for example.
</p>

<p align="justify">In short, it is clear that there are several difficulties that still need to be faced in the implementation of ML at the edge, however, there are already several suggestions for solutions that can be implemented in a context of TinyMLOps.
</p>
