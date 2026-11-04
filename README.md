# Louvor Pro — Projeção, Slides e Temporizador

Aplicação web para apoiar **projeções de textos, avisos e referências bíblicas**, além de oferecer um **temporizador e relógio** para apresentações e reuniões.

> O nome atual do repositório é `TIMER-`, mas a aplicação se apresenta no código como **Louvor Pro App**.

## Funcionalidades identificadas no código

- Temporizador com controles de início, pausa e reinicialização, alertas de tempo e contagem até horário definido.
- Modo projetor em uma janela separada, com opções de layout e tela escura (*blackout*).
- Cadastro e exibição de textos, avisos e slides.
- Editor de slides para músicos.
- Busca e navegação por textos bíblicos, incluindo opção de download de versões para acesso local.
- Ajustes visuais de fontes, cores, posição e tamanho de texto, relógio e timer.
- Armazenamento local de algumas preferências e conteúdos no navegador.

## Demonstração online

A demonstração foi preparada para publicação em **GitHub Pages**. Quando a publicação estiver ativa, o endereço será:

https://sheldoncupper.github.io/TIMER-/

O workflow de publicação está em `.github/workflows/pages.yml`. A ativação inicial do GitHub Pages em **Settings → Pages → Source: GitHub Actions** pode ser necessária.

## Como executar

1. Abra `index.html` em um navegador atualizado.
2. Configure o conteúdo e as opções de projeção.
3. Ao usar o modo projetor, permita a abertura de uma nova janela, caso o navegador solicite.

A busca de conteúdo online depende de acesso à internet e da disponibilidade de serviços externos. Alguns dados são mantidos no `localStorage`; portanto, não há sincronização automática entre aparelhos.

## Avisos e limitações

- **Projeto em revisão:** a aplicação ainda precisa de testes funcionais, especialmente no modo projetor, com segunda tela, permissões e consulta bíblica.
- O código contém uma integração experimental com a API Gemini, mas a chave está vazia. Não coloque chaves privadas diretamente em HTML/JavaScript público; use um backend seguro para qualquer integração autenticada.
- A disponibilidade, os direitos autorais e as licenças de textos/traduções bíblicas obtidos de terceiros precisam ser verificados antes de distribuir conteúdo.
- O armazenamento local pode ser apagado pelo navegador.
- Não use esta versão sem testes prévios em eventos reais.

Para validação antes de uso real, veja [roteiro de testes](docs/TESTES.md).

## Tecnologias

HTML, CSS, JavaScript e APIs do navegador (`localStorage`, janelas de projeção e comunicação entre abas).

## Próximas melhorias

- [x] Escapar as principais entradas dinâmicas de slides, avisos e versículos na interface (revisão estática; testes de navegador pendentes).
- [ ] Confirmar compatibilidade com projetores, dispositivos móveis e navegadores.
- [ ] Tratar falhas de rede e disponibilidade das fontes bíblicas.
- [ ] Preparar exemplos de uso, capturas e demonstração online depois dos testes.
- [ ] Renomear o repositório para um título mais descritivo, caso desejado.

## Autor

[Gabriel Alves](https://github.com/SheldonCupper)
