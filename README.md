# Tributaçoes-por-NCM
Eusou contador, mas sou entusiasta de programação, em especial em temas relacionados com Data Science. Inclusive, minha opinião pessoal é que contabilidade e ciência de dados tem tudo a ver (mais sobre isso no futuro). Hoje, a ideia é abordar um tema mais “clássico” da contabilidade, a saber, a questão tributária. Para simplificar muito, com o perdão de qualquer estudioso da incrível complexidade do nosso sistema de impostos, as alíquotas que incidem sobre qualquer mercadoria ou produto no Brasil podem ser resumidas em um único parâmetro: a NCM. Aí, você, querido leitor pode estar se perguntando “que diabos é um NCM? Onde vivem: O que comem?”. Pois bem, NCM é a sigla para Nomenclatura Comum do Mercosul, que é basicamente um tabelão para padronizar a nomenclatura de produtos. Assim, você pode utilizar um 9609.10.00 para desenhar em seu 4820.20.00. Tudo o que circula no país está devidamente codificado pela NCM, você pode conferir na nota fiscal, logo depois da descrição do produto. Voltando aos tributos, os fiscos federal e estaduais, em suas legislações, utilizam a classificação da NCM para a a indicação dos tributos. Então, para saber a alíquota de IPI, Pis, Cofins, Icms ou Icms-ST, ou mesmo se existem condições especiais como redução de base de calculo ou isenções, você procura as NCMs nos diversos regulamentos de impostos. Parametrizar as configurações tributárias em sistemas integrados de gestão é basicamente vincular as alíquotas a uma NCM, uma UF de Origem e uma UF de Destino (e meu amigo, isso dá trabalho…). Então, nesse hobby de brincar com dados, pensei em qual seria a dificuldade de constituir essa base de dados, em relacionar todos as alíquotas, isenções e benefícios fiscais em uma única base de dados, usando a NCM como chave. Para não pegar pesado logo de cara, escolhi o IPI, que é tributo federal então eu só precisaria começar com uma fonte de dados: A Receita Federal (para o ICMS teríamos que raspar pelo menos 27 fontes diferentes). Eu esperava encontrar um arquivo CSV mas… o que tinha era PDF. Ocorre que PDF é uma formato pensado para a visualização estática de documentos, e não para a distribuição de dados. Já tentou fazer PROCV ou um CORRESP num arquivo PDF? Pois é… não dá… Como nessa quarentena de COVID-19 a gente tá com tédio e tempo de sobra, resolvi abrir uma série qui no Medium para documentar essa jornada de tentar criar um repositório em que se consiga todos os parâmetros tributários de um tributo simplesmente indicando o NCM. E também é um jeito de eu estudar Python. Por enquanto é isso. Valeu!
