Title: Usando Pelican como gerador de sites
Date: 2017-04-16 22:00
Category: Geral
Tags: Pelican, Site, Markdown, HTML, GitHub, Git, Hospedagem
Slug: Usando-pelican
Authors: José Antônio
Summary: Pequena explicação da forma de instalação e uso do Pelican para gerenciamento de um site.

## Usando Pelican

Nos últimos dias tive a oportunidade de conhecer melhor o [Pelican][Pel] e suas funcionalidades, não sou programador e nem tenho qualquer experiência na área, no entanto não tive dificuldades em começar a utiliza-lo.
[Pel]: https://blog.getpelican.com/  
O [Pelican][Pel] é um gerador de sites estáticos escrito em Python que pode ser utilizado em qualquer sistema operacional. Em meu caso estou utilizando o Pelican em uma máquina virtual com Debian 8 na distribuição [Qubes][QB].  
Mas se não sei HTML como irei escrever o conteúdo do site? Basta você escrever as páginas utilizando [Markdown][Mark], [reStructuredText][res] ou [AsciiDoc][Ascii]. Em meu caso estou escrevendo este texto em Markdown, caso queira ver este texto escrito antes da conversão para HTML clique [aqui][md].
[md]: http://www.becodoteimoso.com/pelican-ssg.md
[Mark]: http://daringfireball.net/projects/markdown/
[res]: http://docutils.sourceforge.net/rst.html
[Ascii]: http://www.methods.co.nz/asciidoc/
[QB]: https://www.qubes-os.org/  
As instruções para a instalação do [Pelican][Pel] podem ser acessadas clicando neste [link][link]. O procedimento de instalação é bem fácil, basta apenas utilizar o comando:  
[link]: http://docs.getpelican.com/en/stable/install.html

> pip install pelican  

Obs: Estou considerando que seu sistema já possua instalado o [Python][Python] e o [PyPi][PyPi]. =)  
[Python]: https://www.python.org/
[PyPi]: https://pypi.python.org/pypi  
Após a instalação do [Pelican][Pel] vamos ao trabalho, ou seja, vamos configura-lo. Este é o procedimento inicial para que o site possa ser construído, para isso no terminal crie uma pasta para armazenar os arquivos do site:  
> mkdir ~/Documentos/site  

Agora vamos acessar a pasta e configurar o Pelican.  

> cd ~/Documentos/site  
> pelican-quickstart  

Basta apenas responder as perguntas que serão feitas e pronto, já temos a estrutura do site montada agora basta inciar a escrita dos artigos e páginas de seu site.  
Para que seja gerado as páginas em HTML basta que o conteúdo seja salvo na pasta *content*. Após a escrita do material, retorne para a pasta raiz do site, neste exemplo a pasta _site_, e para gerar as páginas basta utilizar o comando:  
> pelican content  

Os arquivos contidos na pasta *content* serão convertidos e salvos na pasta *output*. Agora basta fazer o upload dos arquivos da pasta *output* no servidor que você irá utilizar e pronto, seu site estará on-line.  

### Minha experiência  
Após o pequeno tutorial acima gostaria de descrever um pouco de minha experiência com relação ao uso do [Pelican][Pel].  
Tive algumas dificuldades para a configuração de alguns plugins e também para a configuração do sistema de comentários [Disqus][Dis] porem não foi nada que não houve-se um vasta quantidade de informações na internet que me auxiliaram na resolução destes problemas.
[Dis]: https://disqus.com/  
Para reduzir ao máximo o custo de manutenção deste site escolhi como local para hospeda-lo o [GitHub][GitHub] para isso tive que aprender a utilizar o [Git][Git], neste ponto que fiquei supresso, esta é uma ferramenta extremamente poderosa para o gerenciamento de versões e utilização não é complicada, penso agora em utiliza-lo no meu trabalho para o controle das versões do sistema de gestão ambiental que coordeno.
[Git]: https://git-scm.com/
[GitHub]: https://github.com/  
Espero que este pequeno texto seja o suficiente para que mais pessoas tomem coragem para construir seus próprios sites.
