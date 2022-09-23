# Bootcamp Database Experience - 5º Desafio de Projeto
 ---
Há apenas alguns dias o título de um artigo publicado nos fóruns da Digital Innovation One me chamou à atenção. Dizia: "Os dados por si só não valem de muita coisa". Não sei se o título era um *clickbait*, mas foi efetivo em atrair a minha atenção. Após proceder à leitura do artigo e processar as razões de tal afirmação, conclui que "concordo discordando". E este desafio me ajudará a explicar o porquê.

O desafio propõe demonstrar a compreensão do "papel dos Bancos de Dados Relacionais (SQL) e Não Relacionais (NoSQL) no contexto de um Engenheiro de Dados". Assim, pretendo começar discorrendo sobre os dados em geral e porque eu discordo da proposição que inicia nossa discussão.

Em meados das décadas de 1960 e 1970, sociólogos de renome como Alain Touraine e Daniel Bell, cunharam uma expressão que buscava definir a sociedade pós-industrial, que eles chamariam de **sociedade da informação**. A expressão ganha força na década de 1990, com os trabalhos do sociólogo espanhol Manuel Castells.  A expressão é bastante abrangente e carregada de significados, principalmente no que se refere aos estudos das ciências sociais. Mas ela também enceja o surgimento de expressões correlatas, como **era da informação** e **era dos dados** (vide documentário da Netflix). Todas essas expressões apontam para dois fatores importantes sobre a nossa história recente:

1. Nossa sociedade vive um *momentum* de desenvolvimento tecnológico sem precedentes e isso tem alterado nossa maneira de viver e de nos relacionarmos uns com os outros;
2. Vivemos em rede, em teias cada vez maiores e mais globalizadas. O que, em parte, decorre do primeiro fator.

Em outras palavras, nossa sociedade é permeada pela tecnologia, com ênfase nas tecnologias de informação e comunicação (TIC) e ela se configura em (cada vez mais) em rede(s). Para se ter uma ideia, quase 80% da população brasileira está nas redes sociais, isso equivale a mais 170 milhões de brasileiros, o dobro de 8 anos atrás (86 milhões em 2014). Além das redes sociais utlizamos serviços de *streaming*, *marketplace*, *delivery*, finanças, saúde, e uma infinidade de outras coisas à distância de um clique na tela do celular. Tudo isso gera uma infinidade de dados diariamente. Um levantamento realizado em 2012 detectou que a cada 24 horas cerca de 500TB (*terabytes*) eram gerados pelo Facebook. Isso nos leva a um terceiro e um quarto fator:

3. Vivemos a **era dos dados**, tudo são dados, nossa vida transformada em dados diariamente;
4. Preceitua o *The Economist*, **"o recurso mais valioso do mundo não é mais o petróleo, são os dados"**.

Os dados são, antes de qualquer tratamento, muito valiosos. Os grandes *players* do mercado hoje em dia entendem a importância imanente desses ativos. A analogia do petróleo é muito boa para explicar esse ponto de vista. O petróleo bruto, da forma que é extraída da crostra terrestre não estará ainda em condições abastecer a sua BMW, contudo seu valor é devidamente reconhecido. Vejo o mesmo acontecer com os dados, é fácil saber o valor dos dados (brutos) para um empresa quando há uma invasão a seus sistemas, ou quando uma falha faz perder temporária ou permanentemente esses ativos.

Mas, roubo da física quântica uma de suas características e proponho uma sobreposição de estados ao também concordar com a frase. E talvez aqui o objetivo do desafio esteja mais presente. Pois os **dados são a forma bruta, a matéria prima** a atividade dos hipotéticos artesãos, os muitos profissionais que trabalham com tratamento de dados, entre eles o engenheiro de dados. Na maioria esmagadora das atividades que envolvem dados, o seu valor só será percebido a partir do seu tratamento. E aqui desponta a importância do engenheiro de dados, "o responsável pela criação do *pipeline* que transforma os dados brutos que estão nos mais variados formatos, desde bancos de dados transacionais até arquivos de texto, em um formato que permita ao Cientista de Dados começar seu trabalho". **Análises consistentes de dados só poderão ser produzidas se uma engenharia consistente for aplicada**.

Nessa atividade algumas tecnologias apresentam casos de sucesso no mercado. Tecnologias que, de certa forma, fazem do dia a dia dos profissionais dos dados. Discorreremos agora um pouco sobre algumas dessas tecnologias.

---
### O modelo relacional - SQL
---
Malgrado não tenha sido o primeiro modelo para o gerenciamento de banco de dados, o modelo relacional, criado no início dos anos 1970, se estabelece em finais da década seguinte. Sua adoção é tão capilarizada que por muito tempo, em inúmeros contextos o modelo relacional se tornou sinônimo banco de dados. Durante décadas falar de banco de dados era falar no modelo relacional. Muito desse sucesso se dá, até a atualidade, pelo conjunto de propriedades (ACID) de transação característicos dos bancos relacionais, que preceitua que cada transação em um banco de dados relacional dele ter Atomicidade (A), Consistência (C), Isolamento (I) e Durabilidade (D). Os bancos relacionais são também conhecidos por ter uma estrutura rígida, disposta em tabelas ligadas por relacionamentos.

---
### O modelo não relacional ou não só relacional - NoSQL
---
Preceitua-se que o termo *NoSQL* possivelmente teria sido usado a peimeira vez Carlo Strozzi para designar um projeto de sistema de banco de dados *open source* de sua autoria em 1998. O termo "não pegou", nem as tecnologias relacionadas, até junho de 2009, quando "um encontro promovido por Johan Oskarsson e Eric Evans, que teve como objetivo discutir o crescente surgimento de soluções *open source* de armazenamento de dados distribuídos não relacionais". O movimento crescente de adoção de tecnologias, entre elas sistemas de gerenciamento de bancos de dados não relacionais, dispunha dessa vez de uma característica interessante: não é objetivo dessas alternativas substituir por completo o modelo relacional. Por isso sustenta-se que *NoSQL* não seria pura e simplesmente a negação do *SQL*, mas seu siginificado seria *Not Only SQL* (não somente SQL).

A prática atual tem demonstrado que, de fato tecnologias relacionais e não relacionais compartilham projetos de desenvolvimento e análise. Vale salientar que o termo *NoSQL* não se refere a uma única tecnologia, nem se aplica a uma única estrutura de dados, pelo contrário, é um termo guarda chuva que informa muito mais o que não é, do que aquilo que de fato é. "A ideia principal é abrir mão da consistência em favor da disponibilidade e escalabilidade". As principais categorias de orientação de bancos não relacionais são:
1. Docmunetos;
2. Chave-valor;
3. Colunas;
4. Grafos.

Na tentativa de elencar as propriedades dos sistemas não relacionais, Dan Pritchett cunhou o termo BASE (Basically Available, Soft-state, Eventual consistency), "que de forma elegante conseguiu jogar com as palavras e montar uma sigla para contrapor o termo ACID, gerando uma comparação entre Ácido vs. Básico", como nos componentes químicos. ""

---
### O equilíbrio ACID vs BASE
---
Na química, ácidos e bases se estabilizam quando em contato um com o outro. O *NoSQL* não existe para substituir o *SQL*, mas para complementá-lo. Otimizar as possiblidades em contextos onde a utilização do relacional mas atrapalha do que ajuda. O contrário também é verdadeiro. E o profissional que busca se envolver nessa seara, engenheiro de dados ou não, precisa reconhecer tal fato e saber decidir na hora certa para o projeto certo qual tecnologia (das tantas existentes) melhor se aplica.

---
### Referências  e citações (não indexadas e nem um pouco organizadas)
http://www4.fe.uc.pt/fontes/trabalhos/2008007.pdf

https://canaltech.com.br/redes-sociais/Facebook-gera-mais-500TB-de-dados-diariamente/#:~:text=Voc%C3%AA%20j%C3%A1%20imaginou%20qual%20%C3%A9,dados%20a%20cada%2024%20horas

https://medium.com/somos-tera/o-recurso-mais-valioso-do-mundo-nao-e-mais-o-petroleo-sao-os-dados-d0ad3cf72496

https://resultadosdigitais.com.br/marketing/estatisticas-redes-sociais/#:~:text=Estat%C3%ADsticas%20gerais%20de%20Redes%20Sociais,usu%C3%A1rios%20de%202021%20para%202022

https://blog.dsacademy.com.br/o-que-faz-um-engenheiro-de-dados/

https://pt.wikipedia.org/wiki/ACID

https://www.devmedia.com.br/o-que-e-nosql-java-magazine-86/18777#:~:text=O%20movimento%20noSQL%20teve%20sua,de%20dados%20distribu%C3%ADdos%20n%C3%A3o%20relacionais

https://db-engines.com/en/ranking

